javascript-questions
====================

JavaScript Interview Questions

Q: Add the class of 'threes' to every third row without using a library.

A: 

Solution 1:
<pre>  var thirdRows = document.querySelectorAll('tr:nth-of-type(3n)'),
       count,
       i;
  count = thirdRows.length;
  for(i = 0; i &lt; count; i++){
    thirdRows[i].classList.add('threes');
  }</pre>
  
Solution 2: 
<pre>  /* old school method */
  var rows = document.getElementsByTagName('tr'),
      count,
      i;
  count = rows.length;
  for(i = 0; i &lt; count; i += 3){
     rows[i].setAttribute('class', 'threes');
  }</pre>
  
  Bonus points if they say there's no need to add closs odd, just style based on the selector
  tr:nth-of-type(3n) 
  
  </pre> 
