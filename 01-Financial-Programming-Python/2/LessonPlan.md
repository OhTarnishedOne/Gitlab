# Module 1: Virtual Class II Lesson Plan (2 hours)

## Overview

The goal of this class is to introduce students to Python's conditional statements, functions, and loops. These will all be viewed through the lens of program automation.

In addition, the students should be shown how to create and upload a folder to GitHub, as this skill will be necessary to submit their Challenge assignment.

## Learning Objectives

At the end of the session, learners will be able to do the following:

* Articulate how conditional statements are used to make decisions in a program.

* Define and call a Python function.

* Explain the purpose of a Python loop and iterate over an iterable object.

* Iterate over a Python list using a `for` loop.

* Describe how these elements combine to help automate a program.

* Create a new repository in GitHub and manually upload a folder to the GitHub GUI.

---

## Time Tracker

| Start   | #  | Activity                                           | Time |
| ------- | -- | -------------------------------------------------- | ---- |
| 6:50 PM |    | *Optional:* Pre-Class Warm-Up Activities           | 0:10 |
| 7:00 PM | 1  | Instructor Do: Temperature Check                   | 0:05 |
| 7:05 PM | 2  | Instructor Do: Conditional Statements              | 0:10 |
| 7:15 PM | 3  | Student Do: Conditional Conundrum                  | 0:10 |
| 7:25 PM | 4  | Instructor Do: Review Conditional Conundrum        | 0:10 |
| 7:35 PM | 5  | Instructor Do: Python Functions                    | 0:10 |
| 7:45 PM | 6  | Student Do: Functions                              | 0:10 |
| 7:55 PM | 7  | Instructor Do: Review Functions                    | 0:10 |
| 8:05 PM | 8  | Break                                              | 0:05 |
| 8:10 PM | 9  | Instructor Do: for Loops                           | 0:15 |
| 8:25 PM | 10 | Student Do: Loop-De-Loop                           | 0:15 |
| 8:40 PM | 11 | Instructor Do: Review Loop-De-Loop                 | 0:10 |
| 8:50 PM | 12 | Instructor Do: GitHub                              | 0:10 |
| 9:00 PM |    | END                                                |      |

---

## Instructor Do: Office Hours (0:30)

Welcome to Office Hours! Remind the students that this is their time to ask questions and get assistance from their instructional staff as they’re learning new concepts and working on the challenge assignment. Feel free to use breakout rooms to create spaces focused on specific topics, or to have 1:1s with students.
Expect that students may ask for assistance such as the following:

* Challenge assignment
* Further review on a particular subject
* Debugging assistance
* Help with computer issues
* Guidance with a particular tool

---

## Class Activities

### Optional Warm-Up Activities: Variables, Terminal/GitBash, Conditional Statements

The first three activities of today's class are **completely optional**. If students show up early looking for a challenge, send these activities to them on Slack. Alternatively, you can send out the activities on Slack in the afternoon as an optional pre-class preparation activity.

Students having issues running Python script files in Terminal or GitBash should be prioritized at this point. Ask TAs to work one-on-one with students to ensure that they can access Python files in Visual Studio and run them in Terminal or GitBash.

* Explain to students that for the first section of class, they’ll do some warm-up activities to review Python variables and conditional statements. This is an opportunity to get into the groove with these fundamental Python concepts before getting into more complex material.

* Remind students that they’ll need to open the file in VS Code to work with the code, but then navigate to the file in either Terminal or GitBash to run it.

* Ask a TA to send any solution files to students on Slack as the class begins.

#### Warm-Up Student Do: Variables (10 min)

[Starter File](Activities/01_Stu_Variables/Unsolved/variables.py)

[Instructions](Activities/01_Stu_Variables/README.md)

In this activity, students will get additional practice declaring, printing, and concatenating variables.

#### Warm-Up Student Do: Terminal and GitBash (5 min)

Students who have completed the variable activity can work on the following command-line activity.

They’ll use the command-line interface continually throughout the course, and they should get comfortable with the various commands.

[Command-Line Cheat Sheet](Activities/02_Stu_Terminal_Gitbash/Unsolved/CommandLine-Cheatsheet.md)

[Instructions](Activities/02_Stu_Terminal_Gitbash/README.md)

#### Warm-Up Student Do: Conditional Statements (10 min)

In this activity, students will declare and manipulate variables, as well as use `if-else` statements.

This material hasn't yet been covered in a live classroom setting, so it might present a challenge for some students.

[Starter File](Activities/03_Stu_Conditional_Statements/Unsolved/conditional_statements.py)

[Instructions](Activities/03_Stu_Conditional_Statements/README.md)

---

### 1. Instructor Do: Temperature Check (5 min)

Welcome students to the first required lesson of the course. Let them know that you’re thrilled to work with all of them and that you look forward to getting to know everyone better over the coming weeks.

Assure students that they aren’t alone if they feel overwhelmed by the async content and the prospect of the upcoming Challenge assignment. Let them know that you’ll cover material in the lesson tonight that will help them to both complete and submit their Challenge successfully.

> **Important:** Confirm that ALL students can access the async content's Python files, open them in VS Code, and run them in either Terminal or GitBash. If a student has an issue with this process, ask them to send a direct message to either you or a TA so that they can get individual help.

---

### 2. Instructor Do: Conditional Statements (10 min)

In this section, students will learn how conditional statements apply decision logic to control the flow of a computer program. Conditional statements are integral to decision-making in a computer program.

**Files:**

[conditionals.py](Activities/04_Ins_Conditionals/Solved/conditionals.py)

* Start with the concept that computers are simple, in that they only do exactly what you tell them to. If you want a useful script, you must write logic into the program.

* **Conditional statements** are evaluations of variables or expressions and their associated values. These evaluations dictate the behavior of the computer program.

  * The evaluation of the conditional statement controls the flow of the computer program.

  * This decision-making is called **conditional logic**, and it is a fundamental building block of all computer programs.

* Imagine a self-driving car. Code that tells the car's computer to drive forward will work for straight stretches of road. But what happens when a pedestrian steps into the path? You need to include additional logic to instruct the car's computer to not hit the pedestrian. Remember, computers only do what you tell them to!

Open a console within VS Code, and code the example of the self-driving car:

* What would happen if a driver fell asleep behind the wheel of a car? Well, if it's a self-driving car, nothing. The car's safety mechanisms will activate, and the car will begin auto-piloting itself to avoid collisions and swerving. If it's not a driverless car, well, a miracle might be needed. An example of such a case could look like the following code block:

  ```python
  driverless_car = True
  if driverless_car == True:
      # Do something
      print("Oh no! The driver's asleep! What do we do?!")
      print()
      print("All is good. Auto-pilot initiated.")
  else:
      # Do something else
      print("Oh no! The driver's asleep! MAYDAY! MAYDAY!")
  ```

* Conditionals can be executed by using **`if-else` statements**.

  * We create `if-else` statements by using the `if` and `else` keywords. Both keywords accept a condition. The `if` condition is usually specified, and the `else` defaults to the alternative.

  * Colons indicate which action should occur if the condition evaluates as defined.

* Conditional statements operate based on **Boolean conditions**, which are `True` or `False` values.

  * If a conditional statement returns `True`, the `if` statement will execute.

  * If a conditional statement evaluates as `False`, the program will behave according to what is defined by `else`.

  See the following example of a Boolean condition:

  ```python
  is_raining = True
  if is_raining:
      print("Bring an umbrella!")
  else:
      print("Leave the umbrella at home!")
  ```

Boolean is a pretty weird word, which makes it easier to remember! Booleans are named after their inventor, George Boole, a famous 19th-century logician.

Conditional statements can be used to control all types of decisions.

* Conditional statements can help you decide what value will be stored in a variable.

  * Revisit the self-driving car scenario. A car could have a variable of `immediate_action`. The value stored in `immediate_action` would be dependent on how conditional statements evaluate.

  * If there's not a pedestrian in the path, put `"drive"` in `immediate_action`.

  * Else, put `"stop"` in `immediate_action`, as follows:

    ```python
    pedestrian = False

    if not pedestrian:
        immediate_action = "drive"
    else:
        immediate_action = "stop"
    ```

* Think of conditional statements as optional gatekeepers for blocks of code. If you want the code to execute only under specific circumstances or conditions, use a conditional statement.

  * Equality is the most frequently used **comparison operator**. On Slack, send students the link to this [list of Python comparison operators](https://www.tutorialspoint.com/python/comparison_operators_example.htm).

  * The equality operator checks whether the value of one variable equals another; it returns `True` if both values equal one another, as follows:

    ```python
    x = 1
    if x == 1:
        print("x is equal to 1")

    y = 5
    if y == 1:
        print("x is equal to 1")
    ```

  * We can also use conditionals to check inequality.

    * There will be instances when computations or actions shouldn’t be executed if equality isn’t achieved.

    * The inequality operator returns `True` if the two values don’t equal one another, as shown in the following example:

      ```python
      z = 9
      if z != 1:
          print("y is not equal to 1")
      ```

  * Conditionals can include one or many conditions. When more than one condition is provided, the conditions have to be separated by **logical operators**. Logical operators include `AND` and `OR`. On Slack, send the link to this [list of Python logical operators](https://www.tutorialspoint.com/python/logical_operators_example.htm).

    * `AND` requires that both conditions return `True` for the action or computation to occur, as shown in the following example:

      ```python
      x = 1
      y = 10
      if x == 1 and y < 10:
          print("Both values returned True")
      ```

    * `OR` only requires one condition to return `True`.

  * We can create complex conditional statements by **nesting** `if-else` statements.

    * Nested `if-else` statements allow you to execute layers of computation.

    * For a nested `if-else` statement to execute, the first `if-else` condition must return `True`.

    * Note that you can use the `elif` keyword to include an extra set of conditions within the `if-else` decision structure. As the following image shows, `elif` works just as `if` does:

      ```python
      if x < 10:
          if y < 5:
              print("x is less than 10 and y is less than 5")
          elif y == 5:
              print("x is less than 10 and y is equal to 5")
          else:
              print("x is less than 10 and y is greater than 5")
      ```

Ask the students if they have any questions about conditional statements before moving on to an activity.

---

### 3. Student Do: Conditional Conundrum (10 min)

In this activity, students will review Python scripts that implement conditional statements using comparison and logical operators and try to determine the output before running the code.

**Files:**

[Starter File](Activities/05_Stu_Conditionals/Unsolved/conditionals.py)

[Instructions](Activities/05_Stu_Conditionals/README.md)

**Instructions:**

Working with conditional statements takes practice. Review each of the five conditional statement scenarios included with the starter file and see if you can determine the results before you run the code.

1. Open the [starter file](Activities/05_Stu_Conditionals/Unsolved/conditionals.py). Look through the examples and figure out what the output would be for each conditional statement.

2. Don’t run the code yet; first see if you can follow the thought process and guess.

3. Once you've guessed, run the file.

---

### 4. Instructor Do: Review Conditional Conundrum (10 min)

Take some time to walk through the solution while gauging students' comfort level with conditionals.

[Solution File](Activities/05_Stu_Conditionals/Solved/conditionals.py)

Begin by saying something like the following:

> "You've just learned a lot of new syntax and keywords. You've also started working with logical and comparison operators, and `if-else` statements are about to become your best friend.
>
> Let's reflect for a minute. What makes sense and what's still confusing?"

If no response is forthcoming, offer up the following question:

* In Python, how is a single equals sign (`=`) used versus that of a double equals (`==`)?

  **Answer:** The comparison operators use the double equals sign `==` to represent equality. The equals sign `=` assigns values to variables. What's the difference?

  * `==` checks to see if a value equals another; it double-checks equality. (Like all work, you want to double-check what you're doing!) So when you're basing a condition on equality, you should double-check what's being compared. You don't want to compare apples to oranges. They'll never be equal!

  * `=` is used to set and put values in a variable; it is used to assess and declare that a variable is something. You're not comparing it; you know for sure that this is the answer. Think back to algebra. When you finish showing your work in the calculation, you declare that `x = <some value>`. This is exactly how using the `=` works when declaring variables. You're declaring rather than evaluating.

* Be sure to focus on question #3, asking students what they think will print based on the following code—and why:

  ```python
  age = 18
  if age > 18:
      print("You are of voting age!")
  else:
      print("Argggggh! You think you can hoodwink me?! You're too young to vote!")
  ```

  Then ask students if this is the correct outcome based on the law. (The answer is no.)

Follow up with this question: how do you decide when to use greater than (`>`) and less than (`<`) operators, and when to use greater than or equal to (`>=`) and less than or equal to (`<=`)?

**Answer:** Deciding when to use specific comparison operators comes down to whether you want your conditional statement to include the minimum and maximum values needed to pass the condition.

* This is best explained with the example of the voting age. In the US, you have to be 18 years old or older to vote legally. The minimum acceptable age is 18.

* If we were to write a program to check whether someone's age meets the legal conditions, we’d need to check for the minimum value acceptable, plus all numbers greater than it. If the minimum number isn’t included, the program will say that people who are 18 can’t vote.

Ask students for two possible ways to fix the preceding logic.

**Answer:**

* Switch from using `age > 18` to `age >= 18`.

* Or check `if age > 17`, as shown in the following example:

    ```python
    age = 18
    if age > 17:
        print("You are of legal voting age!")
    else:
        print("Argggggh! You think you can hoodwink me?! You're too young to vote!")
    ```

    This code would return the following print statement:

    ```text
    Argggggh! You think you can hoodwink me! You're too young to vote!
    ```

Shift focus to #4 and nesting, shown in the following code block:

```python
height = 66
age = 16
adult_permission = True

if (height > 70) and (age >= 18):
    print("Can ride all the roller coasters")
elif (height > 65) and (age >= 18):
    print("Can ride moderate roller coasters")
elif (height > 60) and (age >= 18):
    print("Can ride light roller coasters")
elif ((height > 50) and (age >= 18)) or ((adult_permission) and (height > 50)):
    print("Can ride bumper cars")
else:
    print("Stick to lazy river")
```

* `if-else` statements can have multiple conditions, which can be achieved by using `elif` or by nesting `if-else` statements.

* `elif` statements basically indicate, “Hey, if the first round of conditions don't evaluate to true, try these!”

  * Consider `elif` statements a list of thorough checks used to weigh every option.

  * `else` encapsulates all scenarios that weren’t covered in the aforementioned conditions.

  * Consider the `else` block like a contingency plan: no matter what happens, the `else` statement has your back and is equipped with a plan of action.

If time remains, continue to review the activity solution and highlight the following details:

* We can combine comparison and logical operations to create complex decision structures.

* `if` conditions can be hardcoded or calculated.

  * We can provide a specific value as a condition (e.g., `x` must be greater than 10). So `10` is the hardcoded condition.

  * We can use a calculation to figure out what the condition value should be.

In the following example, instead of hardcoding the condition value, logic computes the condition:

```python
x = 2
y = 5
if (x ** 3 >= y) and (y ** 2 < 26):
    print("GOT QUESTION 5!")
else:
    print("Oh good you can count")
```

As you can see, condition 1 is `x ** 3 >= y`, and condition 2 is `y ** 2 < 26`.

Finally, engage students with the following questions:

* If you want to instruct your program or computer to behave a certain way, what should you use?

  **Answer:** Conditional statements. Conditional statements require specific conditions to be met for a block of code to be executed. Conditional statements evaluate expressions to determine whether the code should be executed. If the expression evaluates as `True`, the code is executed.

* How does the `AND` operator work?

  **Answer:** The `AND` logical operator requires all conditions to return `True` to satisfy the condition. The `AND` operator includes two conditions for evaluation.

* How does the `OR` operator compare to the `AND` operator?

  **Answer:** The `OR` logical operator works much like the `AND` operator; however, only one condition must return as `True`.

* How do nested `if-else` statements work?

  **Answer:** A nested `if-else` statement is an `if-else` statement within another `if-else` statement. The statements execute sequentially. For the nested `if-else` statement to execute, the first `if-else` statement must evaluate accordingly.

Review what students just learned by asking the following questions:

* We learned about two types of operators: logical and comparison. Is a greater than sign (`>`) a logical or comparison operator?

  **Answer:** Comparison.

* Is `OR` a logical or comparison operator?

  **Answer:** Logical.

* If you want TWO conditions to be met, which operator should you use?

  **Answer:** `AND`

* If you have two conditions, but either one is good enough, which operator should you use?

  **Answer:** `OR`

* What tells the computer that we want something that’s not equal to something else?

  **Answer:** `!`

* If you want to declare (or assign) a variable, do you use a single or double equals sign?

  **Answer:** You should use a single equals sign (`=`).

* When do you use double equals signs (`==`)?

  **Answer:** When you’re checking equality.

Reaffirm for students that conditional statements are extremely important because they control the flow of a computer program. If a program requires any type of evaluation to determine how the program will respond, a conditional statement will be required!

Answer any questions about conditional statements before moving on.

---

### 5. Instructor Do: Python Functions (10 min)

In this section, students are introduced to the concept of functions and the role they play in writing DRY code.

**File:**

[functions.py](Activities/06_Ins_Functions/Solved/functions.py)

**Functions** are blocks of reusable code that often perform repeated programmatic actions. Functions can be used whenever or wherever you need them within a program.

* Functions are valuable because they make programs more readable, modular, and reusable.

* Engage students by asking if they can remember any of the functions used in class so far. These functions might include the following examples:

  * `print()`

  * `append()`

  * `pop()`

Explain that these functions come built into Python. They are part of the underlying codebase. It’s also possible to create custom functions that allow us to decide exactly what happens with the code.

Open the [functions.py](Activities/06_Ins_Functions/Solved/functions.py) file.

* You can create a function by using the `def` keyword to define it. Give the function a name, then indent whatever code you want to become part of the function.

  * Mention that function names should follow the snake_case naming convention of other Python variables.

For the upcoming example, do NOT call the functions. Live code and define the following functions, then run the Python script and ask students what has happened:

```python
def hello():
    print("Hi! This is the hello function.")


def main(stock_ticker):
  print(stock_ticker + " is booming right now!")
```

Explain that a function won't be executed if it isn’t **called**. Add a line of code that shows the function call, like in the following example:

```python
hello()

main('AAPL')
```

Review the following mechanics of function inputs and outputs while showing the code:

* Functions should be designed to do only ONE task, and they should do that task very well.

* Functions are defined by the `def` keyword, a function name, a set of parentheses followed by a colon, and some type of execution statement or statements.

* Functions can have inputs, as outlined in the following guidelines:

  * Inputs are called **arguments**; arguments are passed into functions.

  * Arguments can be variables, data structures, or other functions.

  * Inputs are not required.

* Functions have outputs, as outlined in the following guidelines:

  * The output can range from a print statement to a complex computational value.

  * If a value is to be exported from a function, the `return` keyword must be used. This exported value can then be used elsewhere in the program.

  * The `return` keyword can only be used once per function, as shown in the following example:

    ```python
    def calculate_market_cap(market_price, number_of_shares):
        cap = market_price * number_of_shares
        # Output market_cap value
        return cap
    ```

  * Each function call will need to include all of the expected arguments.

  * By passing in an argument as input, a program can run the same code against two different types of input, as the following example shows:

    ```python
    stock_ticker = "SBUX"
    market_price = 76.06
    number_of_shares = 1243600000

    # Call calculate_market_cap() function
    market_cap = calculate_market_cap(market_price, number_of_shares)
    print(f"{stock_ticker} Market Capitalization: {market_cap}")
    ```

  * The output of a function can be captured and saved as a variable.

  * The variable to which you assign the output of the function will inherit the data type and value of the function output, like in the following example:

    ```python

    market_price = 76.06
    number_of_shares = 1243600000

    # Call calculate_market_cap() function and capture output as market_cap
    market_cap = calculate_market_cap(market_price, number_of_shares)
    print(f"Market Capitalization: {market_cap}")
    print(f"Data type of market_cap variable is: {type(market_cap)}")
    ```

* Variable scope is an important concept when working with functions. Variables can be understood as either globally or locally scoped.

  * **Globally** scoped variables are defined in the main body of the program, and the value can be accessed anywhere in the codebase.

  * **Locally** scoped variables are defined inside a function, so the value can only be accessed inside that function.

  * To work around this obstacle, return a function's locally scoped variable and capture the results in a different variable.

  * Let students know that variable scope is a difficult concept to understand—but if a function isn’t working as they expect, it might be due to a variable scoping issue, and the value might not be available where they think it should be.

> **Challenge Connection:** Advise students that they’ll use functions in the module Challenge.

Answer any questions students have about functions before moving on to a practice activity.

---

### 6. Student Do: Functions (10 min)

Advise students that this activity has a direct application to their Challenge assignment.

On Slack, send out both the instructions and starter files for the Functions student activity.

Remind students that they’ll need to open the file in VS Code to work with the code, but then navigate to the file in either Terminal or GitBash to run it.

Finally, if students seem overwhelmed by this activity, you can either send them to a breakout room for assistance or call it early and change it to a We Do group activity.

**Files:**

[Instructions](Activities/07_Stu_Functions/README.md)

[Starter code](Activities/07_Stu_Functions/Unsolved/functions.py)

**Instructions:**

Ever since you figured out how to calculate the total cost of the loan for your own new car, all of your friends have been asking you to do their calculations.

As such, it makes sense to put the future calculation in a function so that you only have to write it once but can call it over and over.

Use the instructions and the [starter file](Activities/07_Stu_Functions/Unsolved/functions.py) to create a `calculate_future_value` function, and call it using the following `new_car_loan` dictionary, as follows:

```python
new_car_loan = {
    "current_loan_value" : 25000,
    "months_remaining" : 6,
    "annual_interest_rate" : 0.085
}
```

Open the [starter file](Activities/07_Stu_Functions/Unsolved/functions.py) and complete the following steps.

1. Use the following future value formula for reference:

    ```python
    future_value = current_loan_value * (1 + (annual_interest_rate)) ** months_remaining
    ```

2. Create a function called `calculate_future_value` that fulfills the following criteria.

    * The function should take in three arguments: `current_loan_value`, `annual_interest_rate`, and `months_remaining`.

    * The function body should contain the `future_value` formula.

    * The function should return the `future_value`.

3. Call the `calculate_future_value` function, passing the relevant information from the `new_car_loan` dictionary as parameters. Make sure to set the function call equal to a variable called `cost_of_new_car`.

4. Print the `cost_of_new_car`. Round the figure to two decimal places.

---

### 7. Instructor Do: Review Functions (10 min)

[Solution File](Activities/07_Stu_Functions/Solved/functions.py)

Assume the `new_car_loan` dictionary was defined as follows:

```python
new_car_loan = {
    "current_loan_value" : 25000,
    "months_remaining" : 6,
    "annual_interest_rate" : 0.085
}
```

Review the Functions activity in detail, walking through the following key parts of the function:

* Creating the function and returning the `future_value` calculation, as follows:

  ```python
  def calculate_future_value(current_loan_value, annual_interest_rate, months_remaining):
      future_value = current_loan_value * (1 + (annual_interest_rate/12)) ** months_remaining
      print("fv", future_value)
      return future_value
  ```

* Calling the function and passing the required arguments

* Setting the function call equal to the variable `cost_of_new_car` to capture the value of the `future_value` calculation

* Printing the `cost_of_new_car` and rounding the figure to 2 decimal places, as follows:

  ```python
  cost_of_new_car = calculate_future_value(new_car_loan["current_loan_value"], new_car_loan["annual_interest_rate"], new_car_loan["months_remaining" ])

  print("The cost of the new car is: $", round(cost_of_new_car, 2))
  ```

Answer any additional student questions about functions before turning your attention to financial automation.

---

### 8. Break (5 min)

Gauge the students’ need for a break. If everyone seems engaged, you can either skip the break or postpone it until later.

---

### 9. Instructor Do: for Loops (15 min)

**Files:**

[loops.py](Activities/08_Ins_Loops/Solved/loops.py)

Introduce `for` loops by presenting the following scenario:

* Imagine that your new job at Accrual World, Inc., is to generate a daily report for each of your client's total sales. Every day, you need to gather the sales data from each client and then break out your trusty calculator to add up their total sales. This results in hours of manual labor.

* Just before you finish, you realize that you were given last week's data. You have to start over! Well, there's a better way to handle repetitive tasks like this.

At this point, transition your discussion to `for` loops, covering the following points:

* We’ve already learned how to tell computers what to remember by using variables. We also learned how to tell computers to make simple decisions by using conditionals. Now we'll tell computers to do what they do best: endlessly repeat an action.

* The ability to endlessly repeat the same decision or action for a large dataset is very valuable, and computers can do it much better than people can. Computers don't make as many mistakes, and they don't get tired!

* Almost every programming language has the concept of loops. **Loops** allow programs to execute code over and over until a condition exists to exit the loop. Simply put, a loop is a repeating process.

* Python has two types of loops: `for` and `while`. In this lesson, you’ll focus on `for` loops only.

* **`for` loops** are used for iterating over a sequence or collection. As each element in the sequence or collection is iterated over, the same process is executed on that element. They work according to the following principles:

  * `for` is a keyword and an iterator. It grants us access to each element in the sequence or collection one at a time.

  * At each cycle of the loop, a repeating action happens.

  * For example, if you have a string, “Hello World”, a loop would allow you to iterate over each letter in the phrase and perform some type of operation (e.g., capitalize each letter).

  * Another way to think about it is that if you loop a song, the song will play over and over again until the loop ends. DJs loop songs to make trendy beats; programmers loop blocks of code to automate tasks.

Open [loops.py](Activities/08_Ins_Loops/Solved/loops.py) and review the following points about `for` loops:

* `for` loops should be used when you want a process to run a certain number of times.

  * For example, let's say you're training a new analyst at an investment firm. Your supervisor has asked you to review the portfolio of clients to determine how each stock has performed over the last year. Your loop would look as follows:

    ```python
    for stock in portfolio:
        # Review `stock` performance
    ```

  * Notice how when we grab an element from the collection, we assign it a variable name that helps to identify it (i.e., `stock` as it relates to `portfolio`). That same variable name is what is referenced inside the loop to define the action.

  * In another example, executing a decision or behavior for each number in a range required the use of a `for` loop: you know you have a certain number of items, and you want a behavior executed for each item.

  * The `range()` function can be used to create a sequence of numbers based on the limit provided as input (e.g., 5). Ranges begin with 0 and increment by one. When looping over the range of numbers, we’ll put each number in variable `x`, as follows:

    ```python
    for x in range(5):
        print(x)
    ```

* Because strings are a sequence of letters, they can also be looped. When strings are looped, each character is iterated.

* In the following example, `x` is the variable and `phrase` is the sequence:

  ```python
  word = "fINtECH rOCKS!"
  for letter in word:
      print(letter.swapcase())
  ```

  * In the first iteration of the preceding loop, `x` is “H”.

  * In the second iteration, `x` is “e”.

* Lists are a natural choice for iterating over `for` loops because you can efficiently access each element in the list and perform an action, as shown in the following example:

  ```python
  shopping_spree_charges = [117.95, 17, 35, 77.83, 345.67, 45.39]
  spending_total = 0.00

  for charge in shopping_spree_charges:
      spending_total += charge
      print("Inside loop: $", spending_total)

  print("The total spent on my spending spree was $", round(spending_total, 2))
  ```

  * Highlight how `spending_total` was initialized as a floating point variable. This is common in fintech when working with currency values and prices.

  * Call attention to the shortcut syntax for `+=`, called the **addition assignment operator**. It is short for `spending_total = spending_total + charge`.

  * Finally, call out how the `spending_total` calculation is displayed both inside and outside the loop.

  * Ask students what would happen if the `spending_total` variable was declared inside the `for` loop.

  **Answer:** The sum would be reset to 0.00 every time through the loop!

It’s also possible to iterate over dictionaries, with some slight adjustments to the syntax.

* With a list, we can access each element directly, but with a dictionary you have to go through the key to get to the value.

Referring back to the `trading_pnl` dictionary, see the following example:

```python
trading_pnl = {
    "03-18-2019": -224,
    "03-19-2019": 352,
    "03-20-2019": 252,
    "03-21-2019": 354,
    "03-22-2019": -544,
    "03-23-2019": -650,
    "03-24-2019": 56,
    "03-25-2019": 123,
    "03-26-2019": -43,
    "03-27-2019": 254,
    "03-28-2019": 325,
    "03-29-2019": -123,
    "03-30-2019": 47,
    "03-31-2019": 321,
    "04-01-2019": 123,
    "04-02-2019": 133,
    "04-03-2019": -151,
    "04-04-2019": 613,
    "04-05-2019": 232,
    "04-06-2019": -311
}
```

* Capture just the keys with the following syntax:

  ```python
  for key in trading_pnl:
      print(key)
  ```

* To capture the values, use the following syntax:

  ```python
  for key in trading_pnl:
      print(trading_pnl[key])
  ```

* With the values, we can perform calculations as follows:

  ```python
  net_pnl = 0.00

  for key in trading_pnl:
      net_pnl += trading_pnl[key]
      print("Inside loop:", net_pnl)

  print("The net pnl for the period was $", round(net_pnl, 2))
  ```

* The final point you should stress about `for` loops is that they’re the beginning of the **automation process**. Being able to access every element in a data set—whether it be in the form of a list or a dictionary—and perform an action on that element means that we can begin to convert the manual processes to automated ones.

* By combining functions with `for` loops, we can automatically pass in a dataset, iterate over each element, perform an action or analysis, and then return the resulting value back to be used later on in the program.

* This is largely what fintech is all about—automating manual processes so that they become faster, more efficient, and more cost-effective!

Answer any questions about iterators and `for` loops before moving on to student activity.

---

### 10. Student Do: Loop-De-Loop (15 min)

In this activity, students will explore a number of use cases for using loops to gain more experience with iterating through both lists and dictionaries. These activities should give them some insight into what’s required in the Challenge assignment.

Send the following files to the students on Slack for this activity.

**Files:**

[Instructions](Activities/09_Stu_Loops/README.md)

[Starter code](Activities/09_Stu_Loops/Unsolved/loops.py)

**Instructions:**

You’re doing a brief review of your portfolio's performance over the month of February 2019. Use loops to help determine the net total of gains and losses for the period. You can also use loops to help determine the days with big gains versus the days that had big losses.

Using the [starter code](Activities/09_Stu_Loops/Unsolved/loops.py) provided, loop through the provided list and dictionary to find the information specified by the instructions.

**Looping Through a List:**

List of Portfolio gains and losses for the investment period of February 2019:

```python
portfolio_gain_loss_list = [
    168.48, 2445.21, 1461.00, -461.98,
    -3368.62, 427.03, 193.99, 4443.63,
    1132.76, -779.18, 3372.93, 604.64,
    703.99, -1249.01, 2156.62, 475.81,
    -250.61, -150.43, -653.08
]
```

1. Using a `for` loop, calculate the total sum of gains and losses for the period. Print the result.

2. Using the `len()` method, determine the number of days in the investment period. Set that value equal to a variable called `number_of_days`. Print the value.

3. Use the `sum_list` and `number_of_days` variables to determine the `average_gain_loss_per_day` value. Print that value, rounding it to 2 decimal places.

**Looping Through a Dictionary:**

Dictionary of portfolio gains and losses for the investment period of February 2019.

```python
portfolio_gain_loss_dict = {
    "02-01-2019": 168.48,
    "02_04-2019": 2445.21,
    "02-05-2019": 1461.00,
    "02-06-2019": -461.98,
    "02-07-2019": -3368.62,
    "02-08-2019": 427.03,
    "02-11-2019": 193.99,
    "02-12-2019": 4443.63,
    "02-13-2019": 1132.76,
    "02-14-2019": -779.18,
    "02-15-2019": 3372.93,
    "02-19-2019": 604.64,
    "02-20-2019": 703.99,
    "02-21-2019": -1249.01,
    "02-22-2019": 2156.62,
    "02-25-2019": 475.81,
    "02-26-2019": -250.61,
    "02-27-2019": -150.43,
    "02-28-2019": -653.08
}
```

1. Using a `for` loop, calculate the total sum of gains and losses for the period. Print the result.

    **Hint:** This total should match the one calculated from looping through the list.

2. Conditionally filter the dictionary to find the days with a gain greater than or equal to $1000 or a loss less than or equal to -$1000. Add these gain or loss values only to either the `big_gains` list or `big_losses` list—print both lists.

3. Loop through both the `big_gains` and `big_losses` lists to determine whether the days with the big gains were more profitable than the days with the big losses were painful.

---

### 11. Instructor Do: Review Loop-De-Loop (10 min)

[Solution File](Activities/09_Stu_Loops/Solved/loops.py)

Review the solution for each loop while engaging students with the following questions:

* How do `for` loops execute?

  **Answer:** `for` loops operate by executing iteratively over a sequence or collection.

* What are the components of `for` loops?

  **Answer:** `for` loops are composed of a variable and a sequence or collection.

* What do variables represent in a `for` loop?

  **Answer:** Variables represent a single element contained within the sequence or collection. This element holds a specific position, which the `for` loop can access.

* How do you create a range of numbers to loop over?

  **Answer:** The `range()` function can create a range of numbers.

Solution to looping over the list:

```python
sum_list = 0.00
for day in portfolio_gain_loss_list:
    sum_list += day
print("Total gain_loss", round(sum_list, 2))

# Answer
# Total gain_loss 10673.18
```

Solution for calculating the average gain or loss per day:

```python
number_of_days = len(portfolio_gain_loss_list)
print("The number of days in the period was", number_of_days)
average_gain_loss_per_day = sum_list / number_of_days
print("The average gain/loss per day was", round(average_gain_loss_per_day, 2))

# Answer
# The number of days in the period was 19
# The average gain/loss per day was 561.75
```

Solution to looping over the dictionary:

```python
sum_dict = 0.00
for key in portfolio_gain_loss_dict:
    sum_dict += portfolio_gain_loss_dict[key]
print("Total gain_loss", round(sum_dict, 2))

# Answer
# Total gain_loss 10673.18
```

Solution to conditionally filtering the dictionary:

```python
big_gains = []
big_losses = []
for key in portfolio_gain_loss_dict:
    if portfolio_gain_loss_dict[key] >= 1000:
        big_gains.append(portfolio_gain_loss_dict[key])
    if portfolio_gain_loss_dict[key] <= -1000:
        big_losses.append(portfolio_gain_loss_dict[key])
print("The biggest gains were:", big_gains)
print("The biggest losses were:", big_losses)

# Answer
# The biggest gains were: [2445.21, 1461.0, 4443.63, 1132.76, 3372.93, 2156.62]
# The biggest losses were: [-3368.62, -1249.01]
```

Solution to looping through the `big_gains` and `big_losses` lists:

```python
total_big_gains = 0.00
total_big_losses = 0.00
for gain in big_gains:
    total_big_gains += gain
for loss in big_losses:
    total_big_losses += loss
print("The big gains total was", round(total_big_gains, 2))
print("The big losses total was", round(total_big_losses, 2))

# Answer:
# The big gains total was 15012.15
# The big losses total was -4617.63
```

Answer any questions before moving on to the GitHub activity.

---

### 12. Instructor Do: GitHub (10 min)

As part of the submission for the Challenge assignment, the students will have to upload their folder to a GitHub repository. Please work through these steps—along with the students—to both create a new repository and manually upload and commit a folder.

Advise students that Git and GitHub are tools that make tracking different versions of a program's files and folders easy.

* **Git** is the version-control system that allows developers to track changes to files and folders. Git is software.

* **GitHub** is a central location to create projects, host files and folders, and track changes to the files and folders associated with those projects. Github is a user interface that uses the Git software. GitHub is just one of many vendors that use Git on the back end (e.g., GitLab, BitBucket, SourceForge, etc.).

Under the hood, GitHub uses the Git tool for file versioning.

Walk students through the following steps for creating a repo:

1. Everyone logs into their GitHub account.

2. From the GitHub account main page, create a NEW repository with a repository name of your choice, keep the repository Public, and check the **Initialize a README.md box**. Click the **Create repository** button.

    * Advise students that they’ll repeat this process over and over again. The trick is to always check the **Initialize a README.md** box.

3. With your repository created, turn your attention to Visual Studio Code. Complete the following steps:

    * On your desktop, create a folder called 'Github_Upload'.

    * Open that folder in VS Code and create a new file named `main.py`.

    * Inside the `main.py` file, create a print statement that logs your name, like the following example:

      `print("Hello, My name is <your name here>.")`

    You should now have a folder called `Github_Upload' on your desktop that contains a Python file inside of it.

4. Navigate back to your repository on the Github GUI and click the **Upload files** button.

5. Drag and drop your `Github_Upload` folder from your desktop into the appropriate space on the file upload window. Point out that the file path appears below the box.

6. Add the required commit messages and click the **Commit changes** button.

7. From the main screen, you can now see and navigate to the folder that was just uploaded.

    You can now navigate the folder structure and even edit the `main.py` file directly from inside GitHub.

    **Important:** Any changes students make to a Python file directly in Github will NOT be automatically transferred back down to your local machine. To transfer information back and forth between your local machine and Github, you’ll be doing **pushes** and **pulls**, but more on those in Module 2.

8. Show the students that they can see the commits that you made to this new repository by clicking on the commits tab.

Let the students know that that process of creating a repository and uploading files should begin to feel more comfortable as they continue to do it.

The specific steps for this activity can be found in the last lesson in their async content.

> **Important:** Again, advise students that this is the process they’ll use to upload their submission for the Module 1 Challenge. They should ask questions if they have them.

Finally, let students know that what they’ve learned in this lesson just barely scratches the surface of what Git and Github offer. They’ll learn much more about the functionality and importance of both systems in Module 2.

---

## Open Office Hours (Optional)

### Q&A and System Support

This is an opportunity to support students in any way that they require.

* Ask the students if they have any questions about the material covered in today's lesson.

* Remind them that their Challenge assignment is due after presentations.

* Advise students of instructional staff availability over the weekend.

* Dismiss students for the evening.

---

© 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
