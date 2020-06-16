# Jetbrainsproject
Storing jet brains project notes

Function

>> A function is a block of code that does some useful work for you, e.g. prints a text. 
>> In some sense, a function is a subprogram that can be reused within your programs. 
>> When the name of a function is followed by parentheses, it means that it was called to get the result.

Using quotes convention

>> Use double quotes if your string contains single quotes, for example, "You're doing great!"
>> Use single quotes if your string contains double quotes, for example, 'Have you read "Hamlet"?'
>> do NOT mix two styles in one literal, for example, something like "string!' is NOT correct
>> most importantly, be consistent in your use!

Escaping
>> Using the backslash symbol (\) before the quotes inside of the string will tell Python that the quote symbol that follows it is a part of the string.
>> Rather than its end or beginning. It is called escaping.

Multiple lines 

>> You can also write multi-line strings in Python, and to do that you need to use triple quotes on each side of the string literal.
>> Example: 
print("""This
is
a
multi-line
string""")

Type Casting

>> The process of converting a value to another type is also called type casting
>> Example:
>> raw_age = "22"
    print(type(raw_age))  # <class 'str'>
    age = int(raw_age)
    print(type(age))  # <class 'int'>

>> string containing float numbers cannot be converted to int directly. Change to float then to int. But str with int number can be converted to float directly












