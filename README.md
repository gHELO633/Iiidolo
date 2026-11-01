

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



# Python Learning System (Prelim, Midterm, Final)
# Strict Constraint: Uses only loops, if/elif/else, and nested conditions.

running = 1

while running == 1:
    print("\n========================================")
    print("   PYTHON PROGRAMMING LEARNING SYSTEM   ")
    print("========================================")
    print("[1] Prelim Section")
    print("[2] Midterm Section")
    print("[3] Final Section")
    print("[4] Exit Program")
    
    choice = input("Select a section (1-4): ")
    
    # ---------------------------------------------------------
    # PRELIM SECTION
    # ---------------------------------------------------------
    if choice == "1":
        print("\n----------------------------------------")
        print("           PRELIM SECTION               ")
        print("----------------------------------------")
        print("Lessons:")
        print("1. Intro to Python & Variables")
        print("2. Basic Output & Input")
        print("3. Basic Arithmetic Operators")
        print("4. Introduction to Conditions (if)")
        print("5. Two-Way Selection (if-else)")
        
        print("\n--- Very Short Tutorials ---")
        print("Lesson 1: Variables are containers that store data values using '='.")
        print("Lesson 2: print() shows text on screen, input() gets text from the user.")
        print("Lesson 3: Basic math uses +, -, *, and /.")
        print("Lesson 4: An 'if' statement runs code only when a condition is true.")
        print("Lesson 5: An 'else' block provides an alternative if the condition is false.")
        
        print("\n--- Prelim Quiz (5 Questions) ---")
        print("Note: Type your exact short answer in lowercase.")
        score = 0
        
        q1 = input("Q1: What symbol is used to assign a value to a variable? ")
        if q1 == "=":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is '='.")
            
        q2 = input("Q2: Which function displays text to the screen? ")
        if q2 == "print":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is 'print'.")
            
        q3 = input("Q3: What is the result of 10 + 5 * 2? ")
        if q3 == "20":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is 20.")
            
        q4 = input("Q4: Which keyword executes code when a condition is true? ")
        if q4 == "if":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is 'if'.")
            
        q5 = input("Q5: What block runs when an 'if' condition is false? ")
        if q5 == "else":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is 'else'.")
            
        print("Your Total Prelim Score:", score, "/ 5")

    # ---------------------------------------------------------
    # MIDTERM SECTION
    # ---------------------------------------------------------
    elif choice == "2":
        print("\n----------------------------------------")
        print("           MIDTERM SECTION              ")
        print("----------------------------------------")
        print("Lessons:")
        print("1. Nested if Conditions")
        print("2. Multiple Selection (elif)")
        print("3. Introduction to while Loops")
        print("4. Introduction to for Loops")
        print("5. Loop Control (break statement)")
        
        print("\n--- Very Short Tutorials ---")
        print("Lesson 1: A nested condition is an 'if' statement placed inside another 'if'.")
        print("Lesson 2: 'elif' allows checking multiple sequential alternative conditions.")
        print("Lesson 3: A 'while' loop repeats code as long as its condition is true.")
        print("Lesson 4: A 'for' loop repeats over a fixed range or sequence.")
        print("Lesson 5: The 'break' statement stops and exits a loop immediately.")
        
        print("\n--- Midterm Quiz (5 Questions) ---")
        score = 0
        
        q1 = input("Q1: What is an 'if' statement placed inside another 'if' called? ")
        if q1 == "nested":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is 'nested'.")
            
        q2 = input("Q2: Which keyword checks an alternative condition after 'if'? ")
        if q2 == "elif":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is 'elif'.")
            
        q3 = input("Q3: Which loop repeats while its condition is true? ")
        if q3 == "while":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is 'while'.")
            
        q4 = input("Q4: Which loop type is used for a fixed set of repetitions? ")
        if q4 == "for":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is 'for'.")
            
        q5 = input("Q5: Which statement terminates a loop immediately? ")
        if q5 == "break":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is 'break'.")
            
        print("Your Total Midterm Score:", score, "/ 5")

    # ---------------------------------------------------------
    # FINAL SECTION
    # ---------------------------------------------------------
    elif choice == "3":
        print("\n----------------------------------------")
        print("           FINAL SECTION                ")
        print("----------------------------------------")
        print("Lessons:")
        print("1. Advanced Nested Conditions")
        print("2. Loop Accumulators and Counters")
        print("3. Validating Choice with Loops")
        print("4. Nested Loops")
        print("5. Interactive Console Menus")
        
        print("\n--- Very Short Tutorials ---")
        print("Lesson 1: Combining complex decision trees using multiple levels of nesting.")
        print("Lesson 2: Counters track frequency; accumulators keep running totals.")
        print("Lesson 3: Using loops to re-prompt users until valid inputs are provided.")
        print("Lesson 4: Placing a loop inside another loop to handle grid or matrix data.")
        print("Lesson 5: Bringing together loops and conditions to build full applications.")
        
        print("\n--- Final Quiz (5 Questions) ---")
        score = 0
        
        q1 = input("Q1: What is created when an entire loop is inside another loop? ")
        if q1 == "nested loop":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is 'nested loop'.")
            
        q2 = input("Q2: What is a variable used inside a loop to keep a running total called? ")
        if q2 == "accumulator":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is 'accumulator'.")
            
        q3 = input("Q3: Which loop structure is best for input validation re-prompting? ")
        if q3 == "while loop":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is 'while loop'.")
            
        q4 = input("Q4: In a nested loop, which loop finishes all its iterations faster? ")
        if q4 == "inner loop":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is 'inner loop'.")
            
        q5 = input("Q5: What control structures are combined to build interactive text menus? ")
        if q5 == "loops and conditions":
            print("Correct!")
            score = score + 1
        else:
            print("Incorrect. The answer is 'loops and conditions'.")
            
        print("Your Total Final Score:", score, "/ 5")

    # ---------------------------------------------------------
    # EXIT PROGRAM
    # ---------------------------------------------------------
    elif choice == "4":
        print("Exiting program. Good luck with your studies!")
        running = 0
    
    # ---------------------------------------------------------
    # INVALID INPUT
    # ---------------------------------------------------------
    else:
        print("Invalid choice. Please enter a number from 1 to 4.")
