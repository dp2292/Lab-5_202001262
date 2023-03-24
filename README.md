# Lab-5_202001262
# Devansh Patel 202001262
Software engineering Lab 5 Submission

In this lab I will do static analysis of the codes.

For doing static analysis I will be using Pylint Tool.

## Installation of Pylint Tool

Pylint is a widely-used tool for analyzing Python code quality and detecting errors, potential bugs, and other issues. It is a popular static code analysis tool that can check the adherence to coding standards, identify potential bugs, and suggest refactoring to improve code quality. Pylint analyzes the source code of Python programs and generates reports on its quality, including code complexity, coding standards adherence, unused code, and many other metrics. It can be integrated with various IDEs and text editors, such as PyCharm, Visual Studio Code, and Sublime Text, to provide real-time feedback on code quality.

![1](https://user-images.githubusercontent.com/75575802/227485588-0ff00e51-62a9-4f0f-b626-108e167e4a26.png)

For the static analysis I will be using multiple python files found online.


### Code 1

+ https://github.com/geekcomputers/Python/blob/master/PDF/images.py

![2](https://user-images.githubusercontent.com/75575802/227486238-6f106ae2-0931-4b6f-80b4-d1011e95af90.png)

### Errors
code1.py:3:0: E0401: Unable to import 'PIL' (import-error)
code1.py:4:0: E0401: Unable to import 'fpdf' (import-error)
code1.py:31:8: C0103: Constant name "orientation" doesn't conform to UPPER_CASE naming style (invalid-name)

The first error, E0401: Unable to import 'PIL' (import-error), means that the Python Imaging Library (PIL) module could not be imported. This error might occur due to several reasons, such as not having the module installed, an incorrect module name, or a problem with the module's installation or configuration.

The second error, E0401: Unable to import 'fpdf' (import-error), indicates that the fpdf module could not be imported. The error message is similar to the first one and may occur for similar reasons.

### Code 2

+ https://github.com/qxf2/wtfiswronghere/blob/master/05_challenge/05_challenge.py

![3](https://user-images.githubusercontent.com/75575802/227486383-476b56da-a42f-493b-aaf8-dea7b5339bcc.png)

### Errors

code2.py:20:9: E0001: Parsing failed: 'Missing parentheses in call to 'print'. Did you mean print(...)? (<unknown>, line 20)' (syntax-error)
  
This error message indicates that there is a syntax error in the Python script code2.py. Specifically, the error is occurring on line 20, column 9, and it is caused by a missing set of parentheses in a call to the print function.

The error message suggests that the correct syntax for calling print is print(...), with the ellipsis indicating the arguments that should be passed to the function.

### Code 3

+ https://github.com/geekcomputers/Python/blob/master/Eight_Puzzle_Solver/eight_puzzle.py

![4](https://user-images.githubusercontent.com/75575802/227486720-4b6ce18b-8599-4748-b426-c9a98204c027.png)
  
### Errors
  
code3.py:256:12: R1705: Unnecessary "else" after "return", remove the "else" and de-indent the code inside it (no-else-return)
code3.py:244:4: R0911: Too many return statements (7/6) (too-many-return-statements)
code3.py:266:0: C0115: Missing class docstring (missing-class-docstring)
  
R1705: Unnecessary "else" after "return", remove the "else" and de-indent the code inside it (no-else-return):
This error message suggests that there is an unnecessary else statement after a return statement that should be removed. The code inside the else block will never be executed, so it is unnecessary and can be deleted.

R0911: Too many return statements (7/6) (too-many-return-statements):
This error message indicates that the Python function has more return statements than recommended. The code might be hard to read and understand when there are too many return statements, so the tool suggests consolidating the return statements where possible.
  

### Code 4

+ https://github.com/geekcomputers/Python/blob/master/Colors/pixel_sort.py

![5](https://user-images.githubusercontent.com/75575802/227486888-e9b292f1-0bdc-4d4c-8eec-41a46e752323.png)
  
### Errors
  
code4.py:7:0: C0411: standard import "import colorsys" should be placed before "import cv2" (wrong-import-order)
code4.py:9:0: C0411: standard import "import os" should be placed before "import cv2" (wrong-import-order)
code4.py:10:0: C0411: standard import "import argparse" should be placed before "import cv2" (wrong-import-order)
  
C0411: standard import "import colorsys" should be placed before "import cv2" (wrong-import-order):
This error message suggests that in the Python script code4.py, the standard import statement for colorsys should be placed before the import statement for cv2. The tool is recommending a specific order for imports to make the code more readable and maintainable.

C0411: standard import "import os" should be placed before "import cv2" (wrong-import-order):
This error message is similar to the first one, but it suggests that the standard import statement for os should be placed before the import statement for cv2.

C0411: standard import "import argparse" should be placed before "import cv2" (wrong-import-order):
This error message is also similar to the first two, but it suggests that the standard import statement for argparse should be placed before the import statement for cv2.

### Code 5

+ https://github.com/geekcomputers/Python/blob/master/Cat/cat.py

![6](https://user-images.githubusercontent.com/75575802/227487041-88f6fd3b-16b6-414e-9876-c6d38cbfb857.png)
  
### Errors

code5.py:28:8: R1722: Consider using 'sys.exit' instead (consider-using-sys-exit)
code5.py:42:8: R1722: Consider using 'sys.exit' instead (consider-using-sys-exit)
code5.py:44:8: R1722: Consider using 'sys.exit' instead (consider-using-sys-exit)
  
R1722: Consider using 'sys.exit' instead (consider-using-sys-exit):
This error message indicates that the Python code is using the exit() function to terminate the program. The tool suggests that the sys.exit() function should be used instead, as it provides a more standardized and reliable way to exit a Python script. The sys.exit() function can take an optional argument that specifies the exit status code.

R1722: Consider using 'sys.exit' instead (consider-using-sys-exit):
This error message is similar to the first one, and it suggests using the sys.exit() function instead of exit() to terminate the program.

R1722: Consider using 'sys.exit' instead (consider-using-sys-exit):
This error message is also similar to the first two, and it suggests using the sys.exit() function instead of exit() to terminate the program.
