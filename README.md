print("==========================================================")
print("************ PYTHON LEARNING TUTORIAL *************")
print("==========================================================")
print("      Complete Study & Quiz System (Prelim - Finals)      ")
print("==========================================================")

learner_name = "Learner"

while True:
    print("\n==========================================================")
    print(f"WELCOME, {learner_name}!")
    print("----------------------------------------------------------")
    print("MAIN MENU:")
    print("  [1] Prelim Lesson (: Intro, Syntax, Vars, Types, Ops,)")
    print("  [2] Midterm Lesson (Conditionals, Nested If, Relational & Logical Ops)")
    print("  [3] Finals Lesson  (Iteration, for Loop, range(), while & break)")
    print("  [4] Take Final 20-Item Quiz (All Lessons)")
    print("  [5] Exit System")
    print("==========================================================")

    main_menu_choice = input("Choose an option (1-5): ").strip()

    if main_menu_choice == "1":
        prelim_page = 1

        while True:
            if prelim_page == 1:
                print("\n----------------------------------------------------------")
                print("PRELIM - PAGE 1: CHAPTER 1 - INTRODUCTION TO PROGRAMMING")
                print("----------------------------------------------------------")
                print("• Programming Language: A special language that computers")
                print("  understand and use to perform tasks.")
                print("• Common Programming Languages Include:")
                print("  - Python    : Easy to learn and read. Great for beginners,")
                print("                data science, and automation.")
                print("  - C / C++   : High performance and efficient. Used in system")
                print("                programming, games, and applications.")
                print("  - PHP       : Used for web development. Works well with")
                print("                databases and server-side scripting.")
                print("  - Java      : Platform-independent and widely used. Great")
                print("                for apps and systems.")
                print("  - JavaScript: The language of the web. Adds interactivity")
                print("                to websites.")
                print("  - Ruby      : Known for simplicity and productivity. Used in")
                print("                web development.")
                print("• What is Python Programming?")
                print("  - Python is a widely-used programming language that was")
                print("    created by Guido van Rossum in 1991.")
                print("  - A Dutch software engineer best known for creating the")
                print("    Python programming language in 1991.")
                print("  - Designed to make programming simple, readable, and easy")
                print("    to learn while remaining powerful enough for professional")
                print("    software development.")
                print("  - Python is a high-level, interpreted, and general-purpose")
                print("    programming language.")
                print("• Why Learn Python?")
                print("  1. Simple and easy to learn - Great for beginners")
                print("  2. Readable syntax - Code looks almost like English")
                print("  3. Versatile - Used in many fields (AI, web, automation,")
                print("     games, etc.)")
                print("  4. Huge community - Lots of support, tutorials, and")
                print("     libraries")
                print("• What Do You Need to Start Python Programming?")
                print("  - Professional IDEs / Code Editors:")
                print("    PyCharm (by JetBrains), VS Code (Visual Studio Code),")
                print("    Jupyter Notebook/JupyterLab")

                print("\nNext Action:")
                print("  [1] Continue to Page 2 (Syntax, Print & Comments)")
                print("  [2] Return to Main Menu")
                step_p1 = input("Select (1-2): ").strip()

                if step_p1 == "1":
                    prelim_page = 2
                else:
                    break

            elif prelim_page == 2:
                print("\n----------------------------------------------------------")
                print("PRELIM - PAGE 2: CHAPTER 2 - SYNTAX, PRINT & COMMENTS")
                print("----------------------------------------------------------")
                print("• Syntax: Syntax refers to the set of rules that tells us")
                print("  how to correctly write a program in Python.")
                print("• 1. Python is Case-Sensitive:")
                print("  - Python treats uppercase and lowercase letters differently.")
                print("  +--------------------------------------------------------+")
                print("  | CORRECT:                                               |")
                print('  |   1  name = "John"                                     |')
                print("  |   2  print(name)                                       |")
                print("  +--------------------------------------------------------+")
                print("  +--------------------------------------------------------+")
                print("  | INCORRECT:                                             |")
                print('  |   1  name = "John"                                     |')
                print("  |   2  print(Name)  -> Error! Name is not same as name.  |")
                print("  +--------------------------------------------------------+")
                print("• 2. Indentation:")
                print("  - Unlike other programming languages, Python uses")
                print("    indentation (spaces) to define blocks of code.")
                print("  +--------------------------------------------------------+")
                print("  | CORRECT:                                               |")
                print("  |   1  age = 18                                          |")
                print("  |   2                                                    |")
                print("  |   3  if age >= 18:                                     |")
                print('  |   4      print("Adult")                                |')
                print("  +--------------------------------------------------------+")
                print("  +--------------------------------------------------------+")
                print("  | INCORRECT:                                             |")
                print("  |   1  age = 18                                          |")
                print("  |   2                                                    |")
                print("  |   3  if age >= 18:                                     |")
                print('  |   4  print("Adult")                                    |')
                print("  +--------------------------------------------------------+")
                print("• Print Statement:")
                print("  - The print() function displays information on the screen.")
                print("  - Syntax: print(value)")
                print("• Printing Text:")
                print("  - Text (also called a string) must be enclosed in")
                print("    quotation marks.")
                print("  +--------------------------------------------------------+")
                print('  | CORRECT:   1  print("Hello, World!")                   |')
                print("  | INCORRECT: 1  print(Hello, World!)                     |")
                print("  +--------------------------------------------------------+")
                print("• Printing Numbers:")
                print("  - You can print numbers directly without quotation marks.")
                print("  +--------------------------------------------------------+")
                print("  | EXAMPLE:                                               |")
                print("  |   1  print(100)                                        |")
                print("  |   2  print(25.5)                                       |")
                print("  |   print(type(100))   -> <class 'int'>                  |")
                print('  |   print(type("100")) -> <class \'str\'>                  |')
                print("  +--------------------------------------------------------+")
                print("• Python Comments:")
                print("  - Comments are ignored by Python. They are used to")
                print("    explain the code.")
                print("  - Single-Line Comment: Uses the hash symbol #")
                print("  +--------------------------------------------------------+")
                print("  |   1  # This is a comment                               |")
                print("  |   2                                                    |")
                print('  |   3  print("Hello")                                    |')
                print("  +--------------------------------------------------------+")
                print("  - Multi-Line Comment: Uses triple quotes")
                print("  +--------------------------------------------------------+")
                print("  |   1  \"\"\"                                              |")
                print("  |   2  This is                                           |")
                print("  |   3  a multi-line                                      |")
                print("  |   4  comment.                                          |")
                print("  |   5  \"\"\"                                              |")
                print("  |   6                                                    |")
                print('  |   7  print("Hello")                                    |')
                print("  +--------------------------------------------------------+")

                print("\nNext Action:")
                print("  [1] Continue to Page 3 (Variables, Naming Rules & Output)")
                print("  [2] Return to Main Menu")
                step_p2 = input("Select (1-2): ").strip()

                if step_p2 == "1":
                    prelim_page = 3
                else:
                    break

            elif prelim_page == 3:
                print("\n----------------------------------------------------------")
                print("PRELIM - PAGE 3: VARIABLES, NAMING RULES & OUTPUT")
                print("----------------------------------------------------------")
                print("• 1. What is a Variable?")
                print("  - A variable is a named storage location used to keep")
                print("    data in a program. The value of a variable can change")
                print("    while the program is running.")
                print("  - Example: a, b, c, age, name")
                print("• Assigned Value to Variable:")
                print("  - We assign a value to a variable using the = (assignment")
                print("    operator).")
                print("  +--------------------------------------------------------+")
                print('  | EXAMPLE: first_name = "John"                           |')
                print("  +--------------------------------------------------------+")
                print("• Variable Naming Rules:")
                print("  - Short names (x, y) or descriptive names (age, carname,")
                print("    total_volume, student_score).")
                print("  - Must start with a letter or the underscore character (_).")
                print("  - Cannot start with a number.")
                print("  - GOOD: number, NUMBER, bread, spam23, _speed")
                print("  - BAD : 1number, 1stValue, 2total, 123name, #bread,")
                print("          var.12, space name, @value")
                print("  - Case-sensitive: age and AGE are two different variables.")
                print("    age = 18  !=  AGE = 25")
                print("• Output Variables:")
                print("  +--------------------------------------------------------+")
                print("  | SINGLE VARIABLE:                                       |")
                print('  |   1  school = "Clark College"                          |')
                print("  |   2  print(school)                                     |")
                print("  +--------------------------------------------------------+")
                print("  +--------------------------------------------------------+")
                print("  | MULTIPLE VARIABLES SEPARATED BY COMMA (,):             |")
                print('  |   1  a = "I"                                           |')
                print('  |   2  b = "LOVE"                                        |')
                print('  |   3  c = "CCST"                                        |')
                print("  |   4  #print multiple variables                         |")
                print("  |   5  print(a, b, c)  -> I LOVE CCST                    |")
                print("  +--------------------------------------------------------+")
                print("  +--------------------------------------------------------+")
                print("  | MULTIPLE VARIABLES SEPARATED BY PLUS (+):              |")
                print('  |   1  x = "I "                                          |')
                print('  |   2  y = "LOVE "                                       |')
                print('  |   3  z = "CCST"                                        |')
                print("  |   4  #Add the variables                                |")
                print("  |   5  print(x + y + z)  -> I LOVE CCST                  |")
                print("  +--------------------------------------------------------+")

                print("\nNext Action:")
                print("  [1] Continue to Page 4 (Basic Data Types)")
                print("  [2] Return to Main Menu")
                step_p3 = input("Select (1-2): ").strip()

                if step_p3 == "1":
                    prelim_page = 4
                else:
                    break

            elif prelim_page == 4:
                print("\n----------------------------------------------------------")
                print("PRELIM - PAGE 4: BASIC DATA TYPES IN PYTHON")
                print("----------------------------------------------------------")
                print("• Data Types:")
                print("  - Data types are categories that tell Python what kind")
                print("    of data a variable stores. They determine the type")
                print("    of value a variable can hold and what operations can")
                print("    be performed on that value.")
                print("• Core Data Types:")
                print("  - int  (Integer numbers): Whole numbers (no decimal part).")
                print("    Examples: 10, 25, -7, 100")
                print("  - float (Decimal numbers): Numbers with a decimal point.")
                print("    Examples: 12.5, 3.14, -0.001, 2.0")
                print("  - str  (String or text): Text or characters inside quotes.")
                print('    Examples: "Hello", "Juan", "CCST"')
                print("  - bool (Boolean values): Represents one of two values:")
                print("    True or False. Examples: True, False")
                print("• Declaration of Variables & Output:")
                print("  +--------------------------------------------------------+")
                print('  |   1  name = "Maria"                                    |')
                print("  |   2  age = 20                                          |")
                print("  |   3  grade = 89.5                                      |")
                print("  |   4  is_enrolled = True                                |")
                print("  |   5  print(name)                                       |")
                print("  |   6  print(age)                                        |")
                print("  |   7  print(grade)                                      |")
                print("  |   8  print(is_enrolled)                                |")
                print("  +--------------------------------------------------------+")

                print("\nNext Action:")
                print("  [1] Continue to Page 5 (Ch. 3 Operators/PEMDAS & Ch. 4 Input/Output)")
                print("  [2] Return to Main Menu")
                step_p4 = input("Select (1-2): ").strip()

                if step_p4 == "1":
                    prelim_page = 5
                else:
                    break

            elif prelim_page == 5:
                print("\n----------------------------------------------------------")
                print("PRELIM - PAGE 5: CH. 3 OPERATORS/PEMDAS & CH. 4 INPUT/OUTPUT")
                print("----------------------------------------------------------")
                print("• What Are Arithmetic Operators?")
                print("  - Arithmetic operators are symbols used to perform")
                print("    mathematical calculations on numbers.")
                print("• Python Arithmetic Operators:")
                print("  - +  : Addition        | 5 + 3   -> 8")
                print("  - -  : Subtraction     | 10 - 4  -> 6")
                print("  - *  : Multiplication  | 7 * 2   -> 14")
                print("  - /  : Division(float) | 15 / 3  -> 5.0")
                print("  - // : Floor Division  | 17 // 3 -> 5")
                print("  - %  : Modulus         | 10 % 3  -> 1")
                print("  - ** : Exponentiation  | 2 ** 3  -> 8")
                print("• Expressions in Python:")
                print("  - An expression is a combination of values, variables,")
                print("    and operators that evaluates to a result.")
                print("  +--------------------------------------------------------+")
                print("  | EXAMPLE (ADD TWO NUMBERS):                             |")
                print("  |   1  a = 10                                            |")
                print("  |   2  b = 5                                             |")
                print("  |   3                                                    |")
                print("  |   4  result = a + b                                    |")
                print('  |   5  print("The result is:", result)  -> Result: 15    |')
                print("  +--------------------------------------------------------+")
                print("  - PEMDAS (Order of Operations):")
                print("    P Parentheses (First) -> E Exponents -> M Multiplication ->")
                print("    D Division -> A Addition -> S Subtraction (Last)")
                print("• Accepting User Input (Chapter 4):")
                print("  - Syntax: variable = input(\"Prompt message: \")")
                print("  - All input is string type by default.")
                print("  +--------------------------------------------------------+")
                print("  | EXAMPLE (INPUT & FORMATTING OUTPUT WITH COMMA):        |")
                print('  |   1  name = input("Enter your name: ")                 |')
                print('  |   2  age = input("Enter your age: ")                   |')
                print('  |   3  print("Name: ", name)                             |')
                print('  |   4  print("Age: ", age)                               |')
                print("  +--------------------------------------------------------+")
                print("• Converting Input to Other Data Types:")
                print("  +--------------------------------------------------------+")
                print('  |   age = int(input("Enter your age: "))                 |')
                print('  |   grade = float(input("Enter your grade: "))           |')
                print('  |   answer = input("Are you a student? (yes/no): ")    |')
                print('  |   is_student = answer.lower() == "yes"               |')
                print('  |   print("Student status:", is_student)               |')
                print("  +--------------------------------------------------------+")

                print("\n==========================================================")
                print("YOU HAVE FINISHED THE PRELIM MODULE!")
                print("==========================================================")
                print("  [1] Return to Main Menu (then choose Midterm or Quiz)")
                input("Press Enter to return to Main Menu...")
                break

    elif main_menu_choice == "2":
        midterm_page = 1

        while True:
            if midterm_page == 1:
                print("\n----------------------------------------------------------")
                print("MIDTERM - PAGE 1: CONDITIONALS & RELATIONAL OPERATORS")
                print("----------------------------------------------------------")
                print("• 2. Introduction to Conditional Statements:")
                print("  - A conditional statement allows a program to make")
                print("    decisions based on whether a condition is True or False.")
                print("• 3. Relational Operators:")
                print("  - Relational operators, also called comparison operators,")
                print("    are used to compare two values. The result is always")
                print("    either True or False.")
                print("  - == : Equal to                 | 10 == 10 -> True")
                print("  - != : Not equal to             | 10 != 5  -> True")
                print("  - >  : Greater than             | 10 > 5   -> True")
                print("  - <  : Less than                | 5 < 10   -> True")
                print("  - >= : Greater than or equal to | 10 >= 10 -> True")
                print("  - <= : Less than or equal to    | 5 <= 10  -> True")
                print("  +--------------------------------------------------------+")
                print("  | EXAMPLE:                                               |")
                print("  |   1  score = 85                                        |")
                print("  |   2                                                    |")
                print("  |   3  print(score >= 75)  -> True                       |")
                print("  +--------------------------------------------------------+")
                print("• 4. The if Statement:")
                print("  - Executes a block of code only when a condition is true.")
                print("  - Syntax:")
                print("    if condition:")
                print("        statement(s)")
                print("  +--------------------------------------------------------+")
                print("  | EXAMPLE:                                               |")
                print("  |   age = 20                                             |")
                print("  |   if age >= 18:                                        |")
                print('  |       print("You are an adult.")                       |')
                print("  +--------------------------------------------------------+")
                print("• 5. The if-else Statement:")
                print("  - The else statement provides an alternative when the")
                print("    if condition is false.")
                print("  +--------------------------------------------------------+")
                print("  | EXAMPLE:                                               |")
                print("  |   score = 65                                           |")
                print("  |   if score >= 75:                                      |")
                print('  |       print("Passed")                                  |')
                print("  |   else:                                                |")
                print('  |       print("Failed")  -> Failed                       |')
                print("  +--------------------------------------------------------+")
                print("• 6. The if-elif-else Statement:")
                print("  - The elif statement is used when there are multiple")
                print("    conditions to evaluate. Python checks each condition")
                print("    from top to bottom and executes the first condition")
                print("    that is True.")
                print("  +--------------------------------------------------------+")
                print("  | EXAMPLE:                                               |")
                print("  |   1  score = 85                                        |")
                print("  |   2                                                    |")
                print("  |   3  if score >= 90:                                   |")
                print('  |   4      print("Excellent")                              |')
                print("  |   5  elif score >= 80:                                 |")
                print('  |   6      print("Very Good")  -> Very Good              |')
                print("  |   7  elif score >= 75:                                 |")
                print('  |   8      print("Passed")                                 |')
                print("  |   9  else:                                             |")
                print('  |   10     print("Failed")                                 |')
                print("  +--------------------------------------------------------+")

                print("\nNext Action:")
                print("  [1] Continue to Page 2 (Nested Condition in Python)")
                print("  [2] Return to Main Menu")
                step_m1 = input("Select (1-2): ").strip()

                if step_m1 == "1":
                    midterm_page = 2
                else:
                    break

            elif midterm_page == 2:
                print("\n----------------------------------------------------------")
                print("MIDTERM - PAGE 2: NESTED CONDITION IN PYTHON")
                print("----------------------------------------------------------")
                print("• Nested Condition in Python:")
                print("  - A nested condition is a condition inside another")
                print("    condition.")
                print("  - TIP: Read the flow from the top. The inner condition")
                print("    (age) is checked only if the outer condition (gender)")
                print("    is True.")
                print("• Syntax:")
                print("  if condition1:")
                print("      if condition2:")
                print("          block of code")
                print("      else:")
                print("          block of code")
                print("  else:")
                print("      block of code")
                print("• Debutant Age Rules by Gender Example:")
                print("  +--------------------------------------------------------+")
                print('  |   gender = input("Enter gender (M/F): ")               |')
                print('  |   age = int(input("Enter age: "))                      |')
                print("  |   if gender == 'M':                                    |")
                print("  |       if age >= 21:                                     |")
                print('  |           print("You are a MALE DEBUTANT.")            |')
                print("  |       else:                                            |")
                print('  |           print("You are a male, but not debutant yet.")|')
                print("  |   else:                                                |")
                print("  |       if age >= 18:                                     |")
                print('  |           print("You are a FEMALE DEBUTANT.")          |')
                print("  |       else:                                            |")
                print('  |           print("You are a female, not debutant yet.") |')
                print("  +--------------------------------------------------------+")

                print("\nNext Action:")
                print("  [1] Continue to Page 3 (Logical Operators & Truth Tables)")
                print("  [2] Return to Main Menu")
                step_m2 = input("Select (1-2): ").strip()

                if step_m2 == "1":
                    midterm_page = 3
                else:
                    break

            elif midterm_page == 3:
                print("\n----------------------------------------------------------")
                print("MIDTERM - PAGE 3: LOGICAL OPERATORS & TRUTH TABLES")
                print("----------------------------------------------------------")
                print("• What Are Logical Operators?")
                print("  - Logical operators are used to combine or reverse")
                print("    conditions in a Python program. They are commonly")
                print("    used with if, elif, and else.")
                print("• The and Operator (AND = KAILANGAN LAHAT TRUE):")
                print("  - Returns True only when ALL conditions are True.")
                print("  - Truth Table: True & True = True | True & False = False")
                print("                 False & True = False | False & False = False")
                print("  +--------------------------------------------------------+")
                print("  | EXAMPLE:                                               |")
                print("  |   age = 20                                             |")
                print("  |   has_id = True                                        |")
                print("  |   if age >= 18 and has_id:                            |")
                print('  |       print("You are allowed to enter.")               |')
                print("  |   else:                                                |")
                print('  |       print("You are not allowed to enter.")           |')
                print("  +--------------------------------------------------------+")
                print("• The or Operator (OR = KAHIT ISA LANG TRUE):")
                print("  - Returns True when at least ONE condition is True.")
                print("  - Truth Table: True | True = True | True | False = True")
                print("                 False | True = True | False | False = False")
                print("  +--------------------------------------------------------+")
                print("  | EXAMPLE:                                               |")
                print('  |   day = "Saturday"                                     |')
                print('  |   if day == "Saturday" or day == "Sunday":             |')
                print('  |       print("It\'s the weekend!")                       |')
                print("  |   else:                                                |")
                print('  |       print("It\'s a regular school day.")               |')
                print("  +--------------------------------------------------------+")
                print("• The not Operator (NOT = BALIKTARIN ANG RESULT):")
                print("  - Reverses the result of a condition.")
                print("  - True -> False | False -> True")
                print("  +--------------------------------------------------------+")
                print("  | EXAMPLE:                                               |")
                print("  |   is_raining = False                                   |")
                print("  |   if not is_raining:                                   |")
                print('  |       print("You can go outside.")                     |')
                print("  |   else:                                                |")
                print('  |       print("Bring an umbrella.")                      |')
                print("  +--------------------------------------------------------+")

                print("\n==========================================================")
                print("YOU HAVE FINISHED THE MIDTERM MODULE!")
                print("==========================================================")
                input("Press Enter to return to Main Menu...")
                break

    elif main_menu_choice == "3":
        finals_page = 1

        while True:
            if finals_page == 1:
                print("\n----------------------------------------------------------")
                print("FINALS - PAGE 1: ITERATION & PYTHON FOR LOOP")
                print("----------------------------------------------------------")
                print("• Introduction to Iteration:")
                print("  - Iteration means repeating a process. In programming,")
                print("    it means repeatedly executing a set of instructions.")
                print("    Each repetition is called an iteration.")
                print("  - Iteration allows a program to perform the same task")
                print("    multiple times. Loops make the program shorter and")
                print("    easier to modify.")
                print("• Types of Loops in Python:")
                print("  - for loop: Repeats instructions for each item in a")
                print("    sequence. Useful when the number of repetitions is")
                print("    known.")
                print("  - while loop: Repeats instructions while a condition is")
                print("    True. Useful when repetition depends on a condition.")
                print("• Python for Loop Syntax:")
                print("  for variable in sequence:")
                print("      statement(s)")
                print("• Examples:")
                print("  +--------------------------------------------------------+")
                print("  |   for number in range(3):                              |")
                print('  |       print("Welcome to Python!")                      |')
                print("  +--------------------------------------------------------+")
                print("  +--------------------------------------------------------+")
                print("  | FOR LOOP: PRINT NUMBERS 1 TO 5:                        |")
                print("  |   for number in range(1, 6):                           |")
                print("  |       print(number)                                    |")
                print("  |   (Start value 1 is included; stop 6 is excluded)      |")
                print("  +--------------------------------------------------------+")
                print("  +--------------------------------------------------------+")
                print("  | COUNTING DOWNWARD WITH RANGE(): 5 TO 1:                |")
                print("  |   for number in range(5, 0, -1):                       |")
                print("  |       print(number)                                    |")
                print("  |   (Start 5, stop before 0, step -1 decreases by 1)     |")
                print("  +--------------------------------------------------------+")

                print("\nNext Action:")
                print("  [1] Continue to Page 2 (while Loop & while True)")
                print("  [2] Return to Main Menu")
                step_f1 = input("Select (1-2): ").strip()

                if step_f1 == "1":
                    finals_page = 2
                else:
                    break

            elif finals_page == 2:
                print("\n----------------------------------------------------------")
                print("FINALS - PAGE 2: WHILE LOOP & WHILE TRUE")
                print("----------------------------------------------------------")
                print("• Python while Loop Syntax:")
                print("  while condition:")
                print("      statement(s)")
                print("  +--------------------------------------------------------+")
                print("  | EXAMPLE CODE:                                          |")
                print("  |   count = 1                                            |")
                print("  |   while count <= 5:                                    |")
                print("  |       print(count)                                     |")
                print("  |       count += 1                                       |")
                print("  |   (When count becomes 6, condition is False & stops)   |")
                print("  +--------------------------------------------------------+")
                print("• Repeating a Program with while True:")
                print("  +--------------------------------------------------------+")
                print("  |   while True:                                          |")
                print('  |       name = input("Enter your name (X to exit): ")    |')
                print('  |       if name.upper() == "X":                          |')
                print('  |           print("Program stopped.")                    |')
                print("  |           break                                        |")
                print('  |       print("Hello,", name)                            |')
                print("  +--------------------------------------------------------+")

                print("\n==========================================================")
                print("YOU HAVE FINISHED ALL LESSONS (PRELIM, MIDTERM & FINALS)!")
                print("==========================================================")
                input("Press Enter to return to Main Menu...")
                break

    elif main_menu_choice == "4":
        print("\n==========================================================")
        print("      COMPREHENSIVE PYTHON QUIZ (20 ITEMS - ALL LESSONS)  ")
        print("==========================================================")
        print("Instructions: Type the letter of your choice (a, b, or c).")
        print("----------------------------------------------------------")

        quiz_score = 0

        print("\n1. Who created the Python programming language in 1991?")
        print("   a) James Gosling   b) Guido van Rossum   c) Bjarne Stroustrup")
        if input("   Answer: ").strip().lower() == "b":
            quiz_score += 1

        print("\n2. Which programming language is described as 'The language of the web; adds interactivity to websites'?")
        print("   a) JavaScript   b) C++   c) Ruby")
        if input("   Answer: ").strip().lower() == "a":
            quiz_score += 1

        print("\n3. Why does print(Name) cause an error if the variable was created as name = \"John\"?")
        print("   a) Missing quotes   b) Python is case-sensitive   c) Wrong indentation")
        if input("   Answer: ").strip().lower() == "b":
            quiz_score += 1

        print("\n4. Which symbol is used to start a single-line comment in Python?")
        print("   a) //   b) /*   c) #")
        if input("   Answer: ").strip().lower() == "c":
            quiz_score += 1

        print("\n5. Which of the following is a VALID variable name in Python?")
        print("   a) 1stValue   b) _speed   c) space name")
        if input("   Answer: ").strip().lower() == "b":
            quiz_score += 1

        print("\n6. What is the data type of the value 89.5?")
        print("   a) int   b) str   c) float")
        if input("   Answer: ").strip().lower() == "c":
            quiz_score += 1

        print("\n7. What is the result of the floor division expression 17 // 3?")
        print("   a) 5   b) 5.66   c) 2")
        if input("   Answer: ").strip().lower() == "a":
            quiz_score += 1

        print("\n8. According to PEMDAS, which operation is evaluated FIRST in Python?")
        print("   a) Multiplication   b) Addition   c) Parentheses")
        if input("   Answer: ").strip().lower() == "c":
            quiz_score += 1

        print("\n9. What type of value do relational operators (==, !=, >, <, >=, <=) always return?")
        print("   a) Integer   b) String   c) True or False")
        if input("   Answer: ").strip().lower() == "c":
            quiz_score += 1

        print("\n10. In an if-elif-else structure, what happens if multiple conditions are True?")
        print("   a) Only the FIRST True block runs   b) All True blocks run   c) The else block runs")
        if input("   Answer: ").strip().lower() == "a":
            quiz_score += 1

        print("\n11. When is the inner condition inside a nested 'if' statement checked?")
        print("   a) Always   b) Only if the outer condition is True   c) Only if the outer condition is False")
        if input("   Answer: ").strip().lower() == "b":
            quiz_score += 1

        print("\n12. Which logical operator returns True ONLY when ALL conditions are True?")
        print("   a) or   b) not   c) and")
        if input("   Answer: ").strip().lower() == "c":
            quiz_score += 1

        print("\n13. What is the result of: True or False?")
        print("   a) True   b) False   c) None")
        if input("   Answer: ").strip().lower() == "a":
            quiz_score += 1

        print("\n14. If is_raining = False, what does 'not is_raining' evaluate to?")
        print("   a) False   b) True   c) Error")
        if input("   Answer: ").strip().lower() == "b":
            quiz_score += 1

        print("\n15. In programming, what is each single repetition of a loop called?")
        print("   a) iteration   b) indentation   c) concatenation")
        if input("   Answer: ").strip().lower() == "a":
            quiz_score += 1

        print("\n16. Which loop is best used when the number of repetitions is already known?")
        print("   a) while loop   b) for loop   c) if-else")
        if input("   Answer: ").strip().lower() == "b":
            quiz_score += 1

        print("\n17. What numbers are printed by: for number in range(1, 6): print(number)?")
        print("   a) 1, 2, 3, 4, 5, 6   b) 0, 1, 2, 3, 4, 5   c) 1, 2, 3, 4, 5")
        if input("   Answer: ").strip().lower() == "c":
            quiz_score += 1

        print("\n18. What is the first number printed by: for number in range(5, 0, -1)?")
        print("   a) 5   b) 0   c) -1")
        if input("   Answer: ").strip().lower() == "a":
            quiz_score += 1

        print("\n19. In a while loop with 'count = 1' and 'while count <= 5:', at what value of count does the loop stop?")
        print("   a) 5   b) 6   c) 0")
        if input("   Answer: ").strip().lower() == "b":
            quiz_score += 1

        print("\n20. Which keyword is used to immediately stop a 'while True' loop when the user enters 'X'?")
        print("   a) stop   b) exit   c) break")
        if input("   Answer: ").strip().lower() == "c":
            quiz_score += 1

        print("\n==========================================================")
        print(f"QUIZ COMPLETED! {learner_name}, your score is: {quiz_score} / 20")
        if quiz_score == 20:
            print("REMARKS: PERFECT SCORE!")
        elif quiz_score >= 15:
            print("REMARKS: PASSED WITH HONORS!")
        elif quiz_score >= 12:
            print("REMARKS: PASSED! .")
        else:
            print("REMARKS: NEEDS REVIEW. Go back to the modules and try again!")
        print("==========================================================")

    elif main_menu_choice == "5":
        print("\n==========================================================")
        print(f"Thank you for studying, {learner_name}! Happy coding!")
        print("==========================================================")
        break

    else:
        print("\nInvalid choice! Please select an option from 1 to 5.")
    
