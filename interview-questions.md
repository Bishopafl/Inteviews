# General Knowledge Questions:

Please write your answers in the code blocks.

**NOTICE:** Some (but not all) questions may be easier to answer with code or pseudocode. As an example, all of these are an acceptable answer to the question "How do you iterate a variable in PHP?"

```
$number++;
```

```
num = num + 1
```

```
variable "num" now equals "num" + 1
```

-----------------------------------------------------------------------

## Section: PHP

1. How do you get information from a form that is submitted using the "get" method?

```
<?php 
    if(isset(_GET['submmit']) {
        $firstname = $_GET['firstname'];
        $lastname = $_GET['lastname'];
    } 
?>
```

2. What is the correct way to create a function in PHP?

```
<?php 
    function myNewFunction() {
        // code here
    }

?>
```

3. Name a method to output an array?

```
<?php var_dump($array); ?>
```

4. Which operator is used to check if two values are equal and of same data type?

```
The equality operator, used with double equal sign (==) compares numbers, strings, booleans, variables and functions
```

5. Which superglobal variable holds information about headers, paths, and script locations?

```
the $_SERVER superglobal variable holds information about headers, paths and scripts.
```

6. Explain how `static function` works in PHP class methods.

```
Static functions are associated with the class they are in and not the instance of the class they are referred from. If you use a static function, methods inside can be called directly without creating an instance of the class.
```


7. What is the commonly used library for database connections?

```
Portable Data Objects (PDO) library
```

8. What is the commonly used library for making requests?

```
HTTP methods GET & POST
```

9. What is PHP function strlen?

```
outputs the length of a string
```


## Section: SQL

For the below questions, assume you are using this table (named `Persons`):

| Id | FirstName | LastName  |
|----|-----------|-----------|
| 1  | Peter     | Jackson   |
| 2  | Adam      | Savage    |
| 3  | Linus     | Sebastian |
| 4  | Brent     | Spiner    |
| 5  | Doom      | Guy       |

1. How would you select just the first record and only the column `FirstName`?

```
SELECT FirstName FROM Persons WHERE Id = 1;
```

2. How would you select all the records where the `FirstName` is "Peter" and the `LastName` is "Jackson"?

```
SELECT * FROM Persons where FirstName = 'Peter' and LastName = 'Jackson';
```

3. How would you select all the records where the `LastName` starts with an "s"?

```
SELECT * FROM Persons WHERE LastName LIKE 's%';
```

4. How would you select all the records where the `FirstName` is alphabetically between "Brent" and "Linus"?

```
SELECT * FROM Persons WHERE LEFT(FirstName, 1) BETWEEN 'B' and 'L';
```

5. How would you insert the name "David Tennant"?

```
INSERT INTO Persons (FirstName, LastName) VALUES ('David', 'Tennant')
```

6. How would you change all the records where the `FirstName` is equal to "Peter" into "Samuel"?

```
UPDATE FirstName SET FirstName = 'Samuel' WHERE FirstName = 'Peter';
```

7. How would you delete the records where the `LastName` is "Sebastian"?

```
DELETE FROM Persons WHERE LastName = 'Sebastian';
```

8. How would you get the number of records in the `Persons` table?

```
SELECT COUNT(*) FROM Persons;
```

9. Give an example of how would you join 2 related tables together?

```
SELECT Persons.FirstName, Persons.LastName, Orders.OrderDate
FROM Orders
JOIN Persons ON Orders.Id=Persons.Id
```


## Section: Vanilla Javascript

1. How do you create a function in JavaScript?

```
<script>
function name(x,y,z) {
    // code
}
</script>
```

2. How do you call a function named "myFunction"?

```
var x = myFunction(x,y);

function myFunction(a,b){
    return a + b;
}
```

4. How to write an IF statement for executing some code if "i" is NOT equal to 5?

```
var x = 6;

if(x != 5) {
    // do something
}
```

5. How does a WHILE loop start?

```
text = ""; 
x = 1;
while (x < 6) {
    text += 'Number is ' + x;
}
document.write(text);
```

6. How does a FOR loop start?

```
for (i = 0; i < 6; i++) {
    text += i;
}
document.write(text);
```

7. How do you round the number 7.25, to the nearest integer?

```
Math.round(7.25);
```

8. What will the following code return: Boolean(10 > 9)

```
true
```

## Section: jQuery

1. Can jQuery animate() method can be used to animate ANY CSS property?

```
Only numeric values can be animated, like padding and margins.  Background colors cannot because they are strings
```

2. Which jQuery method is used to hide selected elements?

```
$("element").hide();
```

3. Which jQuery method is used to perform an asynchronous HTTP request?

```
$.ajax({foo:value, bar:value});
```

4. Look at the following selector: $("div p"). What does it select?

```
All paragraph elements within div elements

```


## Section: React

1. What is JSX?

```
it's an XML/HTML like syntax that React uses 
```

2. What triggers a render cycle?

```
Saving any changes in the code
```

3. What is a React Hook?

```
It's special function that lets you use components within React without using classes
```

4. Which method in a React Component should you override to stop the component from updating?

```
shouldComponentUpdate
```

5. Which method in a React Component is called after the component is rendered for the first time?

```
The contructor component
```

6. What happens when you call setState() inside render() method?

```
tells React that the component and it's children need to be re-rendered with the updated state.
```
