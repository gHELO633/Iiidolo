

def tutorial_system():
    print("=== Welcome to the Tutorial Quiz System ===")
    print("Choose a subject:")
    print("1. Python Basics")
    print("2. Mathematics")
    print("3. Science")

    try:
        choice = int(input("Enter your choice (1-3): "))
    except ValueError:
        print("Invalid input. Please enter a number between 1 and 3.")
        return

    score = 0 

    # Outer condition: subject selection
    if choice == 1:
        print("\n--- Python Basics Tutorial ---")
        print("Let's start the quiz! Answer with the correct option number.\n")

        # Nested quiz loop
        for i in range(1, 6):
            if i == 1:
                print("Q1: Which keyword is used to define a function in Python?")
                print("1. func\n2. def\n3. function\n4. define")
                ans = input("Your answer: ")
                if ans == "2":
                    score += 1
            elif i == 2:
                print("Q2: Which symbol is used for comments in Python?")
                print("1. //\n2. #\n3. /* */\n4. <!-- -->")
                ans = input("Your answer: ")
                if ans == "2":
                    score += 1
            elif i == 3:
                print("Q3: Which data type is used for decimal numbers?")
                print("1. int\n2. float\n3. str\n4. bool")
                ans = input("Your answer: ")
                if ans == "2":
                    score += 1
            elif i == 4:
                print("Q4: Which function is used to get user input?")
                print("1. input()\n2. read()\n3. scan()\n4. get()")
                ans = input("Your answer: ")
                if ans == "1":
                    score += 1
            elif i == 5:
                print("Q5: Which keyword is used for conditional branching?")
                print("1. if\n2. elif\n3. else\n4. All of the above")
                ans = input("Your answer: ")
                if ans == "4":
                    score += 1

    elif choice == 2:
        print("\n--- Mathematics Tutorial ---")
        print("Let's start the quiz!\n")

        for i in range(1, 6):
            if i == 1:
                print("Q1: What is 5 + 3?")
                print("1. 7\n2. 8\n3. 9\n4. 10")
                ans = input("Your answer: ")
                if ans == "2":
                    score += 1
            elif i == 2:
                print("Q2: What is the square root of 16?")
                print("1. 2\n2. 4\n3. 8\n4. 16")
                ans = input("Your answer: ")
                if ans == "2":
                    score += 1
            elif i == 3:
                print("Q3: What is 10 / 2?")
                print("1. 4\n2. 5\n3. 6\n4. 8")
                ans = input("Your answer: ")
                if ans == "2":
                    score += 1
            elif i == 4:
                print("Q4: What is 7 * 6?")
                print("1. 42\n2. 36\n3. 48\n4. 40")
                ans = input("Your answer: ")
                if ans == "1":
                    score += 1
            elif i == 5:
                print("Q5: What is 15 - 9?")
                print("1. 5\n2. 6\n3. 7\n4. 8")
                ans = input("Your answer: ")
                if ans == "2":
                    score += 1

    elif choice == 3:
        print("\n--- Science Tutorial ---")
        print("Let's start the quiz!\n")

        for i in range(1, 6):
            if i == 1:
                print("Q1: What planet is known as the Red Planet?")
                print("1. Earth\n2. Mars\n3. Jupiter\n4. Venus")
                ans = input("Your answer: ")
                if ans == "2":
                    score += 1
            elif i == 2:
                print("Q2: What gas do plants produce during photosynthesis?")
                print("1. Oxygen\n2. Carbon Dioxide\n3. Nitrogen\n4. Hydrogen")
                ans = input("Your answer: ")
                if ans == "1":
                    score += 1
            elif i == 3:
                print("Q3: What is H2O commonly known as?")
                print("1. Water\n2. Hydrogen Peroxide\n3. Salt\n4. Oxygen")
                ans = input("Your answer: ")
                if ans == "1":
                    score += 1
            elif i == 4:
                print("Q4: Which organ pumps blood in the human body?")
                print("1. Brain\n2. Heart\n3. Lungs\n4. Liver")
                ans = input("Your answer: ")
                if ans == "2":
                    score += 1
            elif i == 5:
                print("Q5: What force keeps us on the ground?")
                print("1. Magnetism\n2. Gravity\n3. Friction\n4. Inertia")
                ans = input("Your answer: ")
                if ans == "2":
                    score += 1

    else:
        print("Invalid choice. Please restart and choose between 1-3.")
        return

    # Final score display
    print(f"\nYour score: {score}/5")
    if score == 5:
        print("Excellent! You got all correct.")
    elif score >= 3:
        print("Good job! You passed.")
    else:
        print("Keep practicing! You can do better.")

# Run the system
tutorial_system()
