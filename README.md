Download Link: https://assignmentchef.com/product/solved-cs320-homework-1-integers
<br>
<h2>1       Integers</h2>

<ol>

 <li>Define the function dollar2won, which consumes an integer number of dollars and produces the won equivalent. Use the won/dollar conversion rate of 1100 won per dollar.</li>

 <li>Write the function volumeOfCuboid, which consumes three integer numbers denoting lengths of three sides and produces the volume of the cuboid.</li>

 <li>Write the function isEven, which consumes an integer number and returns whether the number is even.</li>

 <li>Write the function isOdd, which consumes an integer number and returns whether the number is odd.</li>

 <li>Write the function gcd, which consumes two integer numbers and returns the greatest common divisor of them.</li>

 <li>Write the function lcm, which consumes two integer numbers and returns the least common multiple of them.</li>

</ol>

<h2>2          Pattern Matching</h2>

You have a type COURSE, which is either CS320, CS311, or CS330. CS320 has two members: quiz for a number of quizzes and homework for a number of programming assignments. CS311 has one member: homework which is a number too. CS330 has two members: projects for a number of projects and homework for a number of programming assignments.

<table width="673">

 <tbody>

  <tr>

   <td width="673">trait COURSE case class CS320(quiz: Int, homework: Int) extends COURSE case class CS311(homework: Int) extends COURSEcase class CS330(projects: Int, homework: Int) extends COURSE</td>

  </tr>

 </tbody>

</table>

<ol>

 <li>Define the function numOfHomework, which consumes a course and produces the number of programming assignments for the given course.</li>

 <li>Define the function hasProjects, which consumes a course and produces true only when the given course is CS330 with more than or equal to two projects, otherwise produces false.</li>

</ol>

<h2>3       List</h2>

<ol>

 <li>Define the function namePets, which consumes a list of pets and produces a corresponding list of pets with names; it names all occurrences of dog with happy, cat with smart, pig with pinky, and keeps the other pets as unnamed. For example,</li>

</ol>

namePets(List(“dog”, “tiger”, “cat”)) == List(“happy”, “tiger”, “smart”)

1

<ol start="2">

 <li>Generalize namePets to the function giveName. The new function consumes two strings, called old and new. It produces a function that gets a list of strings and replaces all occurrences of old by new in the list. For example,</li>

</ol>

namePets(List(“dog”, “tiger”, “cat”)) == List(“happy”, “tiger”, “smart”) val nameBears: List[String] =&gt; List[String] = giveName(“bear”, “pooh”) nameBears(List(“pig”, “cat”, “bear”)) = List(“pig”, “cat”, “pooh”)