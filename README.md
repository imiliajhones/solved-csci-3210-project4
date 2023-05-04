Download Link: https://assignmentchef.com/product/solved-csci-3210-project4
<br>
<strong>Goal: To learn how to use functional programming language to solve a problem.</strong>

<strong>Description:</strong>

In this assignment, you are required to write functions specified below in Scheme, one of the functional programming languages.

<ul>

 <li>Write a Scheme function <strong><em>sphereVolume(r)</em></strong> that given the radius r of a sphere, computes its volume as 4/3 * 3.14 * r * r * r.</li>

 <li>Write a Scheme function <strong><em>power(A, B)</em></strong> that takes two numeric parameters, A and B, and returns A raised to the B power.</li>

 <li>Write a Scheme function <strong><em>countZero(list)</em></strong> that returns the number of zeros in a given <strong>simple list</strong> of numbers.</li>

 <li>Write a Scheme function <strong><em>reverse(list)</em></strong> that returns the reverse of its <strong>simple list </strong></li>

 <li>Write a Scheme function <strong><em>findEnds(list) </em></strong>that takes a <strong>simple list</strong> of numbers as its parameter and returns the largest and smallest numbers in the list.</li>

 <li>Write a Scheme function <strong><em>replace(atom1, atome2, list)</em></strong> that takes two atoms and <strong>a list</strong> as parameters and returns a list identical to the parameter list except all occurrences of the first given atom in the list are replaced with the second given atom, no matter how deeply the first atom is nested.</li>

</ul>

Note: A simple list is a list such that none of its element is a list. For example, ‘(1 2 3) is a simple list, while ‘((1 2) 3) is not a simple list.

To avoid typing long lists at the command line, I suggest you create a few sample arguments in files:

&gt; (load “my_lists”)

&gt; (countZero list1)

where the file my_lists contains the definition

(define list1 ‘(1 9 0 12 0 30 50 0))

<strong>Important</strong>: <em>you are required to use <strong>only</strong> the functional features of Scheme; functions with an exclamation point in their names (e.g. </em><em>set!) and input/output mechanisms other than </em><em>load and the regular read-eval-print loop are not allowed. (You may find imperative features useful for debugging. That’s ok, but get them out of your code before you hand anything in.)</em>

<strong>Requirement</strong>:

<ul>

 <li>All functions should be put within the same source file.</li>

 <li>The signature of each function (including function name and order of parameters) must match the given signature.</li>

</ul>

<strong>IDE: Dr. Racket</strong>

Dr. Racket is the IDE we are going to use. The software is free and can be downloaded from: <u>http://racket-lang.org/download/</u>. It supports different platforms such as Windows, Mac, or Linux. You can also use Dr. Racket on shemp.cs.mtsu.edu. Here is how it looks like:

The top window is the editor, and bottom half is the command line window. After completing coding, click the Run button on the menu bar, and if there is no syntax error, functions defined in the code can be invoked from the command line window. The following pictures gives an example: after typing <u>(list-sum ‘(1 2 3 4 5 6 7 8))</u> and press ENTER, the function is called and result is diplayed.

<strong>Project Tips</strong>

The detailed manual of Racket can be found at: <u>http://docs.racket-lang.org/reference/index.html</u>

You don’t need read through the whole reference, just find information you need such as how to define/invoke functions, how to manipulate lists, and how to use conditional statements.

For these two functions, using recursive solution is properly easier. Make sure you cover all base cases (for example, function arguments are lists, empty lists).

Some useful functions are provided below with a brief description:

<ul>

 <li><strong>(list? listvalue ) </strong>returns true (#t) if listvalue is a list value; otherwise false (#f)</li>

 <li><strong>(null? listvalue) </strong>returns true if listvalue is an empty list, otherwise false</li>

 <li><strong>(equal? value1 value2) </strong>returns true if value1 is equal to value2, otherwise false</li>

 <li><strong>(&gt; value1 value2) </strong>returns true if value1 greater than value2, otherwise false. (similar for &gt;)</li>

 <li><strong>(- value1 value2) </strong>returns the result of value1 – value2 (similar for +)</li>

 <li><strong>(length listvalue) </strong>returns the number of elements in the listvalue.</li>

 <li><strong>(list-tail listvalue pos) </strong>returns the list after the first pos elements of listvalue.</li>

 <li><strong>(drop-right listvalue pos) </strong>returns a fresh list whose elements are the prefix of listvalue, dropping its poslength tail.</li>

 <li><strong>(list-ref listvalue pos) </strong></li>

</ul>

Returns the element of listvalue at position pos, where the list’s first element is position 0.

<ul>

 <li><strong>(not boolvalue) </strong></li>

</ul>

Returns true if boolvalue is false; otherwise false.

For detailed information on list operations, please refer to the page below:

<u>http://docs.racket-lang.org/reference/pairs.html#%28part._.List_.Operations%29 </u><strong>How to submit?</strong>

<ul>

 <li>Copy the rubric4.doc and your source program to the project4 folder in your individual repository. Edit the file to put your name.</li>

 <li>Commit the whole project2 folder to the server. Make sure the folder contains your source program.</li>

 <li><strong>Any commit of the project after the deadline is considered as cheating. If this happens, the latest version before the deadline will be graded, and you may receive up to 50 points deduction.</strong></li>

 <li><strong>No hard copy needed</strong></li>

</ul>