Download Link: https://assignmentchef.com/product/solved-cse222_505-hw2-asymptotic-notations-and-algorithm-performance
<br>
<strong>PART 1 :</strong> Analyze the following algorithms. Write worst-case, average-case, base-case analysis if significant. Express your results using most proper asymptotic notation.

Explain your solutions. For the 1<sup>st</sup> to the 4<sup>th</sup> algorithms use table method and show table.

<ol>

 <li></li>

</ol>

<table width="602">

 <tbody>

  <tr>

   <td width="602">somefunction(rows, cols){      for(i = 1; i &lt;= rows; i++){           for( j = 1; j &lt;= cols; j++)                print(*)            print(newline)}} </td>

  </tr>

 </tbody>

</table>




<ol start="2">

 <li></li>

</ol>

<table width="602">

 <tbody>

  <tr>

   <td width="602">somefunction(a, b){       if (b == 0)           return 1       answer = a       increment = afor(i = 1; i &lt; b; i++){           for(j = 1; j &lt; a; j++){               answer += increment}           increment = answer}       return answer} </td>

  </tr>

 </tbody>

</table>




<ol start="3">

 <li></li>

</ol>

<table width="602">

 <tbody>

  <tr>

   <td width="602">somefunction(arr[], arr_len){val = 0for (i = 0; i &lt; arr_len / 2; i++)         val = val + arr[i]for (i = n / 2; i &lt; arr_len; i++)          val = val – arr[i]if (val &gt;= 0)          return 1     elsereturn –1} </td>

  </tr>

 </tbody>

</table>




<ol start="4">

 <li></li>

</ol>

somefunction(n)

{

c = 0      for (i = 1 to n*n)           for (j = 1 to n)                for (k = 1 to 2*j)                     c = c+1

return c

}




<ol start="5">

 <li></li>

</ol>

<table width="602">

 <tbody>

  <tr>

   <td width="602">otherfunction(xp, yp){       temp = xp      xp = yp      yp = temp}      somefunction(arr[], arr_len){        for (i = 0; i &lt; arr_len – 1; i++){         min_idx = ifor (j = i+1; j &lt; arr_len; j++)               if (arr[j] &lt; arr[min_idx])                    min_idx = jotherfunction(arr[min_idx], arr[i])}}</td>

  </tr>

  <tr>

   <td width="602"> </td>

  </tr>

 </tbody>

</table>




<ol start="6">

 <li></li>

</ol>

<table width="602">

 <tbody>

  <tr>

   <td width="602">otherfunction(a, b){if b == 0:       return 1 answer = aincrement = a for i = 1 to b:{       for j = 1 to a:answer += increment increment = answer}return answer} somefunction(arr, arr_len){for i = 0 to arr_len):       for j = i to arr_len):          if otherfunction(arr[i], 2) == arr[j]:print(arr[i], arr[j])          elif otherfunction(arr[j], 2) == arr[i]:print(arr[j], arr[i])} </td>

  </tr>

 </tbody>

</table>




<ol start="7">

 <li></li>

</ol>

<table width="602">

 <tbody>

  <tr>

   <td width="602">otherfunction(X, i){      s = 0      for(j = 0; j &lt;= i; j=j*2)           s = s + X[j]      return s}  somefunction(arr[], arr_len){for(i = 0; i &lt;= arr_len-1; i++)A[i] = otherfunction(arr, i) / (i + 1)      return A}</td>

  </tr>

 </tbody>

</table>




<ol start="8">

 <li></li>

</ol>

<table width="602">

 <tbody>

  <tr>

   <td width="602">somefunction(n){res = 0j = 1 if(n &lt; 10)return n + 10 for(i = 9; i &gt;= 1; i–)           while (n % i == 0)                n = n / i                res = res + j * i                j *= 10 if(n &gt; 10)          return -1      return res} </td>

  </tr>

 </tbody>

</table>




<strong>PART 2 :</strong> Design an algorithm for each of the problems. Write your algorithms in pseudo code. Obtain the complexities of the algorithms. Write worst-case, average-case, base-case analysis if significant. Express your results using most proper asymptotic notation. Explain your solutions.

<ol>

 <li>Assume you have an array of points in 2d space. Find the closest point in the array to a given point.</li>

 <li>The i<sup>th</sup> element of an array A is a local minimum if, A[i] &lt;= A[i+1] and A[i] &lt;= A[I-1].

  <ol>

   <li>Find a local minimum in a given array A.</li>

   <li>Find all local minimums in a given array A.</li>

  </ol></li>

 <li>Find if a given array of integers contains two numbers whose sum is a given number b.</li>

 <li>A sequence of positive integers in increasing order, a1, a2,…,an is called a “Sum Chain of Length n” if for all k (1 &lt; k ≤ n), there exist i, j (1 ≤ i ≤ j ≤ k) such that ak=ai+aj</li>

</ol>

Example: {1, 2, 3, 5, 10, 13, 15} : (2=1+1, 3=2+1, 5=3+2, 10=5+5, 13=10+3, 15=10+5)

Find if a given sequence of n numbers is a “Sum Chain of Length n”. Use the algorithm you design for the third question in this part.


