# Python Programming

In this part of the course you will learn the basics of Python programming, from data types to scientific packages.

The contents of the course are distributed in lessons, grouped by topic (functions, conditional structures, exceptions...) in the form of [Jupyter Notebooks](https://jupyter.org/). These are the elements that you will discover through the lessons:

- **Theory blocks**: information regarding the current study topic.
- **Code blocks**: embedded scripts that can be executed by clicking the "Play" button on its upper-left corner. These blocks are not meant to be modified.
- **Playgrounds**: code blocks intended for you to modify and explore a specific functionality.
- **Exercises**: sets of instructions that describe the structure of a practical exercise, which you must solve.

## Exercises

Exercises will contain links to **dedicated scripts** (files where you will need to add your own code). They will also contain instructions on how to execute **tests** over said scripts, which will automatically determine where you are failing, or just verify that your solution is right.

### Tests

In order to execute tests, you will need to execute a specific task that matches the number of the exercise you are solving, for example, here is the description for exercise 4:

> _Exercise 4: Type casting_
>
> Initial data:
>
> - Variable `value` with value `123`.
>
> Steps:
>
> 1. Create a variable named `casted` that contains the value of the `value` variable casted to a string.
>
> - [Click here to open the script in the editor](./solutions/exercise_04.py)
> - Test the script using `Ctrl + Shift + P` > `Tasks: Run Task` > `Test exercise 04`

Note that the last line instructs you to open the command palette of Visual Studio Code. Once you open it and search for *"Tasks: Run Task"*, you will be able to choose amongst plenty of tests.

![Test selection](/media/lessons/tests-1.png)

Do not look for the test manually, just write its number and it will be selected automatically.

![Test search](/media/lessons/tests-2.png)

Last step is to press enter and the test will be executed in a dedicated terminal window. Here is what you would see when you still have not modified exercise 4:

```powershell
=========================================================================== test session starts ============================================================================
collected 1 item

lessons\solutions\solution_tests\test_exercise_04.py F

================================================================================= FAILURES =================================================================================
V:\development\repositories\basic-formation-courses\lessons\solutions\solution_tests\test_exercise_04.py:12: AssertionError: You have not defined the variable `casted`.
========================================================================= short test summary info ==========================================================================
FAILED lessons/solutions/solution_tests/test_exercise_04.py::test - AssertionError: You have not defined the variable `casted`.
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! stopping after 1 failures !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
============================================================================ 1 failed in 0.10s =============================================================================
```

The relevant part of this report is the line above all the exclamation marks. If you read it carefully, you will notice it says *"You have not defined the variable `casted`."*. This is self explanatory. If you then add the variable casted, but the value is not right, you will receive the following report:

```powershell
=========================================================================== test session starts ============================================================================
collected 1 item

lessons\solutions\solution_tests\test_exercise_04.py F

================================================================================= FAILURES =================================================================================
V:\development\repositories\basic-formation-courses\lessons\solutions\solution_tests\test_exercise_04.py:14: AssertionError: The variable `casted` has the wrong value.
========================================================================= short test summary info ==========================================================================
FAILED lessons/solutions/solution_tests/test_exercise_04.py::test - AssertionError: The variable `casted` has the wrong value.
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! stopping after 1 failures !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
============================================================================ 1 failed in 0.16s =============================================================================
```

The error now says *"The variable `casted` has the wrong value."*. Finally, if you set the right value, you will receive the following report:

```powershell
=========================================================================== test session starts ============================================================================
collected 1 item

lessons\solutions\solution_tests\test_exercise_04.py .

============================================================================ 1 passed in 0.18s =============================================================================
```

As you can imagine, *"passed"* means that you successfully completed the exercise. There are multiple error variants, depending on the feedback required for each exercise. There can even be errors that are not defined in the tests (i.e. syntax errors). **Always make sure to read the error messages at least two times**.

## Let's go!

Now you are ready to take on the lessons and exercises, so go ahead and dive into [the first lesson](./introduction.ipynb).