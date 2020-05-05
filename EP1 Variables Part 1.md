# EP1 Python and Python Variables
## Python programming language
1. **High-level** programming language
2. **Dynamically typed**
3. **Auto garbage collection**

## Python compiling
1. Python **has** compiler and it compile program automatically.
2. Python does not compile program to native machine code, it compiles programs into byte code
3. Python has virtual machine which can run compiled byte codes

## Python variable names
1. Must start with a letter or underscore, **CANNOT** start with a number
2. Can only use characters from A-Z, a-z, 0-9 and _
3. Case-sensitive (*name*, *Name*, *NAME* are different variables)
4. Avoid using keywords (AFAIK 33 in total)

    | Keywords ||||
    | -|-|-|-|
    | and | except | lambda | with |
    | as | finally | nonlocal | while |
    | assert | False | None | yield |
    | break | for | not | class |
    | from | or | continue | global |
    | pass | def | if | raise |
    | del | import | return | elif |
    | in | True | else | is |
    | try | | | |
5. PEP8 (*Python Enhancement Proposals*): variable names in lowercase, words separated by **underscores**

## Primitive Types
1. Integer
    * Python2 <*int*>, <*long*>
    * Python3 <*int*>
    * Range:
        ```python
        import sys
        sys.maxsize # gives us the max positive value of int
        type(sys.maxsize) # => <class 'int'>
        # Python2
        type(sys.maxsize + 1) # => <type 'long'>
        # Python3
        type(sys.maxsize + 1) # => <class 'int'>
        # Python2
        type(-sys.maxsize - 2) # => <type 'long'>
        # Python3
        type(-sys.maxsize + 2) # => <class 'int'>
        ```
    * Based integer range: **-2147483648 ~ 2147483647**
        * Range may larger on machine with larger natural word size but not smaller than based integer range.
2. Float
    * Python only support double precision
3. Boolean
    * Two values: *True* and *False*
    * Note: Captical **T** and Captical **F**
4. String
    * text enclosing a sequence of characters in a **single**, **double** or **triple** quotes
    ```python
    greeting = "hello"
    user_name = 'botLearner'
    # multiple lines
    greeting_user = """
        Hello,
        botLearner
    """
    # OR
    greeting_user = "Hello,\nbotLearner"
    ```







