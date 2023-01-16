# Operators

<b> Types of Operators </b> <br>
1) Arithmetic Operators <br>
2) Comparison Operators <br>
3) Logical Operators <br>

# 1) Arithmetic Operators


<b>Arithmetic Operators are used to do some arithmetic operation or mathematical operation on two values</b>

<b>Types of Arithmetic Operators: </b> <br>
1) Addition (+) <br>
2) Subtraction (-) <br>
3) Division (/) <br>
4) Multiplication (*) <br>
5) Exponent (**) <br>
6) Remainder (%) <br>
7) Floor Division (//) <br>


```python
# In the below code, we are using "Addition" Arithmetic Operator between two values
5 + 6
```




    11




```python
# In the below code, we are using "Subtraction" Arithmetic Operator between two values

5 - 6
```




    -1




```python
# In the below code, we are using "Division" Arithmetic Operator between two values

6.6 / 2.2
```




    2.9999999999999996




```python
# In the below code, we are using "Multiplication" Arithmetic Operator between two values

5 * 6
```




    30




```python
# In the below code, we are using "Exponent" Arithmetic Operator between two values

3 ** 4
```




    81




```python
# In the below code, we are using "Exponent" Arithmetic Operator between two values

2 ** 3
```




    8




```python
# In the below code, we are using "Remainder" Arithmetic Operator between two values

7 % 3
```




    1




```python
# In the below code, we are using "Remainder" Arithmetic Operator between two values

8 % 3
```




    2




```python
# In the below code, we are using "Remainder" Arithmetic Operator between two values

9 % 3
```




    0



<b>Working of Floor divison Operator:</b> <br>
Step 1) Normal divide and get the output <br>
Step 2) Find the integer value closest to the output and less than the output <br>


```python
# In the below code, we are using "Floor Division" Arithmetic Operator between two values

7 // 3
```




    2




```python
# In the below code, we are using "Floor Division" Arithmetic Operator between two values

8 // 3
```




    2




```python
# In the below code, we are using "Floor Division" Arithmetic Operator between two values

-10 // 3
```




    -4



# 2) Comparison Operators


<b>Types of Comparison Operators </b> <br>
1) Equal to (==) <br>
2) Not equal to (!=) <br>
3) Less than (<) <br>
4) Less than or equal to (<=) <br>
5) Greater than (>) <br>
6) Greater than or equal to (>=) <br>

<b>Comparison operators are used to compare two values</b>

# 1) Equal to (==)


<b> Working of "Equal to" Operator: </b> <br>
If the two values are equal we get a output of True, or else we get output of False


```python
4 == 7
```




    False




```python
4 == 4.0
```




    True




```python
4 == 'apple'
```




    False



# 2) Not equal to (!=)


<b> Working of "Not Equal to" Operator: </b> <br>

If the two values are equal we get a output of False, or else we get of True


```python
4 != 7
```




    True




```python
4  != 4.0
```




    False




```python
4 != 'apple'
```




    True



# 3) Less than (<)


<b> Working of "Less than" Operator: </b> <br>

If the value on the left is less than the value on the right, then we get a output of True. On the other hand, then we will get a output of False


```python
4 < 7
```




    True



<b>NOTE: </b>In "less than" comparison operator we can compare values of different types.However, we cannot compare string with a non-string values. String values can be compared with string values only


```python
4 < 5.0
```




    True




```python
4 < 'apple'
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-21-60a81080431e> in <module>
    ----> 1 4 < 'apple'
    

    TypeError: '<' not supported between instances of 'int' and 'str'


<b>Comparing string with a string value:</b> <br> 
1) We can only compare strings, character by character <br>
2) While comparing character by character we have to compare their ASCII values. <br>
3) If the ASCII value of the character on the left is less than the ASCII value of the character on the right, then we get ouput of True, on the other hand, we get a output of False. <br>
4) We cannot compare characters that are exactly the same. We can only compare characters that are different then each other <br>

<b>In the below example, first two characters of both the strings are the same, so we cannot compare them. The third character of both the strings are different, so we can compare them. On comparing the third characters we find out that the ASCII value of the character of the string on the LHS is 116, while the ASCII value of the character of the string on the RHS is 108. Since 116 is not less than 108, we get a result of False. </b>


```python
"bat" < "ball"
```




    False




```python
ord('t')
```




    116




```python
ord('l')
```




    108



<b>In the below example, first three characters of both the strings are the same, so we cannot compare them. So we will compare the fourth characters. We observe that the string on the LHS does not have a fourth character, we will assume a ASCII value of 0, while the ASCII value of the character of the string on the RHS is 116. Since 0 is less than 116, we get a result of True. </b>


```python
'bat' < 'batter'
```




    True




```python
ord('t')
```




    116



<b>In the below example, first two characters of both the strings are the same, so we cannot compare them. The third character of both the strings are different, so we can compare them. On comparing the third characters we find out that the ASCII value of the character of the string on the LHS is 32, while the ASCII value of the character of the string on the RHS is 116. Since 32 is less than 116, we get a result of True. </b>


```python
'bat ' < 'batter'
```




    True




```python
ord(' ')
```




    32




```python
ord('t')
```




    116



# 4) Less than or equal to (<=)


<b> Working of "Less than or equal to" Operator: </b> <br>

If the value on the left  is less than or equal to the value on the right, then we get a output of True. On the other hand, then we will get a output of False


```python
4 < 4
```




    False




```python
4 <= 4
```




    True



<b>NOTE: </b>In "less than or equal to" comparison operator we can compare values of different types.However, we cannot compare string with a non-string values. String values can be compared with string values only


```python
4 <= 'apple'
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-33-a5ff18b20a7c> in <module>
    ----> 1 4 <= 'apple'
    

    TypeError: '<=' not supported between instances of 'int' and 'str'



```python
4 <= 4.9
```




    True



<b>Comparing string with a string value:</b> <br> 
1) We can only compare strings, character by character <br>
2) While comparing character by character we have to compare their ASCII values. <br>
3) If the ASCII value of the character on the left is less than the ASCII value of the character on the right, then we get ouput of True, on the other hand, we get a output of False. <br>
4) We cannot compare characters that are exactly the same. We can only compare characters that are different then each other <br>

<b>In the below example, first character of both the strings are the same, so we cannot compare them. The second character of both the strings are different, so we can compare them. On comparing the second characters we find out that the ASCII value of the character of the string on the LHS is 97, while the ASCII value of the character of the string on the RHS is 101. Since 97 is less than or equal to 101, we get a result of True. </b>


```python
'sachin' <= 'sehwag'
```




    True




```python
ord('a')
```




    97




```python
ord('e')
```




    101



# 5) Greater than (>)


<b> Working of "Greater than" Operator: </b> <br>

If the value on the left is greater than the value on the right, then we get a output of True. On the other hand, then we will get a output of False


```python
5 > 3
```




    True




```python
5 > 7
```




    False



<b>NOTE: </b>In "greater than" comparison operator we can compare values of different types.However, we cannot compare string with a non-string values. String values can be compared with string values only


```python
4 > 5.9
```




    True




```python
'apple' > 7
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-43-156265bbc735> in <module>
    ----> 1 'apple' > 7
    

    TypeError: '>' not supported between instances of 'str' and 'int'


<b>In the below example, first five characters of both the strings are the same, so we cannot compare them. The sixth character of both the strings are different, so we can compare them. On comparing the sixth character we find out that the ASCII value of the character of the string on the LHS is 36, while the ASCII value of the character of the string on the RHS is 115. Since 36 is not greater than 115, we get a result of False. </b>


```python
'rohit$' > 'rohitsharma'
```




    False




```python
ord('$')
```




    36




```python
ord('s')
```




    115



<b>In the below example, first character of both the strings is different, so we can compare them. On comparing the first character we find out that the ASCII value of the character of the string on the LHS is 114, while the ASCII value of the character of the string on the RHS is 82. Since 114 is greater than 82, we get a result of True. </b>


```python
'rohit' > 'Rohit'
```




    True




```python
ord('r')
```




    114




```python
ord('R')
```




    82



# 6) Greater than or equal to (>=)

<b> Working of "Greater than or equal to" Operator: </b> <br>

If the value on the left is greater than or equal to the value on the right, then we get a output of True. On the other hand, then we will get a output of False


```python
4 > 4
```




    False




```python
4 >= 4
```




    True



<b>NOTE: </b>In "greater than or equal to" comparison operator we can compare values of different types.However, we cannot compare string with a non-string value. String values can be compared with string values only


```python
4  >= 5.0
```




    False




```python
'aPPLE' >= 67
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-53-e19245834eee> in <module>
    ----> 1 'aPPLE' >= 67
    

    TypeError: '>=' not supported between instances of 'str' and 'int'


<b>In the below example, first five characters of both the strings are the same, so we cannot compare them. The sixth character of both the strings are different, so we can compare them. On comparing the sixth character we find out that the ASCII value of the character of the string on the LHS is 32, while the ASCII value of the character of the string on the RHS is 50. Since 32 is not greater than or equal to 50, we get a result of False. </b>


```python
'Rohit Sharma' >= 'Rohit28Sharma'
```




    False




```python
ord(' ')
```




    32




```python
ord('2')
```




    50



# 3) Logical Operators

<b>Logical operators are used to work with boolean values</b>

1) and : <br>
  &emsp;&emsp; a) Is used to work with two boolean values  <br>
   &emsp;&emsp;  b) If both the boolean values are equal to True, then the output will be True. Or else the output will be False.  <br>
2) or:  <br>
   &emsp;&emsp;  a) Is used to work with two boolean values  <br>
 &emsp;&emsp;   b) If atleast one of the two boolean values are equal to True, then the output will be True. Or else the output will be False.  <br>
3) not  <br>
  &emsp;&emsp;   a) Is used to work with one boolean value only  <br>
  &emsp;&emsp;   b) Gives the opposite of the specified boolean value  <br>

# 1) and


```python
# In the below code, since both the boolean value are not equal to True, the "and" operator will give a result of False
True and False
```




    False




```python
# In the below code, since both the boolean value are not equal to True, the "and" operator will give a result of False

False and False
```




    False




```python
# In the below code, since both the boolean value are not equal to True, the "and" operator will give a result of False

False and True
```




    False




```python
# In the below code, since both the boolean value are equal to True, the "and" operator will give a result of True

True and True
```




    True



# 2) or


```python
# In the below code, since atleast one of the boolean value is equal to True, the "or" operator will give a result of True

True or False
```




    True




```python
# In the below code, since atleast one of the boolean value is not equal to True, the "or" operator will give a result of False

False or False
```




    False




```python
# In the below code, since atleast one of the boolean value is equal to True, the "or" operator will give a result of True

False or True
```




    True




```python
# In the below code, since atleast one of the boolean value is equal to True, the "or" operator will give a result of True

True or True
```




    True



# 3) not


```python
# Not operator gives the opposite of the specified boolean value. 
not True
```




    False




```python
# Not operator gives the opposite of the specified boolean value. 

not False
```




    True




```python

```
