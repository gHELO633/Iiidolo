print("==================================================")
print("***************🐍PYTHON TUTORIAL🐍****************")
print("==================================================")
print("   Welcome To My Python Learning Tutorial System  ")
print("==================================================")

student_name = input("Enter your student name / username: ")


if student_name == "":
    student_name = "Learner"

prelim_score = 0
midterm_score = 0
finals_score = 0

prelim_taken = False
midterm_taken = False
finals_taken = False

count = True

while count:
    print("\n==================================================")
    print(f" STUDENT PROFILE: {student_name}")
    print(" SCORE TRACKER:")

    if prelim_taken:
        print(f"   [1] Prelim Status : COMPLETED (Score: {prelim_score} / 5)")
    else:
        print("   [1] Prelim Status : NOT STARTED YET")

    if midterm_taken:
        print(f"   [2] Midterm Status: COMPLETED (Score: {midterm_score} / 5)")
    else:
        print("   [2] Midterm Status: NOT STARTED YET")

    if finals_taken:
        print(f"   [3] Finals Status : COMPLETED (Score: {finals_score} / 5)")
    else:
        print("   [3] Finals Status : NOT STARTED YET")

    print("《《《《《《《《《《《《《《《》》》》》》》》》》》》》》》")
    print("SELECT A LESSON TO STUDY:")
    print("[1] Prelim  (Intro, Syntax, Variables, Data Types, Operators)")
    print("[2] Midterm (Conditionals: If, Elif, Else & Nested Conditions)")
    print("[3] Finals  (Loops: While Loops, For Loops & range())")
    print("[4] View Student Progress or Score")
    print("[5] Exit System")
    print("《《《《《《《《《《《《《《《》》》》》》》》》》》》》》》")

    term_choice = input("Enter option (1-5): ")

    if term_choice == "1":
        prelim_latest = True
        current_lesson = 1

        while prelim_latest:
            if current_lesson == 1:
                print("\n------------------------------------------------")
                print("PRELIM - Introduction to Computers & Python")
                print("--------------------------------------------------")
                print("[Explanation]: Foundations of Programming & Python")
                print("• What is Programming?")
                print("  - A specialized language used to communicate instructions to computers.")
                print("  - Common languages: Python, C++, PHP, Java, JavaScript, Ruby.")
                print("• About Python:")
                print("  - Created by Guido van Rossum in 1991.")
                print("  - High-level, interpreted, and general-purpose.")
                print("• Key Advantages of Learning Python:")
                print("  1. Simple, clean, and beginner-friendly syntax")
                print("  2. Highly readable code structure")
                print("  3. Exceptional versatility across domains")
                print("  4. Massive global community support")

                play = input("\nDo you want to play the mini-game for Lesson 1? (yes/no): ").lower()
                if play in ["yes", "y"]:
                    print("\n--- LESSON 1 MINI-GAME: INTRODUCTION TO PYTHON ---")
                    print("Topic: Python Basics")
                    print("Task: Who created the Python programming language?")
                    print("Answer: __________________")
                    user_answer = input("What goes in the blank? ").lower()
                    if user_answer == "guido van rossum":
                        print("GREAT JOB! Guido van Rossum is the correct answer.")
                    else:
                        print("IT'S OKAY TRY AGAIN. The correct answer is 'Guido van Rossum'.")

                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_input = input("Enter option (1-3): ")

                if next_input == "1":
                    current_lesson = 2
                elif next_input == "2":
                    current_lesson = 5
                elif next_input == "3":
                    prelim_latest = False
                else:
                    prelim_latest = False

            elif current_lesson == 2:
                print("\n--------------------------------------------------")
                print("PRELIM - Basic Syntax & Variables")
                print("--------------------------------------------------")
                print("[Explanation]: Managing Data & Code Structure")
                print("• Variables & Assignment:")
                print("  - Containers used to store data values in memory.")
                print("  - Uses the assignment operator: '='")
                print("  - Rules: Case-sensitive; cannot start with numbers.")
                print("  - Example: name = 'John'")
                print("• Output & Indentation:")
                print("  - print() function displays values (e.g., print(name), print(100))")
                print("  - Indentation is mandatory; it defines code blocks.")
                print("  - Example: if age >= 18: print('Adult')")
                print("• Code Comments:")
                print("  - Written using '#' for single-line notes.")

                play = input("\nDo you want to play the mini-game for Lesson 2? (yes/no): ").lower()
                if play in ["yes", "y"]:
                    print("\n--- LESSON 2 MINI-GAME: VARIABLE ASSIGNMENT ---")
                    print("Topic: Storing Data in Variables")
                    print("Task: Assign the value 100 to a variable named score.")
                    print("Code: score ____ 100")
                    user_answer = input("What operator goes in the blank? ")
                    if user_answer == "=":
                        print("GREAT JOB! '=' is the correct answer.")
                    else:
                        print("IT'S OKAY TRY AGAIN. The correct answer is '='.")

                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_input = input("Enter option (1-3): ")

                if next_input == "1":
                    current_lesson = 3
                elif next_input == "2":
                    current_lesson = 5
                elif next_input == "3":
                    prelim_latest = False
                else:
                    prelim_latest = False

            elif current_lesson == 3:
                print("\n--------------------------------------------------")
                print("PRELIM - Python Data Types")
                print("--------------------------------------------------")
                print("[Explanation]: Understanding Variable Types")
                print("• Core Data Types:")
                print("  - Integer (int): Whole numbers (Ex. element = 10)")
                print("  - Floating-point (float): Decimal numbers (Ex.  pi = 3.14)")
                print("  - String (str): Text enclosed in quotes (Ex. msg = 'Hi')")
                print("  - Boolean (bool): True or False values (Ex. is_pass = True)")

                play = input("\nDo you want to play the mini-game for Lesson 3? (yes/no): ").lower()
                if play in ["yes", "y"]:
                    print("\n--- LESSON 3 MINI-GAME: IDENTIFYING STRING TYPE ---")
                    print("Topic: Data Types (str)")
                    print("Task: Fill in the built-in type keyword for text data.")
                    print("Code: my_text = ____('Hello World')")
                    user_answer = input("What data type goes in the blank? ")
                    if user_answer == "str":
                        print("GREAT JOB! 'str' represents the string data type.")
                    else:
                        print("IT'S OKAY TRY AGAIN. The correct answer is 'str'.")

                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_input = input("Enter option (1-3): ")

                if next_input == "1":
                    current_lesson = 4
                elif next_input == "2":
                    current_lesson = 5
                elif next_input == "3":
                    prelim_latest = False
                else:
                    prelim_latest = False

            elif current_lesson == 4:
                print("\n--------------------------------------------------")
                print("PRELIM - Basic Arithmetic Operators")
                print("--------------------------------------------------")
                print("[Explanation]: Performing Calculations")
                print("• Arithmetic Operators Overview:")
                print("  - Addition (+): add two values")
                print("  - Subtraction (-): subtract the second value from the first")
                print("  - Multiplication (*): multiply two values")
                print("  - Division (/): divides two values and returns a decimal")
                print("  - Floor Division (//): divides two values and returns the whole number part")
                print("  - Modulus (%): Returns division remainder")
                print("• Code Examples:")
                print("  - sum_result = 5 + 3")
                print("  - remainder = 10 % 3")

                play = input("\nDo you want to play the mini-game for Lesson 4? (yes/no): ").lower()
                if play in ["yes", "y"]:
                    print("\n--- LESSON 4 MINI-GAME: MODULUS OPERATOR ---")
                    print("Topic: Modulus / Remainder Operator")
                    print("Task: Fill in the missing operator symbol that calculates the division remainder.")
                    print("Code: remainder = 9 ____ 4")
                    user_answer = input("What operator symbol goes in the blank? ")
                    if user_answer == "%":
                        print("GREAT JOB! '%' is the modulus operator.")
                    else:
                        print("IT'S OKAY TRY AGAIN. The modulus operator is '%'.")

                print("\nWhat would you like to do next?")
                print("[1] Take Prelim Quiz")
                print("[2] Back to Main Menu")
                next_input = input("Enter option (1-2): ")

                if next_input == "1":
                    current_lesson = 5
                else:
                    prelim_latest = False

            elif current_lesson == 5:
                print("\n--------------------------------------------------")
                print("PRELIM QUIZ (5 Questions)")
                print("--------------------------------------------------")
                score = 0

                print("\n1. Which function outputs text to the screen in Python?")
                print("a) display()  b) print()  c) ghelo()")
                ans = input("Answer: ").lower()
                if ans == "b":
                    score += 1

                print("\n2. Which of the following is a valid variable name?")
                print("a) 2nd_name  b) ako-ang-bagyo  c) user_name")
                ans = input("Answer: ").lower()
                if ans == "c":
                    score += 1

                print("\n3. What data type is the value 99.5?")
                print("a) int  b) float  c) str")
                ans = input("Answer: ").lower()
                if ans == "b":
                    score += 1

                print("\n4. What is the output of 10 % 3?")
                print("a) 3  b) 0.33  c) 1")
                ans = input("Answer: ").lower()
                if ans == "c":
                    score += 1

                print("\n5. Which symbol is used for single-line comments in Python?")
                print("a) #  b) //  c) /*")
                ans = input("Answer: ").lower()
                if ans == "a":
                    score += 1

                print("\n--------------------------------------------------")
                print(f" QUIZ FINISHED! Your Prelim Score: {score} / 5")
                if score == 5:
                    print("Badge Earned: Syntax Master")
                elif score >= 3:
                    print("Badge Earned: Syntax Sakto lang")
                else:
                    print("Badge Earned: Beginner Learner (Needs Review)")
                print("--------------------------------------------------")

                prelim_score = score
                prelim_taken = True
                prelim_latest = False

    elif term_choice == "2":
        midterm_latest = True
        current_lesson = 1

        while midterm_latest:
            if current_lesson == 1:
                print("\n--------------------------------------------------")
                print("MIDTERM - Conditional Statements (if, elif, else)")
                print("--------------------------------------------------")
                print("[Explanation]: Making Decisions in Code")
                print("• Conditional Decision-Making:")
                print("  - Allows programs to execute code paths based on Boolean states.")
                print("  - if: Evaluates primary condition")
                print("  - elif: Evaluates alternate secondary conditions")
                print("  - else: Catch-all for remaining scenarios")
                print("• Nested Conditions:")
                print("  - An if statement placed inside another outer if block.")
                print("  - Example: checking ID status before verifying age requirements.")

                play = input("\nDo you want to play the mini-game for Lesson 1? (yes/no): ").lower()
                if play in ["yes", "y"]:
                    print("\n--- LESSON 1 MINI-GAME: ALTERNATE CONDITION CHECKING ---")
                    print("Topic: If / Elif / Else Syntax")
                    print("Task: Fill in the keyword used to check an alternate condition.")
                    print("Code:")
                    print("   if score > 90:")
                    print("       print('A')")
                    print("   ____ score > 80:")
                    print("       print('B')")
                    user_answer = input("What keyword goes in the blank? ").lower()
                    if user_answer == "elif":
                        print("GREAT JOB! 'elif' checks secondary conditions.")
                    else:
                        print("IT'S OKAY TRY AGAIN. The keyword is 'elif'.")

                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Midterm Quiz")
                print("[3] Back to Main Menu")
                next_input = input("Enter option (1-3): ")

                if next_input == "1":
                    current_lesson = 2
                elif next_input == "2":
                    current_lesson = 3
                else:
                    midterm_latest = False

            elif current_lesson == 2:
                print("\n--------------------------------------------------")
                print("MIDTERM - Logical Operators")
                print("--------------------------------------------------")
                print("[Explanation]: Combining & Reversing Conditions")
                print("• Logical Operators Toolkit:")
                print("  - 'and': Evaluates to True only if BOTH conditions are True")
                print("  - 'or': Evaluates to True if AT LEAST ONE condition is True")
                print("  - 'not': Reverses the Boolean outcome (True becomes False, etc.)")

                play = input("\nDo you want to play the mini-game for Lesson 2? (yes/no): ").lower()
                if play in ["yes", "y"]:
                    print("\n--- LESSON 2 MINI-GAME: TRUE OR FALSE ---")
                    print("Topic: Logical Operators")
                    print("Task: Fill in the blank.")
                    print("  10 >= 11 ____ 5")
                    user_answer = input("What operator goes in the blank? ").lower()
                    if user_answer == "and":
                        print("GREAT JOB! 'and' is correct.")
                    else:
                        print("IT'S OKAY TRY AGAIN. The correct answer is 'and'.")

                print("\nWhat would you like to do next?")
                print("[1] Take Midterm Quiz")
                print("[2] Back to Main Menu")
                next_input = input("Enter option (1-2): ")

                if next_input == "1":
                    current_lesson = 3
                else:
                    midterm_latest = False

            elif current_lesson == 3:
                print("\n--------------------------------------------------")
                print("MIDTERM QUIZ (5 Questions)")
                print("--------------------------------------------------")
                score = 0

                print("\n1. Which keyword is used to begin a conditional statement?")
                print("a) check  b) if  c) when")
                ans = input("Answer: ").lower()
                if ans == "b":
                    score += 1

                print("\n2. What operator is used for equality comparison in Python?")
                print("a) =  b) ==  c) equals")
                ans = input("Answer: ").lower()
                if ans == "b":
                    score += 1

                print("\n3. When does the else block execute?")
                print("a) Always  b) When previous conditions are True  c) When all previous conditions are False")
                ans = input("Answer: ").lower()
                if ans == "c":
                    score += 1

                print("\n4. What is a nested condition?")
                print("a) Condition inside another condition  b) Condition inside a loop  c) Sanaol Condition")
                ans = input("Answer: ").lower()
                if ans == "a":
                    score += 1

                print("\n5. Which operator means 'Not Equal to'?")
                print("a) !=  b) <>  c) NOT==")
                ans = input("Answer: ").lower()
                if ans == "a":
                    score += 1

                print("\n--------------------------------------------------")
                print(f" QUIZ FINISHED! Your Midterm Score: {score} / 5")
                if score == 5:
                    print("Badge Earned: Logic Master")
                elif score >= 3:
                    print("Badge Earned: Logic Sakto lang")
                else:
                    print("Badge Earned: Beginner Learner (Needs Review)")
                print("--------------------------------------------------")

                midterm_score = score
                midterm_taken = True
                midterm_latest = False

    elif term_choice == "3":
        finals_latest = True
        current_lesson = 1

        while finals_latest:
            if current_lesson == 1:
                print("\n--------------------------------------------------")
                print("FINALS - For Loops & range()")
                print("--------------------------------------------------")
                print("[Explanation]: Iterating Over Sequences")
                print("• For Loop Mechanics:")
                print("  - Iterates sequentially through items in a collection or numeric range.")
                print("  - The range() function automatically generates number sequences.")
                print("• Example Structure:")
                print("  - for iter in range(3): print(iter)")

                play = input("\nDo you want to play the mini-game for Lesson 1? (yes/no): ").lower()
                if play in ["yes", "y"]:
                    print("\n--- LESSON 1 MINI-GAME: SEQUENCE GENERATION ---")
                    print("Topic: For Loop & Range Function")
                    print("Task: Fill in the function used to generate numeric sequences in for loops.")
                    print("Code:")
                    print("   for iter in ____(5):")
                    print("       print(iter)")
                    user_answer = input("What function name goes in the blank? ").lower()
                    if user_answer == "range":
                        print("GREAT JOB! 'range' generates number sequences.")
                    else:
                        print("IT'S OKAY TRY AGAIN. The correct answer is 'range'.")

                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Finals Quiz")
                print("[3] Back to Main Menu")
                next_input = input("Enter option (1-3): ")

                if next_input == "1":
                    current_lesson = 2
                elif next_input == "2":
                    current_lesson = 3
                else:
                    finals_latest = False

            elif current_lesson == 2:
                print("\n--------------------------------------------------")
                print("FINALS - While Loops")
                print("--------------------------------------------------")
                print("[Explanation]: Conditional Repetition")
                print("• While Loop Mechanics:")
                print("  - Repeatedly executes a block of code as long as its condition remains True.")
                print("  - Crucial to update loop control variables to prevent infinite loops.")
                print("• Example Structure:")
                print("  - count = 1")
                print("  - while count <= 3: print(count); count += 1")

                play = input("\nDo you want to play the mini-game for Lesson 2? (yes/no): ").lower()
                if play in ["yes", "y"]:
                    print("\n--- LESSON 2 MINI-GAME: CONDITIONAL LOOP HEADER ---")
                    print("Topic: While Loop Mechanics")
                    print("Task: Fill in the loop keyword that repeats code while a condition is True.")
                    print("Code:")
                    print("   ____ count < 5:")
                    print("       count = count + 1")
                    user_answer = input("What keyword goes in the blank? ").lower()
                    if user_answer == "while":
                        print("GREAT JOB! 'while' creates a conditional loop.")
                    else:
                        print("IT'S OKAY TRY AGAIN. The keyword is 'while'.")

                print("\nWhat would you like to do next?")
                print("[1] Take Finals Quiz")
                print("[2] Back to Main Menu")
                next_input = input("Enter option (1-2): ")

                if next_input == "1":
                    current_lesson = 3
                else:
                    finals_latest = False

            elif current_lesson == 3:
                print("\n--------------------------------------------------")
                print("FINALS QUIZ (5 Questions)")
                print("--------------------------------------------------")
                score = 0

                print("\n1. Which loop runs as long as a condition remains True?")
                print("a) for  b) while  c) repeat")
                ans = input("Answer: ").lower()
                if ans == "b":
                    score += 1

                print("\n2. How many iterations does range(5) produce?")
                print("a) 4  b) 5  c) 6")
                ans = input("Answer: ").lower()
                if ans == "b":
                    score += 1

                print("\n3. What is the starting number generated by range(3) by default?")
                print("a) 0  b) 1  c) 3")
                ans = input("Answer: ").lower()
                if ans == "a":
                    score += 1

                print("\n4. What occurs if a while loop condition never turns False?")
                print("a) Syntax Error  b) Infinite Loop  c) Program Auto-Fix")
                ans = input("Answer: ").lower()
                if ans == "b":
                    score += 1

                print("\n5. Which keyword is used to start a for loop in Python?")
                print("a) for  b) foreach  c) loop")
                ans = input("Answer: ").lower()
                if ans == "a":
                    score += 1

                print("\n--------------------------------------------------")
                print(f" QUIZ FINISHED! Your Finals Score: {score} / 5")
                if score == 5:
                    print("Badge Earned: Loop Master")
                elif score >= 3:
                    print("Badge Earned: Loop Sakto lang")
                else:
                    print("Badge Earned: Loop Beginner (Needs Review)")
                print("--------------------------------------------------")

                finals_score = score
                finals_taken = True
                finals_latest = False

    elif term_choice == "4":
        print("\n================================================")
        print("              STUDENT ACADEMIC SUMMARY            ")
        print("==================================================")
        print(f"Student Name: {student_name}")

        total_quizzes_taken = 0
        total_quiz_score = 0

        if prelim_taken:
            print(f" - Prelim Quiz Score  : {prelim_score} / 5")
            total_quizzes_taken += 1
            total_quiz_score += prelim_score
        else:
            print(" - Prelim Quiz Score  : Not Completed")

        if midterm_taken:
            print(f" - Midterm Quiz Score : {midterm_score} / 5")
            total_quizzes_taken += 1
            total_quiz_score += midterm_score
        else:
            print(" - Midterm Quiz Score : Not Completed")

        if finals_taken:
            print(f" - Finals Quiz Score  : {finals_score} / 5")
            total_quizzes_taken += 1
            total_quiz_score += finals_score
        else:
            print(" - Finals Quiz Score  : Not Completed")

        print("--------------------------------------------------")
        print(f"Total Quizzes Completed: {total_quizzes_taken} / 3")
        print(f"Total Overall Score    : {total_quiz_score} / 15")
        print("--------------------------------------------------")

        print("=================================================")
        if total_quizzes_taken == 3:
            if total_quiz_score == 15:
                print("FINAL GRADE: PERFECT ACADEMIC EXCELLENCE (GALING MO LODS🫶🏻)")
            elif total_quiz_score >= 12:
                print("FINAL GRADE: HIGH HONORS - (GREAT JOB😎)")
            elif total_quiz_score >= 9:
                print("FINAL GRADE: SATISFACTORY - (BASTA PUMASA🫡)")
            else:
                print("FINAL GRADE: NEED MORE REVIEW🙈🙉")
        else:
            print("STATUS :YOU NEED COMPLETE ALL THE 3 TERM QUIZZES!👏🏻")
        print("==================================================")

    elif term_choice == "5":
        print("\n==================================================")
        print(f"Thank you for using my Python Tutorial System🫶🏻, {student_name}!")
        print("    ^.^Keep practicing and happy coding💪🏻!^.^       ")
        print("====================================================")
        count = False

    else:
        print("\n⚠️ Invalid choice! Please select  between 1 and 5 ONLY.")
    
