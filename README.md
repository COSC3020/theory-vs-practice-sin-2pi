# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.
  
 ### a. Small input sizes are ignored. An algorithm that is 'faster' may actually be slower with a smaller input size.
  
 ### b.There is a worst case, best case, and average case. Asymptotic analysis may show that quicksort would be faster than mergesort, but if each have their 'worst case', then mergesort will actually be faster.

 ### c. Something I noticed that is similar to the calculus classes that I have taken, is that lower order terms are dropped when simplifying a function. When terms are dropped while finding time complexity of an algorithm, it makes sense in theory but when you go to run your program, you might get something that is not at all what you expected.
  
- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.
