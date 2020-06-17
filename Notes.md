# Jetbrainsproject
Storing jet brains project notes

Function

    A function is a block of code that does some useful work for you, e.g. prints a text. 
    In some sense, a function is a subprogram that can be reused within your programs. 
    When the name of a function is followed by parentheses, it means that it was called to get the result.

Using quotes convention

    Use double quotes if your string contains single quotes, for example, "You're doing great!"
    Use single quotes if your string contains double quotes, for example, 'Have you read "Hamlet"?'
    do NOT mix two styles in one literal, for example, something like "string!' is NOT correct
    most importantly, be consistent in your use!

Escaping

    Using the backslash symbol (\) before the quotes inside of the string will tell Python that the quote symbol that follows it is a part of the string.
    Rather than its end or beginning. It is called escaping.

Multiple lines 

    You can also write multi-line strings in Python, and to do that you need to use triple quotes on each side of the string literal.
    
    Example: 
    print("""This
    is
    a
    multi-line
    string""")

Type Casting

    The process of converting a value to another type is also called type casting
    
    Example:
    raw_age = "22"
    print(type(raw_age))  # <class 'str'>
    age = int(raw_age)
    print(type(age))  # <class 'int'>
    string containing float numbers cannot be converted to int directly. Change to float then to int. But str with int number can be converted to float directly

Arithmetic Operation

    Four arithmetic operation. Double slash(//) used for integer division. Error if try to divide by zero.
    Reminder of division to find of even or odd number
    
    Examples:
    print(7 % 2)  # 1, because 7 is an odd number
    print(8 % 2)  # 0, because 8 is an even number
    
    # Divide the number by itself
    print(4 % 4)     # 0
    # At least one number is a float
    print(11 % 6.0)  # 5.0
    # The first number is less than the divisor
    print(55 % 77)   # 55
    # With negative numbers, it preserves the divisor sign
    print(-11 % 5)    # 4. 5 is positive so reminder is positive.
    print(11 % -5)    # -4 5 is negative so reminder is negative.
    
    Exponention. to the power
    Example: print(10 ** 2)  # 100


Operation priority

    To sum up, there is a list of priorities for all considered operations:

    parentheses
    power
    unary minus
    multiplication, division, and remainder
    addition and subtraction
    
    In case of same priority operations, Python follows a left-to-right operation convention from mathematics

PEP on binary operation

    surround a binary operator with a single space on both sides
    Example:
    number=30+12      # No!
    number = 30 + 12  # It's better this way
    

Knuth's style

    formulas always break before binary operations
    # Yes: easy to match operators with operands
    income = (gross_wages
              + taxable_interest
              + (dividends - qualified_dividends)
              - ira_deduction
              - student_loan_interest)

Boolean logic

    True False value
    3 boolean operators
    2 binay operators; and & or, 1 unary operator; not

    And operator:
    a = True and True    # True
    b = True and False   # False
    c = False and False  # False
    d = False and True   # False

    OR operator:
    a = True or True    # True
    b = True or False   # True
    c = False or False  # False
    d = False or True   # True

    NOT operator:
    to_be = True           # to_be is True
    not_to_be = not to_be  # not_to_be is False
    
    Here are the operators in order of their priorities: not, and, or. So, not is considered first, than and, finally or.
    print(False or not False)  # True

Truthy and Falsy Values

    When used with logical operators, values of non-boolean types, such as integers or strings, are called truthy or falsy
    It depends on whether they are interpreted as True or False.

    The following values are evaluated to False in Python:
    constants defined to be false: None and False,
    zero of any numeric type: 0, 0.0,
    empty sequences and containers: "", [], {}.
    Anything else generally evaluates to True
    
    Example: Falsy;
    print(0.0 or False)  # False
    print(False and "")  # False
    
    Truthy;
    # `and` has a higher priority than `or`
    truthy_integer = False or 5 and 100  # 100

    The operators or and and return one of their operands, not necessarily of the boolean type. Nonetheless, not always returns a boolean value.
    Example: tricky = not (False or '')  # True




