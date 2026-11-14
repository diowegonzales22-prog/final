while True:

    print("=" * 40)
    print("  FUNDAMENTALS OF PROGRAMMING LESSONS")
    print("=" * 40)

    print("")
    print("Hello sir! welcome to python tutorial system.")
    print("How can I help you today?")

    print("")
    print("What chapter do you want to study?")
    print("[1] Introduction To Programming")
    print("[2] Basic Syntax")
    print("[3] Arithmetic Operators")
    print("[4] Basic Input and Output in Python")
    print("[5] Midterm Lesson 1 - Conditional Statement in Python")
    print("[6] Midterm Lesson 2 - Logical Operator")
    print("[0] Exit")

    try:
        code = int(input("Choose one lesson from number [1-6] and [0] Exit: "))
    except ValueError:
        print("Please Enter Lesson number only!")
        input("Enter anything to continue.....:")
        continue

    if code == 1:
        print("Lesson 1 - Introduction To Programing")
        print("[C] What is Programming Language?")
        print("[O] Who Build Python Programming?")
        print("[D] What is Python Programming?")
        print("[E] Why Learn Python?")
        print("[S] What do you need to start Python Programming?")
        print("[Q] Exit Lesson.")

        while True:
            letter = input("Enter Letter in Lesson 1 and Enter(Q) Exit: ").upper()

            if letter == "C":
                print("-------What is Programming Language?-------")
                print("")
                print("A programming language is a formal set of rules and instructions used to tell a computer what tasks to perform.")
                print("A programming language is a structured system of rules, keywords, and symbols used by humans to write instructions that a computer can understand and execute.")

            elif letter == "O":
                print("-------Who Build Python Programming?------- ")
                print("")
                print("Python is a widely-used programming language that was created by Guido van Rossum in 1991.")
                print("A dutch software engineer best known for creating the Python programming language in 1991.")
                print("He designed Python with the goal of making programming simple, readable, and easy to learn while remaining powerful enough for professional software development.")

            elif letter == "D":
                print("-------What is Python Programming?-------")
                print("")
                print("Here is a short Python script that uses a list and a loop to greet a group of people.")

                names = ["Sir mark", "Sir jom", "Sir jhe"]

                for person in names:
                    print(f"Hello, {person}! Welcome to Python.")

            elif letter == "E":
                print("-------Why Learn Python?-------")
                print("")
                print("1. Simple and easy to learn - Great for beginners.")
                print("2. Readable syntax – Code looks almost like English.")
                print("3. Versatile – Used in many fields (AI,web, automation, games, etc.)")
                print("4. Huge community– Lots of support, tutorials, and libraries.")

            elif letter == "S":
                print("-------What do you need to start Python Programming?-------")
                print("")
                print("Personal computer or Laptop")
                print("")
                dev = input("Do you have Personal Computer or Laptop? (Y)Yes or (N)No: ").upper()

                if dev == "Y":
                    print("Nice!, you're ready to start.")

                if dev == "Y":
                    print("You have the best setup possible to build real-world projects right away.")
                    print("Professional IDES/ Code editor")
                    print("Py charm (by JetBrain)")
                elif dev == "N":
                    print("if (NO) you can still learn and write real Python code right on your smartphone or tablet.")

                    print("Online GDB is online compiler and debugger for C/C++.")
                    print(
                        "You can compile, run and debug code with gdb online. Using gcc/g++ as compiler and gdb as debugger.")
                else:
                    print("Invalid input, enter Y or N only!")



            elif letter == "Q":
                print("Exiting Lesson 1!")
                break

            else:
                print("Invalid letter choice!.")

    elif code == 2:
        print("Lesson 2 - Basic Syntax")
        print("[1] What is Python Syntax?")
        print("[2] Python syntax case sensitive.")
        print("[3] Python syntax Indentation.?")
        print("[4] Python Printing Output.")
        print("[5] Python Comments.")
        print("[6] Variables, constants and data types in Python.")
        print("[7] Basic Data types in Python.")
        print("[0] Exit Lesson.")

        while True:
            try:
                num = int(input("Choose Lesson 2 Number (1-6) and enter (0) to Exit:"))
            except ValueError:

                print("Please enter 1-7 only and 0 To Exit Lesson!")
                input("Enter anything to continue....:")
                continue

            if num == 1:
                print("-------What is Python Syntax?-------")
                print("")
                print("Syntax refers to the set of rules that tells us how to correctly write a program in Python.")
            elif num == 2:
                print("-------Python Case Sensitive-------")
                print("")
                print("Python treats uppercase and lowercase letters differently.")
                print("")
                example = input("Enter (Y) if YES and NO, Would you like example?: ").upper()
                if example == "Y":
                    print("Example correct code:")
                    print('name = "jow"')
                    print("print(name)")
                    print("")
                    print("Example Wrong code:")
                    print('name = "jow"')
                    print("print(Name), Error! Name is not the same as name.")
                elif example == "N":
                    print("Okay! Thank you!")
                else:
                    print("Invalid input! Please enter only 1 or 2.")
            elif num == 3:
                print("-------Python Indentation-------")
                print("")
                print("Unlike other programming languages, Python uses indentation (spaces) to define blocks of code.")
                print("")
                print("Example Correct code:")
                print("age = 24")
                print("if age >= 18:")
                print('    print("adult")')
                print("")
                print("Example Wrong code:")
                print("age = 24")
                print("if age >= 18:")
                print('print("adult"), Not indented!')
            elif num == 4:
                print("-------Python Printing Output-------")
                print("")
                print("print() — The function that display output.")
                print("Example:")
                print('print("Hello, World!")')
                print('print(100)')
                print('print("My age is", 18)')
                print("")
                print("Output:")
                print("       Hello, World!")
                print("       100")
                print("       My age is 18")
            elif num == 5:
                print("-------Python Comments-------")
                print("")
                print("Used hast '#' for single line comment.")
                print('Used triple quotes """ for multi line comment')
                print("Comments are ignored by Python.")
                print("They are used to explain the code.")
                print("")
                print("Example of Python Comments")
                print("# This is a comment")
                print("")
                print('"""')
                print("This is")
                print("a multi line")
                print("comment")
                print('"""')
            elif num == 6:
                print("-------Variables, constants and data types in Python-------")
                print("")
                print("What is Variable?")
                print("A variable is a named storage location used to keep data in a program. The value of a variable can change while the program is running.")
                print("")
                print("Variable Naming Rules:")
                print("A variable can have a short name (like x and y) or a more descriptive name (age, car name, total_volume).")
                print("A variable name must start with a letter or the underscore character.")
                print("Example: age = 20 start with a letter, _value = 100 start with underscore.")
                print("")
                print("A variable name cannot start with a number.")
                print("Example: X 1stValue = 20 start with a number, Why? Python won't know if its a variable or a number!?")
                print("")
                print("Variable names are case-sensitive (age and AGE are two different variables)")
                print("")
                print("Output Variables")
                print("The Python print() function is often used to output variables.")
                print("Example Code:")
                print('exam = "Welcome Python Tutorial!"')
                print("print(exam")
                print("Output: Welcome Python Tutorial!")
                print("")
                print("In the print() function, you output multiple variables, separated by a comma:")
                print("Example Code:")
                print('c = "I"')
                print('p = "Python"')
                print('d = "Coding"')
                print('print(a, b, c)')
                print("Output: I Python Coding")
            elif num == 7:
                print("-------Basic Data Types in Python-------")
                print("")
                print("Data types: are categories that tell Python what kind of data a variable stores. They determine the type of value a variable can hold and what operations can be performed on that value.")
                print("")
                print("Example of Declaration of Variables:")
                print('name = "jow"   #text - string')
                print('age = 24         #whole number - int')
                print('grade = 87.00.   #decimal - float')
                print('is_student = True #True/False boolean')
                print("")
                print("Assigned Value and Output the Value")
                print('print(name)')
                print('print(age)')
                print('print(grade)')
                print('print(is_student)')
            elif num == 0:
                print("Exiting Lesson 2!")
                break
            else:
                print("Invalid input! Choose only in Lesson 2!")


    elif code == 3:
        print("What are Arithmetic Operators?")
        print("Arithmetic operators are symbols used to perform mathematical calculations on numbers. They work the same way as the operators used in everyday mathematics.")
        print("")
        print("Lesson 3 - Arithmetic Operators")
        print("[1] Addition (+)")
        print("[2] Subtraction (-)")
        print("[3] Multiplication (*)")
        print("[4] Division (/)")
        print("[5] Floor Division (//)")
        print("[6) Modulus (%)")
        print("[7] Exponentiation (**)")
        print("[8] Expression in python.")
        print("[0] Exit Lesson.")

        while True:
            try:
                math = int(input("Choose Arithmetic Operators 1-6 and 0 to Exit: "))
            except ValueError:
                print("Enter 1-6 and 0 To Exit Arithmetic Lesson!")
                input("Enter Anything to Continue....: ")
                continue

            if math == 1:
                print("-------Addition (+)-------")
                print("Adds Two values.")
                print("")
                print("Example:")
                print("5 + 5 Result is: 10")

            elif math == 2:
                print("-------Subtraction (-)-------")
                print("Subtracts the second value from the first.")
                print("")
                print("Example:")
                print("7 - 2 Result is: 5")

            elif math == 3:
                print("-------Multiplication (*)-------")
                print("Multiplies two value.")
                print("")
                print("Example:")
                print("5 * 3 Result is: 15")

            elif math == 4:
                print("------- Division (/)-------")
                print("Divides two values and returns a decimal.")
                print("")
                print("Example:")
                print("9 / 4 Result is: 2.25")

            elif math == 5:
                print("-------Floor Division (//)-------")
                print("Divides two values and returns the whole number part.")
                print("")
                print("Example:")
                print("5 // 2 Result is: 2")

            elif math == 6:
                print("-------Modulus (%)-------")
                print("Returns the remainder of the division.")
                print("")
                print("Example:")
                print("5 % 2 Result is: 1")

            elif math == 7:
                print("-------Exponentiation (**)-------")
                print("Raises the first value to the power of the second.")
                print("")
                print("Example:")
                print("5 ** 2 Result is: 25")

            elif math == 8:
                print("-------Expression in Python-------")
                print("")
                print("An expression is a combination of values, variables, and operators that evaluates to a result.")
                print("Python follows the order of operations (PEMDAS).")
                print("")
                print("Example of Expression:")
                print("p = 1")
                print("e = 3")
                print("m = 5")
                print("d = 8")
                print("a = 11")
                print("s = 15")
                print("total = p + e + m + d + a * s")
                print('The Result is:", total')
                print("")
                print("Output is: The Results is: 182, follow (PEMDAS).")

            elif math == 0:
                print("Exiting Arithmetic Lesson!")
                break

            else:
                print("Invalid Choice! Enter only 1-8 and 0 to Exit!")

    elif code == 4:
        print("Lesson 4 - Basic Input and Output in Python")
        print("[1] Accepting User Input")
        print("[2] Formatting Output")
        print("[3] Converting Input to other data types")
        print("[0] Exit")

        while True:
            try:
                basic = int(input("Enter number 1-3 and (0) to Exit: "))
            except ValueError:
                print("Please Enter 1-3 only and 0 To exit!")
                input("Enter Anything to Continue....: ")
                continue
            if basic == 1:
                print("-------Accepting User Input-------")
                print("Purpose of input in programming")
                print("Real-life analogies (e.g., asking for a user's name and responding)")
                print("Example:")
                print('names = input("Enter your name: ")')
                print('ages = int(input("Enter your age: ")')

            elif basic == 2:
                print("-------Formatting Output-------")
                print("Using comma, in print()")
                print("Example:")
                print('names = input("Enter your name: ")')
                print('ages = int(input("Enter your age: ")')
                print('("Name:", names')
                print('(Ages"", ages')

            elif basic == 3:
                print("-------Converting Input to other data types-------")
                print("Float Input(for decimal numbers")
                print("Example code:")
                print('grade = float(input("Enter math grade:")')
                print('(f"Your grade is: {grade}")')
                print("")
                print('Boo leen input ("True or False using condition")')
                print("Example code:")
                print('answer = input("Are you a student?: Yes  ")')
                print('age = int(input("How old are you?: 19 "))')
                print("")
                print('is_student = answer.lower() == "yes"')
                print('is_young = age < 25')
                print("")
                print('("Student:", is_student)')
                print('("Age under 25:", is_young)')
                print("Output: Student: True")
                print("Output: Age under 25: True")
                print("")

            elif basic == 0:
                print("Exiting Lesson 4!")
                break

            else:
                print("Invalid Lesson 4 choice! Choose only 1-3 and 0 to Exit!")

    elif code == 5:
        print("Midterm Lesson 1 - Conditional Statement in Python")
        print("[1] Introduction to Conditional Statement")
        print("[2] Relational Operator")
        print("[3] The if Statement")
        print("[4] The if-else Statement")
        print("[5] The if-elif-else Statement")
        print("[6] Nested Condition")
        print("[0] Exit!")

        while True:
            try:
                condi = int(input("Choose (1-6) Condition Lesson and (0) To exit: "))
            except ValueError:
                print("Enter only 1-6 and 0 To Exit!")
                input("Enter Anything to Continue.....: ")
                continue

            if condi == 1:
                print("-------Introduction to Conditional Statement-------")
                print("A conditional statement allows a program to make decisions based on whether a condition is True or False.")
                print("")
                print("Basic Structure")
                print("if condition:")
                print("statement")
                print("")
                print("Example:")
                print("age = 18:")
                print("if age >= 18:")
                print("You can vote!")
                print("Output: You can Vote!")
                print("")
                print("The program check the condition.")
                print("if True, it does something.")
                print("if False, it does nothing (or something else).")

            elif condi == 2:
                print("-------Relational Operator-------")
                print("Relational operator, also called comparison operators, are used to compare two values. The result is always either True or FalseFalse.")
                print("")
                print("Operator | Meaning                  | Example | Result")
                print("  ==     | Equal to                 |  5 == 5  | True")
                print("  !=     | Not equal                |  5 != 2  | True")
                print("  >      | Greater than             |  10 > 5  | True")
                print("  <      | Less than                |  3 < 1   | False")
                print("  >=     | Greater than or equal to |  5 >= 5  | True")
                print("  <=     | Less than or equal  to   |  4 <= 2  | False")

            elif condi == 3:
                print("-------The if Statement-------")
                print("The if statement execute a block of codes only when a condition is True")
                print("")
                print("Example code:")
                print("age = 24")
                print("if age >= 18:")
                print("You can vote!")

            elif condi == 4:
                print("-------The if-else Statement-------")
                print("The else statement provides an alternative when the if condition is false.")
                print("")
                print("Example code:")
                print("age = 15")
                print("if age >= 18:")
                print("Adult")
                print("else:")
                print("Not an adult yet")
                print("")
                print("Output: Not an adult yet")

            elif condi == 5:
                print("-------The if-elif-else Statement-------")
                print("The  elif  statement is used when there are multiple conditions to evaluate. Python checks each condition from top to bottom and executes the first condition that is True.")
                print("")
                print("Example Code:")
                print("score = 85")
                print("if score >= 90:")
                print("A")
                print("elif score >= 80:")
                print("B")
                print("elif score >= 70:")
                print("C")
                print("else:")
                print("Needs improvement")
                print("")
                print("Output: B")

            elif condi == 6:
                print("-------Nested Condition-------")
                print("A Nested condition is a condition inside another condition.")
                print("")
                print("Example code:")
                print("age = 20")
                print("has_id = True")
                print("if age >= 18:")
                print("   if has_id:")
                print("You may enter")
                print("   else:")
                print("Need your ID")
                print('else:')
                print("Too young")
                print("")
                print("Output: You may enter")

            elif condi == 0:
                print("Exiting Midterm Lesson 1!")
                break

            else:
                print("Invalid Midterm Lesson 1 Choices!")

    elif code == 6:
        print("Midterm Lesson 2 - Logical Operator")
        print("[1] What are Logical Operators?")
        print("[2] The and Operator")
        print("[3] The OR Operator")
        print("[4] The NOT Operator")
        print("[0] Exit Midterm Lesson!")

        while True:
            try:
                operator = int(input("Choose Number on Logical Operator (1-4) and (0) To Exit: "))
            except ValueError:
                print("Enter number only in Logical Operator!")
                input("Enter anything to continue.....: ")
                continue

            if operator == 1:
                print("-------What are Logical Operator-------")
                print("Logical operators are used to combine or reverse conditions in a Python program.")
                print("They are commonly used with  if ,  elif , and  else .")
                print("Python has three logical Operator")
                print("Operator: AND, OR, NOT")

            elif operator == 2:
                print("-------The AND operator-------")
                print("The  and  operator returns True only when ALL conditions are True.")
                print("Truth Table - and")
                print()
                print("|   A   |   B    | A and B |")
                print("| True  | True   | True    |")
                print("| True  | False  | False   |")
                print("| False | True   | False   |")
                print("| False | False  | False   |")
                print()
                a = input("Would you like example code? Enter Y(Yes) or N(NO): ").upper()

                if a == "Y":
                    print("age = 20:")
                    print("has_id = True")
                    print("if age >= 18 and has_id:")
                    print(" You can enter!")
                    print("else:")
                    print("Cannot enter.")
                    print("")
                    print("Output: You can enter!")
                    print("You need to be 18+ and have an ID")
                elif a == "N":
                    print("Okay, Thank you!")

                else:
                    print("Invalid input! Enter only Y or N.")

            elif operator == 3:
                print("===== The OR operator =====")
                print("The  or  operator returns True when at least ONE condition is True.")
                print("Truth Table - or")
                print("")
                print("|   A   |   B    | A and B |")
                print("| True  | True   | True    |")
                print("| True  | False  | True    |")
                print("| False | True   | True    |")
                print("| False | False  | False   |")
                print()
                o = input("Would you like example code? Enter Y(Yes) or N(NO): ").upper()

                if o == "Y":
                    print("is_weekend = True")
                    print("is_holiday = False")
                    print("if is_weekend or is_holiday:")
                    print('    print(No school!")')
                    print("else:")
                    print('    print("Time for school!")')
                    print()
                    print("Output: No school!")
                elif o == "N":
                    print("Okay, Thank you!")

                else:
                    print("Invalid input! Enter only Y or N.")

            elif operator == 4:
                print("-------The NOT operator-------")
                print("The not operator reverse the result of a condition.")
                print("Truth Table - not")
                print()
                print("    Condition   |   Not condition")
                print("  True          |      True      ")
                print("  True          |      False     ")
                print()
                n = input("Would you like example code? Enter Y(Yes) or N(NO): ").upper()

                if n == "Y":
                    print("is_raining = False")
                    print("if not is_raining:")
                    print('    print("Nice weather!")')
                    print("    else:")
                    print('        print("Bring an umbrella.")')
                    print()
                    print("Output: Nice weather!")
                elif n == "N":
                    print("Okay, Thank you!")

                else:
                    print("Invalid input! Enter only Y or N.")

            elif operator == 0:
                print("Exiting midterm Logical Operator!")
                break

            else:
                print("Invalid your input! Choose only in midterm lesson 2!")


    elif code == 0:
        print("Thank you so much for using Python Tutorial!")
        break

    else:
        print("Invalid Choice! Please choose 1-6 only!")
    input("Enter anything to return in Python Tutorial!: ")
