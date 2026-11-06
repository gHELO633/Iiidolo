print("==================================================")
print("***************** PYTHON TUTORIAL ****************")
print("==================================================")
print(" Welcome to the Interactive Python Learning System ")
print("==================================================")

# User Information & Global Tracking Variables
user_name = input("Enter your Student Name / Username: ")
if user_name == "":
    user_name = "Learner"

prelim_score = 0
midterm_score = 0
finals_score = 0

prelim_taken = False
midterm_taken = False
finals_taken = False

count = True

while count:
    print("\n==================================================")
    print(" STUDENT PROFILE:", user_name)
    print(" PROGRESS TRACKER:")
    
    # Check Prelim Status
    if prelim_taken:
        print("   [1] Prelim Status : COMPLETED (Score:", prelim_score, "/ 5)")
    else:
        print("   [1] Prelim Status : NOT STARTED")
        
    # Check Midterm Status
    if midterm_taken:
        print("   [2] Midterm Status: COMPLETED (Score:", midterm_score, "/ 5)")
    else:
        print("   [2] Midterm Status: NOT STARTED")
        
    # Check Finals Status
    if finals_taken:
        print("   [3] Finals Status : COMPLETED (Score:", finals_score, "/ 5)")
    else:
        print("   [3] Finals Status : NOT STARTED")
        
    print("==================================================")
    print("SELECT A MODULE TO STUDY:")
    print("[1] Prelim  (Intro, Syntax, Variables, Data Types, Operators)")
    print("[2] Midterm (Conditionals: If, Elif, Else & Nested Conditions)")
    print("[3] Finals  (Loops: While Loops, For Loops & range())")
    print("[4] View Complete Student Summary & Analytics")
    print("[5] Exit System")
    print("==================================================")
    
    quarter_choice = input("Enter option (1-5): ")

    # ----------------------------------------------------
    # PRELIM MODULE
    # ----------------------------------------------------
    if quarter_choice == "1":
        prelim_active = True
        current_lesson = 1
        
        while prelim_active:

            if current_lesson == 1:
                print("\n--------------------------------------------------")
                print("PRELIM - LESSON 1: Introduction to Computers & Python")
                print("--------------------------------------------------")
                print("[Explanation]: A computer is an electronic device that processes data.")
                print("Python is a high-level, interpreted programming language known for its")
                print("simplicity and readability, mimicking natural human language.")
                print("[Example Code]:")
                print("   # Computers execute instructions sequentially")
                print("   print('Welcome to Computer Programming!')")
                
                play = input("\nDo you want to play the mini-game for Lesson 1? (yes/no): ")
                if play == "yes" or play == "y" or play == "YES":
                    print("\n--- LESSON 1 MINI-GAME: Output Syntax ---")
                    print("Topic: Python Output Syntax")
                    print("Task: Complete the code to output 'Python is Awesome!'.")
                    print("Code: ____('Python is Awesome!')")
                    user_code = input("What goes in the blank? ")
                    if user_code == "print":
                        print("🌟 EXCELLENT! 'print' displays output to the terminal screen.")
                    else:
                        print("❌ INCORRECT. The correct answer is 'print'.")
                
                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_action = input("Enter option (1-3): ")
                
                if next_action == "1":
                    current_lesson = 2
                elif next_action == "2":
                    current_lesson = 5  
                elif next_action == "3":
                    prelim_active = False
                else:
                    prelim_active = False

            elif current_lesson == 2:
                print("\n--------------------------------------------------")
                print("PRELIM - LESSON 2: Variables & Syntax Rules")
                print("--------------------------------------------------")
                print("[Explanation]: A variable is a container for storing data values.")
                print("Python variable assignment uses the '=' operator. Names cannot start")
                print("with numbers and are case-sensitive.")
                print("[Example Code]:")
                print("   school_name = 'Clark College Of Science And Technology'")
                print("   student_age = 18")
                
                play = input("\nDo you want to play the mini-game for Lesson 2? (yes/no): ")
                if play == "yes" or play == "y" or play == "YES":
                    print("\n--- LESSON 2 MINI-GAME: Variable Assignment ---")
                    print("Topic: Storing Data in Variables")
                    print("Task: Assign the value 100 to a variable named score.")
                    print("Code: score ____ 100")
                    user_code = input("What operator goes in the blank? ")
                    if user_code == "=":
                        print("🌟 EXCELLENT! '=' is the assignment operator in Python.")
                    else:
                        print("❌ INCORRECT. The assignment operator is '='.")
                
                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_action = input("Enter option (1-3): ")
                
                if next_action == "1":
                    current_lesson = 3
                elif next_action == "2":
                    current_lesson = 5
                elif next_action == "3":
                    prelim_active = False
                else:
                    prelim_active = False

            elif current_lesson == 3:
                print("\n--------------------------------------------------")
                print("PRELIM - LESSON 3: Python Data Types")
                print("--------------------------------------------------")
                print("[Explanation]: Data types define the type of value a variable holds.")
                print("Main types: Integer (int), Floating-point (float), String (str), and Boolean (bool).")
                print("[Example Code]:")
                print("   x = 10        # int")
                print("   pi = 3.14     # float")
                print("   msg = 'Hi'    # str")
                print("   is_pass = True # bool")
                
                play = input("\nDo you want to play the mini-game for Lesson 3? (yes/no): ")
                if play == "yes" or play == "y" or play == "YES":
                    print("\n--- LESSON 3 MINI-GAME: Identifying String Type ---")
                    print("Topic: Data Types (str)")
                    print("Task: Fill in the built-in type keyword for text data.")
                    print("Code: my_text = ____('Hello World')")
                    user_code = input("What data type function goes in the blank? ")
                    if user_code == "str":
                        print("🌟 EXCELLENT! 'str' represents the string data type.")
                    else:
                        print("❌ INCORRECT. The data type keyword is 'str'.")
                
                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_action = input("Enter option (1-3): ")
                
                if next_action == "1":
                    current_lesson = 4
                elif next_action == "2":
                    current_lesson = 5
                elif next_action == "3":
                    prelim_active = False
                else:
                    prelim_active = False

            elif current_lesson == 4:
                print("\n--------------------------------------------------")
                print("PRELIM - LESSON 4: Basic Arithmetic Operators")
                print("--------------------------------------------------")
                print("[Explanation]: Operators perform operations on variables and values.")
                print("Arithmetic includes +, -, *, /, and modulus (%) which yields division remainder.")
                print("[Example Code]:")
                print("   sum_result = 5 + 3")
                print("   remainder = 10 % 3  # Output is 1")
                
                play = input("\nDo you want to play the mini-game for Lesson 4? (yes/no): ")
                if play == "yes" or play == "y" or play == "YES":
                    print("\n--- LESSON 4 MINI-GAME: Modulus Operator ---")
                    print("Topic: Modulus / Remainder Operator")
                    print("Task: Fill in the missing operator symbol that calculates the division remainder.")
                    print("Code: remainder = 9 ____ 4")
                    user_code = input("What operator symbol goes in the blank? ")
                    if user_code == "%":
                        print("🌟 EXCELLENT! '%' is the modulus operator.")
                    else:
                        print("❌ INCORRECT. The modulus operator is '%'.")
                
                print("\nWhat would you like to do next?")
                print("[1] Take Prelim Quiz")
                print("[2] Back to Main Menu")
                next_action = input("Enter option (1-2): ")
                
                if next_action == "1":
                    current_lesson = 5
                else:
                    prelim_active = False

            elif current_lesson == 5:
                print("\n--------------------------------------------------")
                print("PRELIM QUIZ (5 Questions)")
                print("--------------------------------------------------")
                score = 0
                
                print("\n1. Which function outputs text to the screen in Python?")
                print("a) display()  b) print()  c) echo()")
                ans = input("Answer: ")
                if ans == "b" or ans == "B":
                    score = score + 1
                    
                print("\n2. Which of the following is a valid variable name?")
                print("a) 2nd_name  b) user-name  c) user_name")
                ans = input("Answer: ")
                if ans == "c" or ans == "C":
                    score = score + 1
                    
                print("\n3. What data type is the value 99.5?")
                print("a) int  b) float  c) str")
                ans = input("Answer: ")
                if ans == "b" or ans == "B":
                    score = score + 1
                    
                print("\n4. What is the output of 10 % 3?")
                print("a) 3  b) 0.33  c) 1")
                ans = input("Answer: ")
                if ans == "c" or ans == "C":
                    score = score + 1
                    
                print("\n5. Which symbol is used for single-line comments in Python?")
                print("a) #  b) //  c) /*")
                ans = input("Answer: ")
                if ans == "a" or ans == "A":
                    score = score + 1
                    
                print("\n--------------------------------------------------")
                print("🏆 QUIZ FINISHED! Your Prelim Score:", score, "/ 5")
                if score == 5:
                    print("Badge Earned: 🏅 Syntax Master")
                elif score >= 3:
                    print("Badge Earned: 🥈 Syntax Apprentice")
                else:
                    print("Badge Earned: 📘 Beginner Learner (Needs Review)")
                print("--------------------------------------------------")
                
                prelim_score = score
                prelim_taken = True
                prelim_active = False

    # ----------------------------------------------------
    # MIDTERM MODULE
    # ----------------------------------------------------
    elif quarter_choice == "2":
        midterm_active = True
        current_lesson = 1
        
        while midterm_active:

            if current_lesson == 1:
                print("\n--------------------------------------------------")
                print("MIDTERM - LESSON 1: Conditional Statements (if, elif, else)")
                print("--------------------------------------------------")
                print("[Explanation]: Conditional statements allow the program to make decisions.")
                print("`if` checks a condition, `elif` checks alternate conditions, and `else` handles fallback.")
                print("[Example Code]:")
                print("   score = 85")
                print("   if score >= 90:")
                print("       print('A')")
                print("   elif score >= 80:")
                print("       print('B')")
                print("   else:")
                print("       print('C')")
                
                play = input("\nDo you want to play the mini-game for Lesson 1? (yes/no): ")
                if play == "yes" or play == "y" or play == "YES":
                    print("\n--- LESSON 1 MINI-GAME: Alternate Condition Checking ---")
                    print("Topic: If/Elif/Else Syntax")
                    print("Task: Fill in the keyword used for checking an alternate condition.")
                    print("Code:")
                    print("   if score > 90:")
                    print("       print('A')")
                    print("   ____ score > 80:")
                    print("       print('B')")
                    user_code = input("What keyword goes in the blank? ")
                    if user_code == "elif":
                        print("🌟 EXCELLENT! 'elif' checks secondary conditions.")
                    else:
                        print("❌ INCORRECT. The keyword is 'elif'.")
                
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

            elif current_lesson == 2:
                print("\n--------------------------------------------------")
                print("MIDTERM - LESSON 2: Nested Conditions")
                print("--------------------------------------------------")
                print("[Explanation]: A nested condition is an `if` statement placed inside")
                print("another `if` statement, allowing multi-layered decision-making logic.")
                print("[Example Code]:")
                print("   has_id = True")
                print("   age = 20")
                print("   if has_id:")
                print("       if age >= 18:")
                print("           print('Allowed to Enter')")
                
                play = input("\nDo you want to play the mini-game for Lesson 2? (yes/no): ")
                if play == "yes" or play == "y" or play == "YES":
                    print("\n--- LESSON 2 MINI-GAME: Inner Condition Check ---")
                    print("Topic: Nested If Statements")
                    print("Task: Fill in the inner condition keyword to check admin status.")
                    print("Code:")
                    print("   if is_user:")
                    print("       ____ is_admin:")
                    print("           print('Welcome Admin')")
                    user_code = input("What keyword goes in the blank? ")
                    if user_code == "if":
                        print("🌟 EXCELLENT! 'if' initiates the nested inner condition.")
                    else:
                        print("❌ INCORRECT. The keyword is 'if'.")
                
                print("\nWhat would you like to do next?")
                print("[1] Take Midterm Quiz")
                print("[2] Back to Main Menu")
                next_action = input("Enter option (1-2): ")
                
                if next_action == "1":
                    current_lesson = 3
                else:
                    midterm_active = False

            elif current_lesson == 3:
                print("\n--------------------------------------------------")
                print("MIDTERM QUIZ (5 Questions)")
                print("--------------------------------------------------")
                score = 0
                
                print("\n1. Which keyword is used to begin a conditional statement?")
                print("a) check  b) if  c) when")
                ans = input("Answer: ")
                if ans == "b" or ans == "B":
                    score = score + 1
                    
                print("\n2. What operator is used for equality comparison in Python?")
                print("a) =  b) ==  c) equals")
                ans = input("Answer: ")
                if ans == "b" or ans == "B":
                    score = score + 1
                    
                print("\n3. When does the `else` block execute?")
                print("a) Always  b) When previous conditions are True  c) When all previous conditions are False")
                ans = input("Answer: ")
                if ans == "c" or ans == "C":
                    score = score + 1
                    
                print("\n4. What is a nested condition?")
                print("a) Condition inside another condition  b) Condition inside a loop  c) Multiple loops")
                ans = input("Answer: ")
                if ans == "a" or ans == "A":
                    score = score + 1
                    
                print("\n5. Which operator means 'Not Equal to'?")
                print("a) !=  b) <>  c) NOT==")
                ans = input("Answer: ")
                if ans == "a" or ans == "A":
                    score = score + 1
                    
                print("\n--------------------------------------------------")
                print("🏆 QUIZ FINISHED! Your Midterm Score:", score, "/ 5")
                if score == 5:
                    print("Badge Earned: 🏅 Logic Master")
                elif score >= 3:
                    print("Badge Earned: 🥈 Logic Tactician")
                else:
                    print("Badge Earned: 📘 Logic Novice (Needs Review)")
                print("--------------------------------------------------")
                
                midterm_score = score
                midterm_taken = True
                midterm_active = False

    # ----------------------------------------------------
    # FINALS MODULE
    # ----------------------------------------------------
    elif quarter_choice == "3":
        finals_active = True
        current_lesson = 1
        
        while finals_active:
            
            if current_lesson == 1:
                print("\n--------------------------------------------------")
                print("FINALS - LESSON 1: While Loops")
                print("--------------------------------------------------")
                print("[Explanation]: A `while` loop repeatedly executes code blocks as long")
                print("as its specified condition evaluates to True.")
                print("[Example Code]:")
                print("   count = 1")
                print("   while count <= 3:")
                print("       print(count)")
                print("       count = count + 1")
                
                play = input("\nDo you want to play the mini-game for Lesson 1? (yes/no): ")
                if play == "yes" or play == "y" or play == "YES":
                    print("\n--- LESSON 1 MINI-GAME: Conditional Loop Header ---")
                    print("Topic: While Loop Mechanics")
                    print("Task: Fill in the loop keyword that repeats code while a condition is True.")
                    print("Code:")
                    print("   ____ count < 5:")
                    print("       count = count + 1")
                    user_code = input("What keyword goes in the blank? ")
                    if user_code == "while":
                        print("🌟 EXCELLENT! 'while' creates a conditional loop.")
                    else:
                        print("❌ INCORRECT. The keyword is 'while'.")
                
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

            elif current_lesson == 2:
                print("\n--------------------------------------------------")
                print("FINALS - LESSON 2: For Loops & range()")
                print("--------------------------------------------------")
                print("[Explanation]: A `for` loop iterates over sequences or items.")
                print("The `range()` function is commonly used to generate a sequence of numbers.")
                print("[Example Code]:")
                print("   for i in range(3):")
                print("       print(i)  # Prints 0, 1, 2")
                
                play = input("\nDo you want to play the mini-game for Lesson 2? (yes/no): ")
                if play == "yes" or play == "y" or play == "YES":
                    print("\n--- LESSON 2 MINI-GAME: Sequence Generation ---")
                    print("Topic: For Loop & Range Function")
                    print("Task: Fill in the function used to generate numeric sequences in for loops.")
                    print("Code:")
                    print("   for i in ____(5):")
                    print("       print(i)")
                    user_code = input("What function name goes in the blank? ")
                    if user_code == "range":
                        print("🌟 EXCELLENT! 'range' generates number sequences.")
                    else:
                        print("❌ INCORRECT. The function name is 'range'.")
                
                print("\nWhat would you like to do next?")
                print("[1] Take Finals Quiz")
                print("[2] Back to Main Menu")
                next_action = input("Enter option (1-2): ")
                
                if next_action == "1":
                    current_lesson = 3
                else:
                    finals_active = False

            elif current_lesson == 3:
                print("\n--------------------------------------------------")
                print("FINALS QUIZ (5 Questions)")
                print("--------------------------------------------------")
                score = 0
                
                print("\n1. Which loop runs as long as a condition remains True?")
                print("a) for  b) while  c) repeat")
                ans = input("Answer: ")
                if ans == "b" or ans == "B":
                    score = score + 1
                    
                print("\n2. How many iterations does range(5) produce?")
                print("a) 4  b) 5  c) 6")
                ans = input("Answer: ")
                if ans == "b" or ans == "B":
                    score = score + 1
                    
                print("\n3. What is the starting number generated by range(3) by default?")
                print("a) 0  b) 1  c) 3")
                ans = input("Answer: ")
                if ans == "a" or ans == "A":
                    score = score + 1
                    
                print("\n4. What occurs if a while loop condition never turns False?")
                print("a) Syntax Error  b) Infinite Loop  c) Program Auto-Fix")
                ans = input("Answer: ")
                if ans == "b" or ans == "B":
                    score = score + 1
                    
                print("\n5. Which keyword is used to start a for loop in Python?")
                print("a) for  b) foreach  c) loop")
                ans = input("Answer: ")
                if ans == "a" or ans == "A":
                    score = score + 1
                    
                print("\n--------------------------------------------------")
                print("🏆 QUIZ FINISHED! Your Finals Score:", score, "/ 5")
                if score == 5:
                    print("Badge Earned: 🏅 Loop Master")
                elif score >= 3:
                    print("Badge Earned: 🥈 Loop Specialist")
                else:
                    print("Badge Earned: 📘 Iteration Beginner (Needs Review)")
                print("--------------------------------------------------")
                
                finals_score = score
                finals_taken = True
                finals_active = False

    # ----------------------------------------------------
    # VIEW STUDENT SUMMARY & ANALYTICS
    # ----------------------------------------------------
    elif quarter_choice == "4":
        print("\n==================================================")
        print("         🎓 STUDENT ACADEMIC SUMMARY 🎓           ")
        print("==================================================")
        print("Student Name:", user_name)
        
        total_quizzes_taken = 0
        total_accumulated_score = 0
        
        if prelim_taken:
            print(" - Prelim Quiz Score  :", prelim_score, "/ 5")
            total_quizzes_taken = total_quizzes_taken + 1
            total_accumulated_score = total_accumulated_score + prelim_score
        else:
            print(" - Prelim Quiz Score  : Not Completed")
            
        if midterm_taken:
            print(" - Midterm Quiz Score :", midterm_score, "/ 5")
            total_quizzes_taken = total_quizzes_taken + 1
            total_accumulated_score = total_accumulated_score + midterm_score
        else:
            print(" - Midterm Quiz Score : Not Completed")
            
        if finals_taken:
            print(" - Finals Quiz Score  :", finals_score, "/ 5")
            total_quizzes_taken = total_quizzes_taken + 1
            total_accumulated_score = total_accumulated_score + finals_score
        else:
            print(" - Finals Quiz Score  : Not Completed")
            
        print("--------------------------------------------------")
        print("Total Quizzes Completed:", total_quizzes_taken, "/ 3")
        print("Total Overall Score    :", total_accumulated_score, "/ 15")
        
        # Calculate evaluation ranking
        if total_quizzes_taken == 3:
            if total_accumulated_score == 15:
                print("FINAL GRADE: 🏆 PERFECT ACADEMIC EXCELLENCE (100%)")
            elif total_accumulated_score >= 12:
                print("FINAL GRADE: 🌟 HIGH HONORS - PYTHON MASTER")
            elif total_accumulated_score >= 9:
                print("FINAL GRADE: 👍 SATISFACTORY - PASSED")
            else:
                print("FINAL GRADE: ⚠️ NEEDS REVISION & STUDY")
        else:
            print("STATUS: Complete all 3 module quizzes to calculate your overall grade!")
        print("==================================================")

    # ----------------------------------------------------
    # EXIT SYSTEM
    # ----------------------------------------------------
    elif quarter_choice == "5":
        print("\n==================================================")
        print("Thank you for using the Python Tutorial System,", user_name, "!")
        print("Keep practicing and happy coding!")
        print("==================================================")
        count = False
        
    else:
        print("\n⚠️ Invalid choice! Please select an option between 1 and 5.")
