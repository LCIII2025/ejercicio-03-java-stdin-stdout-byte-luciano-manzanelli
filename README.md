# Challenge "Standard Input/Output" - Playing with byte data type

Most challenges require you to read input from 
<a href="https://en.wikipedia.org/wiki/Standard_streams#Standard_input_.28stdin.29">stdin</a>
(standard input) and write output to
<a href="https://en.wikipedia.org/wiki/Standard_streams#Standard_output_.28stdout.29">stdout</a> 
(standard output).

One popular way to read input from stdin is by using the 
<a href="https://docs.oracle.com/javase/8/docs/api/java/util/Scanner.html">Scanner</a>
class and specifying the Input Stream as 
System.in. For example:

```
Scanner scanner = new Scanner(System.in);
String myString = scanner.next();
int myInt = scanner.nextInt();
scanner.close();

System.out.println("myString is: " + myString);
System.out.println("myInt is: " + myInt);
```

The code above creates a Scanner object named **_scanner_** and uses it 
to read a String and an int. It then closes the Scanner object because 
there is no more input to read, and prints to stdout using 
System.out.println(String). So, if our input is:

```
Hi 5
```

Our code will print:

```
myString is: Hi
myInt is: 5
```

Alternatively, you can use the 
<a href="https://docs.oracle.com/javase/8/docs/api/java/io/BufferedReader.html">BufferedReader class</a>.

More information about primitive data types can be found
[here](https://docs.oracle.com/en/java/javase/17/docs/api/java.compiler/javax/lang/model/type/PrimitiveType.html).


## Task

In this challenge, you must read **_3_** **byte** from stdin and then print 
them to stdout. Each **byte** must be printed on a new line. 
To make the problem a little easier, a portion of the code is provided 
for you in the editor below.

## Input Format

There are **_3_** lines of input, and each line contains a single **byte**.

### Sample Input

```
42
100
125
```

### Sample Output

```
42
100
125
```