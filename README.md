Download Link: https://assignmentchef.com/product/solved-comp1210-activity5-conditionals-and-loops
<br>
By the end of this activity you should be able to do the following:

<ul>

 <li>Gain a further understanding of <em>if</em> and <em>if-else</em> statements</li>

 <li>Understand the basics of <em>while</em> statements (a.k.a., <em>while loops</em>)</li>

 <li>Introduces the ArrayList class (java.util.ArrayList) <strong>Description: </strong></li>

</ul>

In this activity you will create a <strong>NumberOperations</strong> class which will hold an integer value and provide methods to perform various operations on that value.  You will also download and modify a class called <strong>NumberOpsDriver </strong>which creates an ArrayList object and then reads in a value from the keyboard.  While the value is not zero, the program creates an instance of the NumberOperations class for the value, adds the instance to the ArrayList, and then reads the next value from the keyboard.

<strong>             </strong>

<strong>Directions: </strong>

<strong>Part 1: NumberOperations: Method Stubs (a.k.a. skeleton code)  </strong>

<u>Don’t forget to add your Javadoc comments; the class, constructor and each method will need one</u>.

<ul>

 <li>Create a class called NumberOperations with an instance variable called <em>number</em> of type <em>int</em>.</li>

</ul>




<ul>

 <li>Add method <u>stubs</u> for the following methods<strong>. The first two are given; do the rest on your own</strong>. o The constructor takes an int parameter called numberIn

  <ul>

   <li>oddsUnder: takes no parameters; returns a String o powersTwoUnder: takes no parameters; returns a String</li>

   <li>isGreater: takes an int parameter called compareNumber; returns an int o toString: takes no parameters; returns a String</li>

  </ul></li>

</ul>




Compile NumberOperations and run the following in interactions. <strong>Do not continue until your program compiles and the following code runs without runtime errors in interactions.  Note that return values will be the placeholder values in the “stubbed” methods. </strong>

Ï¼ÏÏNumberOperations numOps = new NumberOperations(5);

Ï¼ÏÏString s1 = numOps.oddsUnder();

Ï¼ÏÏString s2 = numOps.powersTwoUnder();

Ï¼ÏÏint n1 = numOps.isGreater(2);

Ï¼ÏÏString s3 = numOps.toString();




<strong>             </strong>

<strong>Part 2: NumberOperations: Constructor, getValue, and toString </strong>

<ul>

 <li>In your constructor, add code that will set the value of <em>number</em> to <em>numberIn</em>.</li>

 <li>In your getValue method, delete the placeholder return and return the value of <em>number</em>.</li>

 <li>Replace the placeholder return in the toString method with the following code:</li>

</ul>




[<em>Note that the result of concatenating number, which is an int, with an empty String is a String</em>.] Compile NumberOperations and run the following code in the interactions pane. <strong>Do not continue until the following code runs without error in interactions.</strong>




Ï¼ÏÏNumberOperations numOps = new NumberOperations(5);

Ï¼ÏÏnumOps.getValue()

ÏÏÏÏ5

Ï¼ÏÏnumOps // displays the toString return value

<h1>ÏÏÏÏ5ÏÏÏ</h1>







<strong>Part 3: NumberOperations: oddsUnder Method – Returns a String containing the positive odd integers less than the value of number. </strong>

<ul>

 <li>Create a local variable in oddsUnder called <em>output</em> and initialize it to an empty string literal</li>

 <li>Add a local int variable <em>i </em>and a while loop that will iterate through the loop as long as the value of <em>i </em>is less than the value of <em>number</em>.</li>

 <li><u>Inside of the above loop</u>, add code that will concatentate the value of<em> i </em>if it is an odd number. Also increment the value of <em>i </em>during each iteration of the loop.</li>

 <li>After the loop, add code to <strong>return the value of output</strong>.</li>

</ul>




Compile NumberOperations and run the following code in the interactions pane. <strong>Do not continue until the following code runs without error in interactions. </strong>




Ï¼ÏÏNumberOperations numOps = new NumberOperations(9);

Ï¼ÏÏnumOps.oddsUnder()

ÏÏÏÏ1  3  5  7




<strong> </strong>

<strong>Part 4A: NumberOperations: powersTwoUnder Method – returns a String containing the positive powers of two less than the value of number. </strong>

<ul>

 <li>Create a local String variable in powersTwoUnder called <em>output</em> and initialize it to an empty string literal as you did in oddsUnder.</li>

 <li>Create another local variable of type int called <em>powers</em> and initialize its value to 1.</li>

 <li>Add a while loop that will iterate through each number up until the value of <em>number</em>.</li>

</ul>




<ul>

 <li>Inside of the while loop, add code that will concatentate the value of powers to output if it is a power of 2 and then calculate the next power of two (the comments below are optional).</li>

</ul>




<ul>

 <li>After the loop, add code to <strong>return the value of output</strong>.</li>

</ul>




Compile NumberOperations and run the following code in the interactions pane. <strong>Do not continue until the following code runs without error in interactions. </strong>




Ï¼ÏÏNumberOperations numOps = new NumberOperations(20);

Ï¼ÏÏnumOps.powersTwoUnder()

<h1>ÏÏÏÏ1   2   4   8   16    ÏÏÏ</h1>




<strong>Part 4B: NumberOperations: isGreater Method  </strong>

<ul>

 <li>Delete the placeholder return from isGreater and add code that will return 1 if number is greater than compareNumber, -1 if number is less than compareNumber, or 0 if the numbers are equal.</li>

</ul>










Compile NumberOperations and run the following code in the interactions pane. <strong>Do not continue until the following code runs without error in interactions. </strong>

<strong> </strong>

<table width="590">

 <tbody>

  <tr>

   <td width="590">Ï¼ÏÏNumberOperations numOps = new NumberOperations(10);Ï¼ÏÏnumOps.isGreater(2) ÏÏÏÏ1Ï¼ÏÏnumOps.isGreater(15) ÏÏÏÏ-1Ï¼ÏÏnumOps.isGreater(10)ÏÏÏÏ0Ï</td>

  </tr>

 </tbody>

</table>

<strong>Part 5A: NumberOpsDriver Class </strong>

<ul>

 <li>Download the driver program called <em>java</em> and then add the indicated code (described in the // comments) so that it does the following: prompts the users for a list of numbers (ints) separated by a space followed by the number 0; reads the first number in the list; enters a loop and while the number is not 0, creates a NumberOperations object, adds the NumberOperations object to an ArrayList called <strong><em>numOpsList</em></strong>, then read the next number in the list (i.e., iterates through the loop). Once the value of 0 is read from the list, the loop terminates.  Now using a second while loop, print out each NumberOperations object in the ArrayList along with its “odds under” and its “powers of 2 under”.  Example output:</li>

</ul>

<table width="639">

 <tbody>

  <tr>

   <td width="639">MM«M —-jGRASP exec: java NumberOpsDriverMM§MEnter a list of positive integers separated with a space followed by 0:¼¼§M12 9 17 0MM§MFor: 12MM§M   Odds under: 1  3  5  7  9  11MM§M   Powers of 2 under:   1  2  4  8MM§MFor: 9MM§M   Odds under: 1  3  5  7MM§M   Powers of 2 under:   1  2  4  8MM§MFor: 17MM§M   Odds under: 1  3  5  7  9  11 13 15MM§M   Powers of 2 under:   1  2  4  8  16  MM§MMM©M —-jGRASP: operation complete. </td>

  </tr>

 </tbody>

</table>




<strong>Part 5B: Runing NumberOpsDriver in the Canvas </strong>

<ul>

 <li>Download the jGRASP canvas file <em>jgrasp_canvas.xml</em> and save in the folder with your source files for this activity.</li>

 <li>Now click the Run in Canvas button on the desktop toolbar.  After the canvas file opens, click the Play button  and you should see the viewers for Scanner <em>in</em> and ArrayList <em>numOpsList</em> become active although empty.  After entering the input as shown in the example above, you should see the values in the Scanner <em>in</em>  As the each value is read in by your program you should see the Scanner viewer move through the values in its buffer.  And as your program</li>

</ul>

creates each NumberOperations object for the value and adds the NumberOperations object to ArrayList <em>numOpsList</em>, you should <em>numOpsList</em> viewr updated in the canvas.  The figure at right shows the<strong> canvas after two values have been read in and two NumberOperations objects have been created and added to the ArrayList <em>numOpsList</em></strong>.

<ul>

 <li>As the program plays you should see the viewer for <em>output</em> which is a local variable in the oddsUnder() and powersTwoUnder() methods. Note that the “Scope” for <em>output</em> has been set to “None” by using the viewer pull-down menu  and selecting <strong>Scope</strong> and then <strong>None</strong>.  This allows the viewer to display the value of <em>scope</em> regardless of which local variable it is.  The figure at right shows the canvas while the program is executing the powersUnder() method on the third element of numOpsList (i.e., the element at index 2).  The viewer for <em>output</em> shows the five powers of two numbers below 17.</li>

 <li>While running on the canvas, you can</li>

</ul>

pause  and then step  or step-in  as            appropriate to view the behavior of interest.

You can also stop the canvas and then run in canvas     and play           again.  To regulate the speed of the program in the canvas, decrease or increase the delay between steps using the Delay slider .

<ul>

 <li>You should experiment with running this program in the canvas until you are sure that you understand both the <em>NumberOperations</em> and <em>NumberOpsDriver</em> Since this activity introduces the <em>while statement</em>, you should pause the canvas and then single step through each of the while statements to ensure that you understand them.  In the main method, the first while statement reads in the values and the second one populates the ArrayList of NumberOperations objects.  You should also single step through each of the while loops in the oddsUnder() and powersTwoUnder() methods.</li>

</ul>







<strong>Web-CAT</strong> – After you have created the jGRASP project in the next section, you should submit your NumberOperations.java and NumberOpsDriver.java files to Web-CAT via the Web-CAT button on the project toolbar.