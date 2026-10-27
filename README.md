class CarWashSystem:
    def __init__(self):
        # Define available services and their prices
        self.packages = {
            1: {"name": "Basic Wash (Exterior Only)", "price": 10.00},
            2: {"name": "Standard Wash (Exterior + Interior)", "price": 20.00},
            3: {"name": "Premium Wash (Full Detail + Wax)", "price": 35.00}
        }
        
        self.addons = {
            1: {"name": "Tire Shine", "price": 5.00},
            2: {"name": "Rain Repellent Windshield", "price": 7.00},
            3: {"name": "Fragrance/Air Freshener", "price": 3.00}
        }
        
        self.queue = []

    def display_menu(self):
        print("\n" + "="*40)
        print("      WELCOME TO PYTHON CAR WASH      ")
        print("="*40)
        print("Please choose a wash package:")
        for key, pkg in self.packages.items():
            print(f"  [{key}] {pkg['name']} - ${pkg['price']:.2f}")

    def display_addons(self):
        print("\nOptional Add-ons:")
        print("  [0] None / Done selecting")
        for key, addon in self.addons.items():
            print(f"  [{key}] {addon['name']} - ${addon['price']:.2f}")

    def start(self):
        while True:
            self.display_menu()
            try:
                choice = int(input("\nEnter package number (or 0 to exit): "))
                if choice == 0:
                    print("\nThank you for visiting Python Car Wash. Goodbye!")
                    break
                
                if choice not in self.packages:
                    print("\n[Error] Invalid choice. Please select 1, 2, or 3.")
                    continue

                # Get package details
                selected_package = self.packages[choice]
                total_cost = selected_package["price"]
                invoice_items = [selected_package]

                # Get add-ons
                while True:
                    self.display_addons()
                    addon_choice = int(input("Select an add-on number (0 to finish): "))
                    if addon_choice == 0:
                        break
                    elif addon_choice in self.addons:
                        addon = self.addons[addon_choice]
                        # Prevent duplicate add-ons
                        if addon not in invoice_items:
                            invoice_items.append(addon)
                            total_cost += addon["price"]
                            print(f"Added: {addon['name']}")
                        else:
                            print("You already added this item.")
                    else:
                        print("[Error] Invalid add-on choice.")

                # Get customer info
                customer_name = input("\nEnter customer name: ").strip()
                car_model = input("Enter car model/plate number: ").strip()

                # Add to queue
                order_summary = {
                    "name": customer_name,
                    "car": car_model,
                    "items": invoice_items,
                    "total": total_cost
                }
                self.queue.append(order_summary)

                # Print Receipt / Ticket
                print("\n" + "-"*40)
                print("           CAR WASH TICKET            ")
                print("-"*40)
                print(f"Customer : {customer_name}")
                print(f"Vehicle  : {car_model}")
                print("\nSelected Services:")
                for item in invoice_items:
                    print(f" - {item['name']} (${item['price']:.2f})")
                print("-" * 40)
                print(f"TOTAL DUE: ${total_cost:.2f}")
                print("-"*40)
                print(f"Status: Added to queue. Position: {len(self.queue)}")
                print("Please drive your car to the wash bay!\n")

                cont = input("Process another car? (y/n): ").strip().lower()
                if cont != 'y':
                    print("\nCurrent Queue Summary:")
                    for i, job in enumerate(self.queue, 1):
                        print(f" {i}. {job['name']} ({job['car']}) - Total: ${job['total']:.2f}")
                    print("\nThank you for using the system!")
                    break

            except ValueError:
                print("\n[Error] Please enter a valid number.")

if __name__ == "__main__":
    car_wash = CarWashSystem()
    car_wash.start()
