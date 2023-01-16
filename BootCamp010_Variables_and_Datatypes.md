# Variable

A variable is just a reference to a value. A variable does not contain the value.

 <b>Syntax for assigning a reference to a value: </b><br>

 variableName=Value 

<b>NOTE</b>: If there is space to the left and right side of the variableName, then that space will be ignored

<b>Points to follow, while creating variableNames</b> <br>
1) The first character of a variableName should be an alphabet of lower case (a-z), or it can be an alphabet of upper case (A-Z), or an underscore (_) <br>
2) All the characters of the variableName apart from the first character should be an alphabet of lower case (a-z), or it can be an alphabet of upper case (A-Z), or an underscore (_), or it can be a digit charcater(0-9) <br>
3) A variableName cannot have space within it. <br>
4) A variableName cannot have any special characters (!,@,$,#,%,^,&,etc.) <br>
5) A variableName is case sensitive (apple is not the same as Apple)


```python
#The variable created below, is not valid as the first rule for variable creation is not being followed

007bond=25
```


      File "<ipython-input-1-bf1173183aef>", line 1
        007bond=25
          ^
    SyntaxError: leading zeros in decimal integer literals are not permitted; use an 0o prefix for octal integers
    



```python
# The variable created below, is valid as all the five rules of variable creation are being followed

bond007=25
```


```python
# Printing the value referenced by the variable- 'bond007'

bond007
```




    25




```python
#The variable created below, is not valid as the fourth rule for variable creation is not being followed

Devi@=26
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-4-2dea4554d1bb> in <module>
    ----> 1 Devi@=26
    

    NameError: name 'Devi' is not defined



```python
# The variable created below, is valid as all the five rules of variable creation are being followed

Devi=26
```


```python
# The variable created below, is valid as all the five rules of variable creation are being followed

devi=27
```


```python
# Printing the value referenced by the variable- 'devi'

devi
```




    27




```python
# Printing the value referenced by the variable- 'Devi'

Devi
```




    26




```python
#The variable created below, is not valid as the third rule for variable creation is not being followed

Rohit Sharma=28
```


      File "<ipython-input-9-4164e7058332>", line 1
        Rohit Sharma=28
              ^
    SyntaxError: invalid syntax
    



```python
# The variable created below, is valid as all the five rules of variable creation are being followed

RohitSharma=28
```

If a Value does not have a reference in jupyter notebook, then the below 2 things will happen: <br>
1) The value will get printed automatically <br>
2) Value will get deleted automatically <br>


```python
# The below created value does not have a reference assigned to it

31
```




    31




```python
# The below created value does have a reference assigned to it

a=32
```


```python
# Printing the value referenced by the variable- 'a'

a
```




    33



# Types of Values

1) Integer <br>
2) Float <br>
3) String <br>
4) Boolean <br>

# 1) Integer


Integer is just a number without any decimal point


```python
# In the below code, we created a integer value 50

a=50
```


```python
type(a)
```




    int




```python
# In the below code, we created a integer value 0

b=0
```


```python
type(b)
```




    int




```python
# In the below code, we created a integer value -100

c=-100
```


```python
type(c)
```




    int



# 2) Float

Float is just a number with decimal point


```python
# In the below code, we created a float value -30.0

d=30.0
```


```python
type(d)
```




    float




```python
# In the below code, we created a float value 0.001

e=0.001
```


```python
type(e)
```




    float




```python
# In the below code, we created a float value -10.3

f=-10.3
```


```python
type(f)
```




    float



# 3) String


A string is just a collection of characters. Inorder to tell python that you have a collection of characters, you need to surround that collection with single quotes, double quotes, triple quotes. <br>
NOTE: The type of quote that you are starting with should match with the type of quote that you are ending it.


```python
# In the below code, we created a string value - rishabhpant

g="rishabhpant"
```


```python
type(g)
```




    str




```python
# In the below code, we created a string value - bond007

h='bond007'
```


```python
type(h)
```




    str




```python
# In the below code, we created a string value - dollar$

j='''dollar$'''
```


```python
type(j)
```




    str



<b> In the below code, the type of quote at the beginning of the string value is not matching with the type of quote at the end of the string value, because of which we would receive a error </b>


```python


k="apple'
```


      File "<ipython-input-36-7e321b2182e7>", line 1
        k="apple'
                 ^
    SyntaxError: EOL while scanning string literal
    


# 4) Boolean

True and False are called boolean values. The first character of the boolean value needs to be in uppercase, while the rest of the characters of your boolean value need to be in lower case.


```python
#The value created below is not a boolean,string,integer or float

x=true
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-37-fe79c7b8bd75> in <module>
    ----> 1 x=true
    

    NameError: name 'true' is not defined



```python
# The value created below is a boolean value
x=True
```


```python
type(x)
```




    bool




```python
#The value created below is not a boolean,string,integer or float

y=TruE
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-40-07774d5fa91d> in <module>
    ----> 1 y=TruE
    

    NameError: name 'TruE' is not defined



```python
# The value created below is a boolean value

y=True
```


```python
type(y)
```




    bool




```python
# The value created below is a boolean value

z=False
```


```python
type(z)
```




    bool



# Understanding immutability


```python
# Here we have created a value of 50 and assigned a reference of "z" to it
z=50
```

<b>Here we have created a value of 50 and assigned a reference of "z" to it. Now, the variable "z" which was previously referencing the value of 50, will now refer the value 51. The value 50 will not have any variable referencing it. </b>



```python

z=51
```


```python
z
```




    51



<b>NOTE: Integer, Float, String, Boolean are immutable types of values. That means you cannot do any change in them.</b>

# Type Conversion

# 1) Integer to other types of values


```python
# Here, we created a integer value of 50, and assigned a variable of "a" as a reference to it
a=50
```

<b>Conversion to float: </b><br>
1) Convert the value to a real number <br>
2) Convert the real number to a number with decimal <br>


```python
# Here, the value referenced by variable "a" is converted to float

a=float(a)
```


```python
a
```




    50.0




```python
b=-10
```


```python
# Here, the value referenced by variable "b" is converted to float

float(b)
```




    -10.0



<b>If a Value does not have a reference in jupyter notebook, then: </b><br>
1) The value will get printed automatically (while creating that value) <br>
2) Value will get deleted automatically <br>

<b>Conversion to string:</b> <br>
1) Surround the value with quotes(single quote) <br>


```python
c=100
```


```python
type(c)
```




    int




```python
# Here, the value referenced by variable "c" is converted to string

d=str(c)
```


```python
d
```




    '100'




```python

e=40
```


```python
# Here, the value referenced by variable "e" is converted to bool

bool(e)
```




    True




```python
f=0
```


```python
# Here, the value referenced by variable "f" is converted to bool

bool(f)
```




    False




```python
g=-40
```


```python
# Here, the value referenced by variable "g" is converted to bool

bool(g)
```




    True




```python
NOTE: In Numeric values, only 0 is insignificant, rest all numeric values are significant
```

# 2) Float to other types of values


```python
a=30.2
```


```python
type(a)
```




    float



<b>Conversion from float to integer: </b><br>
1) Remove the decimal point as well as the digits that come after the decimal point


```python
# Here, the value referenced by variable "a" is converted to integer

int(a)
```




    30




```python
b=30.9
```


```python
type(b)
```




    float




```python
# Here, the value referenced by variable "b" is converted to integer

int(b)
```




    30




```python
c=-40.987

```


```python
# Here, the value referenced by variable "c" is converted to integer

int(c)
```




    -40



<b>Conversion to string:</b><br>
1) Surround the value with quotes(single quote)


```python
d=90.99
```


```python
type(d)
```




    float




```python
# Here, the value referenced by variable "d" is converted to string

str(d)
```




    '90.99'




```python
e=0.01

```


```python
type(e)
```




    float




```python
# Here, the value referenced by variable "e" is converted to boolean

bool(e)
```




    True




```python
f=0.00
```


```python
type(f)
```




    float




```python
# Here, the value referenced by variable "f" is converted to boolean

bool(f)
```




    False




```python
g=-30.9
```


```python
# Here, the value referenced by variable "g" is converted to boolean

bool(g)
```




    True




```python
q=12.87

```


```python
type(q)
```




    float




```python
Conversion from float to integer:
1) Remove the decimal point as well as the digits that come after the decimal point
```


```python
# Here, the value referenced by variable "q" is converted to integer

int(q)
```




    12




```python
q
```




    12.87



# 3) String to other types of values


```python
a="apple"
```

<b>Inorder to convert string to integer, we need to follow the below step:</b><br>
1) Remove the quotes



```python
type(a)
```




    str



<b>In the below code, we tried to convert a string value to integer. For that we need to remove the quotes. However even after removing the quotes, the resultant value was not a integer, hence python returns a error.</b>


```python

int(a)
```


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    <ipython-input-88-8b2ab3991dae> in <module>
    ----> 1 int(a)
    

    ValueError: invalid literal for int() with base 10: 'apple'



```python
b='50.9'
```


```python
type(b)
```




    str



<b>In the below code, we tried to convert a string value to integer. For that we need to remove the quotes. However even after removing the quotes, the resultant value was not a integer, hence python returns a error.</b>


```python
int(b)
```


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    <ipython-input-91-07ae29993d50> in <module>
    ----> 1 int(b)
    

    ValueError: invalid literal for int() with base 10: '50.9'



```python

c='50'
```


```python
type(c)
```




    str



<b>Inorder to convert string to integer, follow the below step:</b><br>
1) Remove the quotes



```python
# Here, the value referenced by variable "c" is converted to integer

int(c)
```




    50



<b>Conversion from string to float:</b><br>
1) Convert the value to a real number (remove the quotes) <br>
2) Convert the real number to a number with decimal <br>


```python
d='apple'
```


```python
type(d)
```




    str



<b>In the below code, we tried to convert a string value to float. For that we followed the two steps. However even after following the two steps, the resultant value was not a float, hence python returns a error.</b>


```python
float(d)
```


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    <ipython-input-97-375ddbb813ae> in <module>
    ----> 1 float(d)
    

    ValueError: could not convert string to float: 'apple'



```python
e='30'
```


```python
type(e)
```




    str




```python
# Here, the value referenced by variable "e" is converted to float

float(e)
```




    30.0




```python
f='30.9'
```


```python
type(f)
```




    str



<b>Conversion from string to float:</b><br>
1) Convert the value to a real number (remove the quotes)<br>
2) Convert the real number to a number with decimal<br>


```python
float(f)
```




    30.9




```python
x='apple'
```


```python
type(x)
```




    str




```python
# Here, the value referenced by variable "x" is converted to bool

bool(x)
```




    True




```python
len(x)
```




    5




```python
y=' '
```


```python
type(y)
```




    str




```python
len(y)
```




    1




```python
# Here, the value referenced by variable "y" is converted to bool

bool(y)
```




    True




```python
z=''
```


```python
type(z)
```




    str




```python
len(z)
```




    0




```python
# Here, the value referenced by variable "z" is converted to bool

bool(z)
```




    False



<b>NOTE:</b><br>1) In Numeric values, only 0 is insignificant, rest all numeric values are significant <br>
     2) In String, only empty string is insignificant, rest all string values are significant <br>

# 4) Boolean to other types of values



```python
a=True
```


```python
type(a)
```




    bool




```python
# Here, the value referenced by variable "a" is converted to integer


int(a)
```




    1




```python
a
```




    True



<b>Inorder to convert a boolean value to a float value, you have to follow the below steps:<br></b>
1) Convert the value to a real number <br>
2) Convert the real number to a number with decimal


```python
# Here, the value referenced by variable "a" is converted to float


float(a)
```




    1.0




```python
a
```




    True



<b>Inorder to convert a boolean value to a string value, you have to follow the below step:<br></b>
1) Surround the value with quotes(single quote)<br>


```python
# Here, the value referenced by variable "a" is converted to string


str(a)
```




    'True'




```python
b=False
```


```python
type(b)
```




    bool




```python
# Here, the value referenced by variable "b" is converted to integer

int(b)
```




    0




```python
b
```




    False




```python
# Here, the value referenced by variable "b" is converted to float

float(b)
```




    0.0




```python
b
```




    False




```python
# Here, the value referenced by variable "b" is converted to string

str(b)
```




    'False'




```python

```
