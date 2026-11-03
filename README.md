
# ==============================================================================
# PYTHON TUTORIAL SYSTEM
# Strictly using loops, if, elif, else, and nested conditions.
# ==============================================================================

print("=========================================")
print("   WELCOME TO THE PYTHON TUTORIAL SYSTEM ")
print("=========================================")

system_running = True

while system_running:
    print("\n=========================================")
    print("SELECT A QUARTER TO STUDY:")
    print("[1] Prelim (Basics, Data Types, Operators)")
    print("[2] Midterm (If, Elif, Else, Nested Conditions)")
    print("[3] Finals (While Loops, For Loops, Range)")
    print("[4] Exit System")
    print("=========================================")
    
    quarter_choice = input("Enter option (1-4): ")
    
    # ==========================================================================
    # PRELIM QUARTER
    # ==========================================================================
    if quarter_choice == "1":
        prelim_active = True
        while prelim_active:
            print("\n--- PRELIM MENU ---")
            print("[1] Lesson 1: Introduction & Print Statement")
            print("[2] Lesson 2: Data Types & Variables")
            print("[3] Lesson 3: Basic Operators")
            print("[4] Take Prelim Quiz (5 Questions)")
            print("[5] Back to Main Menu")
            
            choice = input("Choose an option (1-5): ")
            
            if choice == "1":
                print("\n-----------------------------------------")
                print("LESSON 1: Print Statement & Syntax")
                print("-----------------------------------------")
                print("The print() function outputs text or values to the console.")
                print("EXAMPLE:")
                print("   print('Hello, Python!')")
                
                play = input("\nDo you want to play the mini-game? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- MINI-GAME: Fill in the Missing Code ---")
                    print("Task: Complete the code to print 'Learning Python!'.")
                    print("Code: ____('Learning Python!')")
                    user_code = input("What goes in the blank? ")
                    if user_code == "print":
                        print("Correct! Great job!")
                    else:
                        print("Incorrect. The correct answer is 'print'.")
                        
            elif choice == "2":
                print("\n-----------------------------------------")
                print("LESSON 2: Data Types & Variables")
                print("-----------------------------------------")
                print("Python supports string, int, float, and boolean data types.")
                print("EXAMPLE:")
                print("   age = 18")
                print("   name = 'Alex'")
                
                play = input("\nDo you want to play the mini-game? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- MINI-GAME: Fill in the Missing Code ---")
                    print("Task: Store the value 10 in a variable named x.")
                    print("Code: x ____ 10")
                    user_code = input("What operator goes in the blank? ")
                    if user_code == "=":
                        print("Correct! Assignment operator '=' assigns values.")
                    else:
                        print("Incorrect. The assignment operator is '='.")
                        
            elif choice == "3":
                print("\n-----------------------------------------")
                print("LESSON 3: Basic Arithmetic Operators")
                print("-----------------------------------------")
                print("Operators: + (Addition), - (Subtraction), * (Multiplication), / (Division), % (Modulus)")
                print("EXAMPLE:")
                print("   result = 10 % 3  # Output is 1")
                
                play = input("\nDo you want to play the mini-game? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- MINI-GAME: Fill in the Missing Code ---")
                    print("Task: Fill in the operator that returns the remainder.")
                    print("Code: remainder = 7 ____ 2")
                    user_code = input("What operator goes in the blank? ")
                    if user_code == "%":
                        print("Correct! '%' is the modulus operator.")
                    else:
                        print("Incorrect. The modulus operator is '%'.")
                        
            elif choice == "4":
                print("\n-----------------------------------------")
                print("PRELIM QUIZ (5 Questions)")
                print("-----------------------------------------")
                score = 0
                
                print("\n1. Which function is used to display text on screen?")
                print("a) display()  b) print()  c) output()")
                ans = input("Answer: ")
                if ans == "b":
                    score = score + 1
                    
                print("\n2. What data type is the value 3.14?")
                print("a) int  b) string  c) float")
                ans = input("Answer: ")
                if ans == "c":
                    score = score + 1
                    
                print("\n3. What is the output of: print(5 + 2 * 3)?")
                print("a) 21  b) 11  c) 13")
                ans = input("Answer: ")
                if ans == "b":
                    score = score + 1
                    
                print("\n4. Which symbol is used for a single-line comment?")
                print("a) //  b) #  c) <!-- -->")
                ans = input("Answer: ")
                if ans == "b":
                    score = score + 1
                    
                print("\n5. What operator is used to get the remainder of division?")
                print("a) /  b) //  c) %")
                ans = input("Answer: ")
                if ans == "c":
                    score = score + 1
                    
                print("\nQUIZ FINISHED! Your Prelim Score:", score, "/5")
                
            elif choice == "5":
                prelim_active = False
            else:
                print("Invalid choice! Please try again.")

    # ==========================================================================
    # MIDTERM QUARTER
    # ==========================================================================
    elif quarter_choice == "2":
        midterm_active = True
        while midterm_active:
            print("\n--- MIDTERM MENU ---")
            print("[1] Lesson 1: IF, ELIF, and ELSE Statements")
            print("[2] Lesson 2: Nested Conditions")
            print("[3] Take Midterm Quiz (5 Questions)")
            print("[4] Back to Main Menu")
            
            choice = input("Choose an option (1-4): ")
            
            if choice == "1":
                print("\n-----------------------------------------")
                print("LESSON 1: Conditional Statements (if, elif, else)")
                print("-----------------------------------------")
                print("Conditionals execute code blocks based on logical criteria.")
                print("EXAMPLE:")
                print("   age = 18")
                print("   if age >= 18:")
                print("       print('Adult')")
                print("   elif age >= 13:")
                print("       print('Teenager')")
                print("   else:")
                print("       print('Child')")
                
                play = input("\nDo you want to play the mini-game? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- MINI-GAME: Fill in the Missing Code ---")
                    print("Task: Fill in the keyword to check an alternate condition.")
                    print("Code:")
                    print("   if score > 90:")
                    print("       print('A')")
                    print("   ____ score > 80:")
                    print("       print('B')")
                    user_code = input("What keyword goes in the blank? ")
                    if user_code == "elif":
                        print("Correct! 'elif' checks secondary conditions.")
                    else:
                        print("Incorrect. The keyword is 'elif'.")

            elif choice == "2":
                print("\n-----------------------------------------")
                print("LESSON 2: Nested Conditions")
                print("-----------------------------------------")
                print("Nested conditions are 'if' statements placed inside other 'if' statements.")
                print("EXAMPLE:")
                print("   has_id = True")
                print("   age = 20")
                print("   if has_id:")
                print("       if age >= 18:")
                print("           print('Entry Allowed')")
                
                play = input("\nDo you want to play the mini-game? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- MINI-GAME: Fill in the Missing Code ---")
                    print("Task: Complete the nested check.")
                    print("Code:")
                    print("   if is_user:")
                    print("       ____ is_admin:")
                    print("           print('Welcome Admin')")
                    user_code = input("What keyword goes in the blank? ")
                    if user_code == "if":
                        print("Correct! 'if' is used for the inner condition.")
                    else:
                        print("Incorrect. The keyword is 'if'.")
                        
            elif choice == "3":
                print("\n-----------------------------------------")
                print("MIDTERM QUIZ (5 Questions)")
                print("-----------------------------------------")
                score = 0
                
                print("\n1. Which keyword starts a conditional check?")
                print("a) when  b) if  c) check")
                ans = input("Answer: ")
                if ans == "b":
                    score = score + 1
                    
                print("\n2. What operator is used to compare equality?")
                print("a) =  b) ==  c) equals")
                ans = input("Answer: ")
                if ans == "b":
                    score = score + 1
                    
                print("\n3. When does the 'else' block execute?")
                print("a) Always  b) When previous conditions are False  c) When previous conditions are True")
                ans = input("Answer: ")
                if ans == "b":
                    score = score + 1
                    
                print("\n4. What is a nested condition?")
                print("a) Condition inside a loop  b) Condition inside another condition  c) Multiple loops")
                ans = input("Answer: ")
                if ans == "b":
                    score = score + 1
                    
                print("\n5. Which operator represents 'Not Equal to'?")
                print("a) !=  b) <>  c) NOT==")
                ans = input("Answer: ")
                if ans == "a":
                    score = score + 1
                    
                print("\nQUIZ FINISHED! Your Midterm Score:", score, "/5")
                
            elif choice == "4":
                midterm_active = False
            else:
                print("Invalid choice! Please try again.")

    # ==========================================================================
    # FINALS QUARTER
    # ==========================================================================
    elif quarter_choice == "3":
        finals_active = True
        while finals_active:
            print("\n--- FINALS MENU ---")
            print("[1] Lesson 1: While Loops")
            print("[2] Lesson 2: For Loops & range()")
            print("[3] Take Finals Quiz (5 Questions)")
            print("[4] Back to Main Menu")
            
            choice = input("Choose an option (1-4): ")
            
            if choice == "1":
                print("\n-----------------------------------------")
                print("LESSON 1: While Loops")
                print("-----------------------------------------")
                print("A while loop repeats code as long as its condition remains True.")
                print("EXAMPLE:")
                print("   count = 1")
                print("   while count <= 3:")
                print("       print(count)")
                print("       count = count + 1")
                
                play = input("\nDo you want to play the mini-game? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- MINI-GAME: Fill in the Missing Code ---")
                    print("Task: Fill in the loop keyword.")
                    print("Code:")
                    print("   ____ x < 5:")
                    print("       x = x + 1")
                    user_code = input("What keyword goes in the blank? ")
                    if user_code == "while":
                        print("Correct! 'while' executes as long as the condition is True.")
                    else:
                        print("Incorrect. The keyword is 'while'.")

            elif choice == "2":
                print("\n-----------------------------------------")
                print("LESSON 2: For Loops & range()")
                print("-----------------------------------------")
                print("For loops iterate over sequences or number ranges using range().")
                print("EXAMPLE:")
                print("   for i in range(3):")
                print("       print(i)")
                
                play = input("\nDo you want to play the mini-game? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- MINI-GAME: Fill in the Missing Code ---")
                    print("Task: Fill in the missing function to generate numbers 0 through 4.")
                    print("Code:")
                    print("   for i in ____(5):")
                    print("       print(i)")
                    user_code = input("What function goes in the blank? ")
                    if user_code == "range":
                        print("Correct! range() generates sequences.")
                    else:
                        print("Incorrect. The function is 'range'.")
                        
            elif choice == "3":
                print("\n-----------------------------------------")
                print("FINALS QUIZ (5 Questions)")
                print("-----------------------------------------")
                score = 0
                
                print("\n1. Which loop runs as long as a condition is True?")
                print("a) for  b) while  c) loop")
                ans = input("Answer: ")
                if ans == "b":
                    score = score + 1
                    
                print("\n2. How many numbers does range(5) produce?")
                print("a) 4  b) 5  c) 6")
                ans = input("Answer: ")
                if ans == "b":
                    score = score + 1
                    
                print("\n3. What is the first number generated by range(3)?")
                print("a) 0  b) 1  c) 3")
                ans = input("Answer: ")
                if ans == "a":
                    score = score + 1
                    
                print("\n4. What happens if a while loop condition never becomes False?")
                print("a) Stops after 100 runs  b) Infinite loop  c) Syntax error")
                ans = input("Answer: ")
                if ans == "b":
                    score = score + 1
                    
                print("\n5. Which keyword is used to iterate over a sequence?")
                print("a) for  b) foreach  c) repeat")
                ans = input("Answer: ")
                if ans == "a":
                    score = score + 1
                    
                print("\nQUIZ FINISHED! Your Finals Score:", score, "/5")
                
            elif choice == "4":
                finals_active = False
            else:
                print("Invalid choice! Please try again.")

    # ==========================================================================
    # EXIT OPTION
    # ==========================================================================
    elif quarter_choice == "4":
        print("\nThank you for using the Python Tutorial System! Goodbye!")
        system_running = False
    else:
        print("\nInvalid choice! Please enter 1, 2, 3, or 4.")
