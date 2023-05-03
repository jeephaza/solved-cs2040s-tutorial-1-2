Download Link: https://assignmentchef.com/product/solved-cs2040s-tutorial-1-2
<br>
<h2>Java Review</h2>

At this point, most of you should be comfortable enough to work with Java. Let’s take some time to review a few concepts in Java so that we can limit our Java-related issues and, hence, focus on the algorithms when solving future Problem Sets.

<ul>

 <li>What is the difference between a class and an object? Illustrate with an example.</li>

 <li>Why does the main method come with a static modifier?</li>

 <li>Give an example class (or classes) that uses the modifier private incorrectly (i.e., the program will not compile as is, but would compile if private were changed to public).</li>

 <li>The following question is about Interfaces.</li>

</ul>

(d)(i) Why do we use interfaces?

(d)(ii) Give an example of using an interface.

(d)(iii) Can a method return an interface?

<ul>

 <li>Refer to java in Coursemology. Without running the code, predict the output of the main method. Can you explain the outputs? There should also be an interface for an animal, an interface for a player, and a player class that implements it.</li>

 <li>Can a variable in a parameter list for a method have the same name as a member (or static) variable in the class? If yes, how is the conflict of names resolved?</li>

</ul>

<h2>Problem 2.           Asymptotic Analysis</h2>

This is a good time for a quick review of asymptotic big-O notation. For each of the expressions below, what is the best (i.e. tightest) asymptotic upper bound (in terms of <em>n</em>)?

<table width="444">

 <tbody>

  <tr>

   <td width="264"><em>f</em><sub>1</sub>(<em>n</em>) = 7<em>.</em>2 + 34<em>n</em><sup>3 </sup>+ 3254<em>n</em></td>

   <td width="180"><em>f</em><sub>2</sub>(<em>n</em>) = <em>n</em><sup>2 </sup>log<em>n </em>+ 25<em>n</em>log<sup>2 </sup><em>n</em></td>

  </tr>

  <tr>

   <td width="264"><em>f</em>3(<em>n</em>) = 24log<em>n </em>+ 5<em>n</em>5</td>

   <td width="180"><em>f</em><sub>4</sub>(<em>n</em>) = 22<em>n</em><sup>2</sup>+4<em>n</em>+7</td>

  </tr>

 </tbody>

</table>

<strong>Problem 3.            More Asymptotic Analysis!</strong>

Let <em>f </em>and <em>g </em>be functions of <em>n </em>where <em>f</em>(<em>n</em>) = <em>O</em>(<em>n</em>) and <em>g</em>(<em>n</em>) = <em>O</em>(log<em>n</em>). Find the best asymptotic bound <em>(if possible) </em>of the following functions.

<ul>

 <li><em>h</em><sub>1</sub>(<em>n</em>) = <em>f</em>(<em>n</em>) + <em>g</em>(<em>n</em>)</li>

 <li><em>h</em><sub>2</sub>(<em>n</em>) = <em>f</em>(<em>n</em>) × <em>g</em>(<em>n</em>)</li>

 <li><em>h</em><sub>3</sub>(<em>n</em>) = max(<em>f</em>(<em>n</em>)<em>,g</em>(<em>n</em>))</li>

 <li><em>h</em><sub>4</sub>(<em>n</em>) = <em>f</em>(<em>g</em>(<em>n</em>))</li>

 <li><em>h</em><sub>5</sub>(<em>n</em>) = <em>f</em>(<em>n</em>)<em><sup>g</sup></em><sup>(<em>n</em>)</sup></li>

</ul>

<h2>Problem 4.           Time complexity analysis</h2>

Analyse the following code snippets and find the best asymptotic bound for the time complexity of the following functions with respect to <em>n</em>.

<ul>

 <li>public int niceFunction(int n) { for (int i = 0; i &lt; n; i++) {</li>

</ul>

System.out.println(“I am nice!”);

} return 42;

}

<ul>

 <li>public int meanFunction(int n) { if (n == 0) return 0; return 2 * meanFunction(n / 2) + niceFunction(n); }</li>

 <li>public int strangerFunction(int n) { for (int i = 0; i &lt; n; i++) {</li>

</ul>

for (int j = 0; j &lt; i; j++) {

System.out.println(“Execute order?”); } } return 66;

}

<ul>

 <li>public int suspiciousFunction(int n) { if (n == 0) return 2040;</li>

</ul>

int a = suspiciousFunction(n / 2); int b = suspiciousFunction(n / 2); return a + b + niceFunction(n);

}

<ul>

 <li>public int badFunction(int n) { if (n &lt;= 0) return 2040; if (n == 1) return 2040; return badFunction(n – 1) + badFunction(n – 2) + 0; }</li>

 <li>public int metalGearFunction(int n) { for (int i = 0; i &lt; n; i++) { for (int j = 1; j &lt; i; j *= 2) {</li>

</ul>

System.out.println(“!”);

} } return 0;

}

<strong>Problem 5. Another Application of Binary Search (Optional) </strong>Given a sorted array of <em>n</em>−1 unique elements in the range [1<em>,n</em>], find the missing element? Discuss possible naive solutions and possibly faster solutions.