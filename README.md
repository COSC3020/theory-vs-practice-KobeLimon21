# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.

- Asymptotic analysis does not account for constants , which can be very misleading in the scope of comparing two algorithms. Foresay, if an algorithm with a better time complexity has a large constant, it could be much more time consuming for small inputs than an algorithm with a worse time complexity and much smaller constant.
- Asmyptotic analysis focuses on the growth of input sizes (n) to determine how efficient an algorithm may be. This could result in a bad case with smaller inputs, where the speed may not reflect what the asymptotic analysis states since it focuses more so how it grows  in relation to large sizes rather than small sizes.
- It does not account hardware in the analysis, which could be a huge factor being that is not reflected on.

Assuming time complexity is `O(log(n))` , I would use log(10000) which is equal to about 13.3.

Using this height of 13.3 we can divide it by 10 which is about the height for 1000 elements and multiply it by 5 seconds 

13/10 * 5 = 6.65 seconds 

- One reason could be a memory leak, where if the computer has ran out of memory it could start to make inefficient decisions to be make up for the leak. This could also be the result of a bad implementation that doesn't account for the memory efficiently. 
- The binary tree could be inbalanced, which would then result in a huge time inefficiency because we are not having to traverse down each and every node for specific elements. This is a result of the tree being skewed heavily, where in the worst case it could start to look like a linked list. 
- Bad implemenations could be a result of the disparity within time, if we are adding conditions on top of what the asymptotic analysis accounted then it will indefinitely take much longer. These conditions will stack the time taken for them to be used as the size grows, which wouldn't have as much of an impact as it does on a smaller input due to the increased workload that would be accounted for with 10000 elements.


Sources : 
https://www.cs.cornell.edu/courses/cs312/2004fa/lectures/lecture16.htm  - explained the analysis with more detail

https://www.geeksforgeeks.org/asymptotic-notation-and-analysis-based-on-input-size-of-algorithms/ - used for more information

https://www.youtube.com/watch?v=2EyEaY4FT0E - used for the second reason 



"I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice."



  
