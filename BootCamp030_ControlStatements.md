#  Statements

<b>Types of Statements: </b><br>
1) Control Statements <br>
2) Error-Handling Statements

# Control Statements

<b>Control statements help us to control the execution of code</b>

<b>Syntax for creating "if" control statement </b><br>

if booleanValue/ CodeThatGIvesBooleanValue :
    #blockOfCode

<b>Syntax for creating "elif" control statement </b><br>

elif booleanValue/ CodeThatGIvesBooleanValue :
    #blockOfCode

<b>Syntax for creating "else" control statement </b><br>

else:
    #blockOfCode

<b>How to create blockOfCode </b><br>
1) We need to have atleast line of code in the blockOfCode <br>
2) All the lines of code in the blockOfCode need to have some space before it <br>
3) All the lines of code in the blockOfCode need to have same space before it <br>

<b>NOTE: In one code structure, only one blockOfCode will execute </b>

<b>Important Points w.r.t. Control Statements </b><br>
1) if   -- a) The "if" control statement is mandatory <br>
   &emsp; &emsp; &emsp;        b) The blockOfCode inside the "if" control statement will only execute only if the booleanValue obtained next to the "if" keyword is equal to True <br>
   &emsp; &emsp; &emsp;        c) The "if" control statement can only be written once in one code structure <br>
2) elif -- a) The "elif" control statement is not mandatory <br>
   &emsp; &emsp; &emsp;        b) The blockOfCode inside the "elif" control statement will only execute only if the booleanValue obtained next to the "elif" keyword is equal to True <br>
   &emsp; &emsp; &emsp;        c) The "elif" control statement can be written multiple times in one code structure <br>
3) else -- a) The "else" control statement is not mandatory <br>
   &emsp; &emsp; &emsp;        b) The blockOfCode inside the "else" control statement will only execute only if none of the previous blocksOfCode have not been executed <br>
   &emsp; &emsp; &emsp;        c) The "else" control statement can be written once in one code structure <br>


```python
room="hall"
```

<b>In the below code structure, we have two blocks of code. The execution will not go inside the blockOfCode of the "if-statement" as the booleanValue next to the "if" keyword is not equal to True. The execution will go inside the blockOfCode of the "elif- statement" as the booleanValue next to the "elif" keyword is equal to True. </b>


```python
if room=="bedroom":
    print("I am in bedroom")
elif room=="hall":
    print("I am in hall")
```

    I am in hall
    


```python
room="kitchen"
```

<b>In the below code structure, we have three blocks of code. The execution will not go inside the blockOfCode of the "if-statement" as the booleanValue next to the "if" keyword is not equal to True. The execution will not go inside the blockOfCode of the "elif- statement" as the booleanValue next to the "elif" keyword is not equal to True. The execution will go inside the blockOfCode of the "else-statement", as none of the previous blocksOfCode have been executed. </b>


```python
if room=="bedroom":
    print("I am in bedroom")
elif room=="hall":
    print("I am in hall")
else:
    print("I am in some other room")
```

    I am in some other room
    

<b>In the below code structure, we have four blocks of code. The execution will not go inside the blockOfCode of the "if-statement" as the booleanValue next to the "if" keyword is not equal to True. The execution will not go inside the blockOfCode of the first "elif- statement" as the booleanValue next to the "elif" keyword is not equal to True. The execution will go inside the blockOfCode of the third "elif-statement", as the booleanValue next to the "elif" keyword is equal to True. </b>


```python
if room=="bedroom":
    print("I am in bedroom")
elif room=="hall":
    print("I am in hall")
elif room=="kitchen":
    print("I am in kitchen")
else:
    print("I am in some other room")
```

    I am in kitchen
    


```python

```


```python

```


```python

```

<b>The below code structure is not valid, as we have not mentioned a "if-statement"</b>


```python
elif room=="hall":
    print("I am in hall")
else:
    print("I am in some other room")
```


      File "<ipython-input-14-c8b9762021f4>", line 1
        elif room=="hall":
        ^
    SyntaxError: invalid syntax
    



```python

```
