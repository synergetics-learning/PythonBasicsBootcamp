# Error Handling Statements

<b> The three lines of code written below will run successfully without any issues </b>


```python
a=4
print(a**2)
print("Important Line")
```

    16
    Important Line
    

<b> NOTE: In python, if we recieve a error at any line, then python will stop the execution at that line itself </b>

<b> If we consider the three lines of code written below, since a error will be thrown at the second line, the execution will stop at the second line itself. And the third line of code will not be executed. This means that in python by default, the errors are not being handled effectively. Hence there is a need for error-handling statements </b>


```python
a="apple"
print(a**2)
print("Important Line")
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-2-517f16f9de0c> in <module>
          1 a="apple"
    ----> 2 print(a**2)
          3 print("Important Line")
    

    TypeError: unsupported operand type(s) for ** or pow(): 'str' and 'int'


 <b>Syntax to create "try" statement </b> <br>

try:
    #blockOfCode

<b>Syntax to create "except" statement</b> <br>

except:
    #blockOfCode

<b>Syntax to create "else" statement</b> <br>

else:
    #blockOfCode

<b>Syntax to create "finally" statement </b><br>

finally:
    #blockOfCode

<b>How to create blockOfCode </b><br>
1) We need to have atleast line of code in the blockOfCode <br>
2) All the lines of code in the blockOfCode need to have some space before it <br>
3) All the lines of code in the blockOfCode need to have same space before it <br>

<b>Points to remember w.r.t. Error-Handling Statements </b> <br>

1) try     -- a) The "try" statement is mandatory <br>
&emsp; &emsp; &emsp;   b) The code on which you have doubt that it can generate a error, such code you will put in the blockOfCode of "try" statement. <br>
&emsp; &emsp; &emsp;              c) The blockOfCode of the "try" statement will always get executed first <br>
&emsp; &emsp; &emsp;              d) The "try" statement can only be written once <br>
&emsp; &emsp; &emsp;              e) The "try" statement cannot be alone, it has to accompanied by some other error-handling statement <br>
2) except  -- a) The "except" statement is not mandatory <br>
   &emsp; &emsp; &emsp;           b) The code that you want to execute if there is error in the try statement, such code such code you will put in the blockOfCode of "except" statement. <br>
   &emsp; &emsp; &emsp;           c) The blockOfCode of the "except" statement will get executed only if there is a error in the try statement <br>
  &emsp; &emsp; &emsp;            d) The "except" statement can only be written once <br>
3) else    -- a) The "else" statement is not mandatory <br>
   &emsp; &emsp; &emsp;           b) The code that you want to execute if there is no error in the try statement, such code such code you will put in the blockOfCode of "else" statement.<br>
   &emsp; &emsp; &emsp;           c) The blockOfCode of the "else" statement will get executed only if there is NO error in the try statement <br>
   &emsp; &emsp; &emsp;           d) The "else" statement can only be written once <br>
   &emsp; &emsp; &emsp;           e) The "else" statement can only be written, only if the "except" statement is present <br>
4) finally -- a) The "finally" statement is not mandatory <br>
    &emsp; &emsp; &emsp;          b) The code that you want to execute no matter what happens in the try statement, such code such code you will put in the blockOfCode of "finally" statement. <br>
    &emsp; &emsp; &emsp;          c) The blockOfCode of the "finally" statement will get executed at the last no matter what happens in the try statement <br>
 &emsp; &emsp; &emsp;             d) The "finally" statement can only be written once <br>


```python
a='apple'
```

 <b>The code for Error-Handling Statements written below is valid </b>


```python
# The Error-Handling Statements created below, are valid
try:
    print(a**2)
except:
    print("The exponent operation was not successful")
else:
    print("The exponent operation was successful")
finally:
    print("Important Line")
```

    The exponent operation was not successful
    Important Line
    


```python
a=4
```

 <b>The code for Error-Handling Statements written below is valid </b>


```python

try:
    print(a**2)
except:
    print("The exponent operation was not successful")
else:
    print("The exponent operation was successful")
finally:
    print("Important Line")
```

    16
    The exponent operation was successful
    Important Line
    


```python
a='apple'
```

 <b>The code for Error-Handling Statements written below is valid </b>


```python

try:
    print(a**2)
except:
    print("The exponent operation was not successful")
finally:
    print("Important Line")
```

    The exponent operation was not successful
    Important Line
    


```python
a=4
```

<b> The code for Error-Handling Statements written below is invalid, because we cannot have the "else" statement without the "except" statement
</b>


```python

try:
    print(a**2)
else:
    print("The exponent operation was successful")
finally:
    print("Important Line")
```


      File "<ipython-input-10-f92d325e662f>", line 3
        else:
        ^
    SyntaxError: invalid syntax
    



```python
a=4
```

<b> The code for Error-Handling Statements written below is invalid, because we cannot have the "try" statement cannot be alone, it has to be accompanies by some other error-handling statement
</b>


```python
try:
    print(a**2)

```


      File "<ipython-input-12-0399c13aa887>", line 2
        print(a**2)
                   ^
    SyntaxError: unexpected EOF while parsing
    


 <b>The code for Error-Handling Statements written below is valid </b>


```python
try:
    print(a**2)
finally:
    print("Important Line")
```

    16
    Important Line
    


```python

```
