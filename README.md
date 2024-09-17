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
- Input size is overlooked, as asmyptotic analysis focuses on large scale input sizes to determine how efficient an algorithm may be. This is not always the best case, as if we are looking at a problem with a small input and choose what looks like the most efficient based on analysis it can lead to consequences as we do not know how fast it is in practice with a much smaller size then it was computed to be used for.
- We do not know what kind of data we are working with, if our data set is already sorted or close to being sorted we could use a algorithm with a theoritcally worse analysis but it would be faster because it's quicker on data that is already sorted such as insertion sort which has a bad time complexity compared to other algorithms with better complexities such as quicksort.

Assuming time complexity is `O(log(n))` , I would use log(10000) which is equal to about 13.3.

Using this height of 13.3 we can divide it by 10 which is about the height for 1000 elements and multiply it by 5 seconds 

13/10 * 5 = 6.65 seconds 

- One reason could be a memory leak, where if the computer has ran out of memory it could start to make inefficient decisions to be make up for the leak. This could also be the result of a bad implementation that doesn't account for the memory efficiently. 
- Another reason could be that the computer is not a very strong computer and infact a weak computer resulting in very sluggish speeds such as this case.
- Finally, if there is a huge program running in the background there can be bad consequences to this because there is not enough resources to handle the ongoing processes.


Sources : 
https://www.cs.cornell.edu/courses/cs312/2004fa/lectures/lecture16.htm  - explained the analysis with more detail

"I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice."



  
