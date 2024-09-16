# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.
  
a. Small input sizes are ignored. An algorithm that is 'faster' may actually be slower with a smaller input size.
  
b.There is a worst case, best case, and average case. Asymptotic analysis may show that quicksort would be faster than mergesort, but if each have their 'worst case', then mergesort will actually be faster.

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

a. The tree could be unbalanced. If it is in its worst case, it will have to traverse every element like a linked list. This would be $O(n)$ time, slowing the search down significantly.

b. Asymptotic analysis does not account for the machine it is being ran on. If your machine is outdated or just does not have a lot of resources, you will have run time issues.

c. As I said earlier, about lower order terms being dropped, this could show some issues in run time. A perfect implementation of the data structure would suggest that the run time would be a certain value. However if you go through your code and analyze the time complexity line by line, it very well could be off from what you believed originally.

Add your answers to this markdown file.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
