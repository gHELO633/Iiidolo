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
    print("[3] Finals (While & For Loops)")
    print("[4] Exit System")
    print("=========================================")
    
    quarter_choice = input("Enter option (1-4): ")
    
    # ==========================================================================
    # PRELIM QUARTER
    # ==========================================================================
    if quarter_choice == "1":
        prelim_active = True
        current_lesson = 1
        
        while prelim_active:
            # ------------------------------------------------------------------
            # PRELIM LESSON 1
            # ------------------------------------------------------------------
            if current_lesson == 1:
                print("\n-----------------------------------------")
                print("PRELIM - LESSON 1: Print Statement & Syntax")
                print("-----------------------------------------")
                print("[Explanation]: The print() function is used to display text,")
                print("numbers, or results onto the console screen.")
                print("[Example Code]:")
                print("   print('Hello, World!')")
                print("   print(25 + 5)")
                
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
                
                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_action = input("Enter option (1-3): ")
                
                if next_action == "1":
                    current_lesson = 2
                elif next_action == "2":
                    current_lesson = 4  # Jump to Quiz
                elif next_action == "3":
                    prelim_active = False
                else:
                    prelim_active = False

            # ------------------------------------------------------------------
            # PRELIM LESSON 2
            # ------------------------------------------------------------------
            elif current_lesson == 2:
                print("\n-----------------------------------------")
                print("PRELIM - LESSON 2: Data Types & Variables")
                print("-----------------------------------------")
                print("[Explanation]: Variables store data values. Common types include")
                print("Strings (text), Integers (whole numbers), Floats (decimals), and Booleans.")
                print("[Example Code]:")
                print("   name = 'Alice'  # String")
                print("   age = 17        # Integer")
                print("   price = 99.95   # Float")
                print("   is_active = True  # Boolean")
                
                play = input("\nDo you want to play the mini-game? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- MINI-GAME: Fill in the Missing Code ---")
                    print("Task: Store the value 10 into a variable named x.")
                    print("Code: x ____ 10")
                    user_code = input("What operator goes in the blank? ")
                    if user_code == "=":
                        print("Correct! '=' assigns values to variables.")
                    else:
                        print("Incorrect. The assignment operator is '='.")
                
                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_action = input("Enter option (1-3): ")
                
                if next_action == "1":
                    current_lesson = 3
                elif next_action == "2":
                    current_lesson = 4
                elif next_action == "3":
                    prelim_active = False
                else:
                    prelim_active = False

            # ------------------------------------------------------------------
            # PRELIM LESSON 3
            # ------------------------------------------------------------------
            elif current_lesson == 3:
                print("\n-----------------------------------------")
                print("PRELIM - LESSON 3: Basic Operators")
                print("-----------------------------------------")
                print("[Explanation]: Arithmetic operators perform mathematical calculations")
                print("like addition (+), subtraction (-), multiplication (*), and modulus (%).")
                print("[Example Code]:")
                print("   total = 10 + 5")
                print("   remainder = 10 % 3  # Results in 1")
                
                play = input("\nDo you want to play the mini-game? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- MINI-GAME: Fill in the Missing Code ---")
                    print("Task: Fill in the operator that returns the division remainder.")
                    print("Code: remainder = 7 ____ 2")
                    user_code = input("What operator goes in the blank? ")
                    if user_code == "%":
                        print("Correct! '%' is the modulus operator.")
                    else:
                        print("Incorrect. The modulus operator is '%'.")
                
                print("\nWhat would you like to do next?")
                print("[1] Take Prelim Quiz")
                print("[2] Back to Main Menu")
                next_action = input("Enter option (1-2): ")
                
                if next_action == "1":
                    current_lesson = 4
                else:
                    prelim_active = False

            # ------------------------------------------------------------------
            # PRELIM QUIZ
            # ------------------------------------------------------------------
            elif current_lesson == 4:
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
                prelim_active = False

    # ==========================================================================
    # MIDTERM QUARTER
    # ==========================================================================
    elif quarter_choice == "2":
        midterm_active = True
        current_lesson = 1
        
        while midterm_active:
            # ------------------------------------------------------------------
            # MIDTERM LESSON 1
            # ------------------------------------------------------------------
            if current_lesson == 1:
                print("\n-----------------------------------------")
                print("MIDTERM - LESSON 1: IF, ELIF, and ELSE Statements")
                print("-----------------------------------------")
                print("[Explanation]: Conditional statements allow programs to make decisions")
                print("based on whether conditions evaluate to True or False.")
                print("[Example Code]:")
                print("   score = 85")
                print("   if score >= 90:")
                print("       print('Grade: A')")
                print("   elif score >= 80:")
                print("       print('Grade: B')")
                print("   else:")
                print("       print('Grade: C')")
                
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
                
                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Midterm Quiz")
                print("[3] Back to Main Menu")
                next_action = input("Enter option (1-3): ")
                
                if next_action == "1":
                    current_lesson = 2
                elif next_action == "2":
                    current_lesson = 3
                else:
                    midterm_active = False

            # ------------------------------------------------------------------
            # MIDTERM LESSON 2
            # ------------------------------------------------------------------
            elif current_lesson == 2:
                print("\n-----------------------------------------")
                print("MIDTERM - LESSON 2: Nested Conditions")
                print("-----------------------------------------")
                print("[Explanation]: A nested condition is an 'if' statement placed")
                print("inside another 'if' statement to handle multi-layered logic.")
                print("[Example Code]:")
                print("   has_id = True")
                print("   age = 20")
                print("   if has_id:")
                print("       if age >= 18:")
                print("           print('Access Granted')")
                
                play = input("\nDo you want to play the mini-game? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- MINI-GAME: Fill in the Missing Code ---")
                    print("Task: Complete the inner condition.")
                    print("Code:")
                    print("   if is_user:")
                    print("       ____ is_admin:")
                    print("           print('Welcome Admin')")
                    user_code = input("What keyword goes in the blank? ")
                    if user_code == "if":
                        print("Correct! 'if' is used for the nested check.")
                    else:
                        print("Incorrect. The keyword is 'if'.")
                
                print("\nWhat would you like to do next?")
                print("[1] Take Midterm Quiz")
                print("[2] Back to Main Menu")
                next_action = input("Enter option (1-2): ")
                
                if next_action == "1":
                    current_lesson = 3
                else:
                    midterm_active = False

            # ------------------------------------------------------------------
            # MIDTERM QUIZ
            # ------------------------------------------------------------------
            elif current_lesson == 3:
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
                print("a) Always  b) When previous are False  c) When previous are True")
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
                midterm_active = False

    # ==========================================================================
    # FINALS QUARTER
    # ==========================================================================
    elif quarter_choice == "3":
        finals_active = True
        current_lesson = 1
        
        while finals_active:
            # ------------------------------------------------------------------
            # FINALS LESSON 1
            # ------------------------------------------------------------------
            if current_lesson == 1:
                print("\n-----------------------------------------")
                print("FINALS - LESSON 1: While Loops")
                print("-----------------------------------------")
                print("[Explanation]: A while loop repeatedly executes a block of code")
                print("as long as its specified conditional statement remains True.")
                print("[Example Code]:")
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
                        print("Correct! 'while' runs as long as the condition is True.")
                    else:
                        print("Incorrect. The keyword is 'while'.")
                
                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Finals Quiz")
                print("[3] Back to Main Menu")
                next_action = input("Enter option (1-3): ")
                
                if next_action == "1":
                    current_lesson = 2
                elif next_action == "2":
                    current_lesson = 3
                else:
                    finals_active = False

            # ------------------------------------------------------------------
            # FINALS LESSON 2
            # ------------------------------------------------------------------
            elif current_lesson == 2:
                print("\n-----------------------------------------")
                print("FINALS - LESSON 2: For Loops & range()")
                print("-----------------------------------------")
                print("[Explanation]: A for loop iterates over sequences or number ranges")
                print("generated by functions like range() to execute repeatable tasks.")
                print("[Example Code]:")
                print("   for i in range(3):")
                print("       print(i)  # Prints 0, 1, 2")
                
                play = input("\nDo you want to play the mini-game? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- MINI-GAME: Fill in the Missing Code ---")
                    print("Task: Fill in the missing function to generate a sequence of numbers.")
                    print("Code:")
                    print("   for i in ____(5):")
                    print("       print(i)")
                    user_code = input("What function goes in the blank? ")
                    if user_code == "range":
                        print("Correct! range() generates numbers.")
                    else:
                        print("Incorrect. The function is 'range'.")
                
                print("\nWhat would you like to do next?")
                print("[1] Take Finals Quiz")
                print("[2] Back to Main Menu")
                next_action = input("Enter option (1-2): ")
                
                if next_action == "1":
                    current_lesson = 3
                else:
                    finals_active = False

            # ------------------------------------------------------------------
            # FINALS QUIZ
            # ------------------------------------------------------------------
            elif current_lesson == 3:
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
                finals_active = False

    # ==========================================================================
    # EXIT OPTION
    # ==========================================================================
    elif quarter_choice == "4":
        print("\nThank you for using the Python Tutorial System! Goodbye!")
        system_running = False
    else:
        print("\nInvalid choice! Please enter 1, 2, 3, or 4.")
