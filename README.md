# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.
  
a. If 'Machine A' is faster but runs a more inefficient program than 'Machine B', the program on 'Machine B' could finish sooner. Run time and performance in practice is not solely dictated by asymptotic analysis.
  
b. As an example, Big O covers the upper bound. So an algorithm that has a time complexity of O(n!), could also have a time complexity of O(n<sup>2</sup>), or O(n), so on. If your algorithm has a time complexity of O(n!), all that's said is it can grow no faster than O(n!). It could have a different run time in a real life application, as long as it is below O(n!).

c. Something I noticed that is similar to the calculus classes that I have taken, is that lower order terms are dropped during some operations. When terms are dropped while finding time complexity of an algorithm, it makes sense in theory but when you go to run your program, you might get something that is not at all what you expected.
  
- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

log<sub>2</sub>(1000) = 9.96

log<sub>2</sub>(10000) = 13.28

If you divide $$\frac{13.28}{9.96}$$, you get 1.3. This means that a finding an element in a tree of 10000 elements will take approximately 1.3 times longer than finding an element in a tree of 1000 elements. We can multiply the given time to search in a tree of 1000 elements (5 seconds) by the ratio (1.3) we found above. 5 * 1.3 = 6.6. So based on this question, I found that finding an element in a tree of 10000 elements will take around 6.6 seconds.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

a. 

b. 

c. 

Add your answers to this markdown file.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
