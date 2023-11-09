# my-leetcode-journey
Repository detailing what I do day to day to improve my data structures, algorithm and problem solving skills using primarily leetcode as my source of learning.

## Day 1

### Leetcode profile:


![image](https://github.com/BlunderBarry/my-leetcode-journey/assets/115489663/1df9efb8-6fdb-45a4-91bc-091790b79ad9)

I will do updates on my profile every 10 days.

### Goals for today: Learn Algorithmic complexity
Im ashamed to admit that I still don't know how Algorithmic complexity works... I think it's a great starting point for this journey.

### Ressource used:
- https://isaaccomputerscience.org/topics/complexity?examBoard=all&stage=all -> I started with reading through this page and taking notes.
- https://www.youtube.com/watch?v=K3NluEdHkao -> Watched this video because I was confused with O(n log n) time complexity.
- https://www.youtube.com/watch?v=yOb0BL-84h8 -> Watched this video to understand how we calculate space complexity of an algorithm.

### What I've learned/practiced:
As this is my Intro to this concept, I do not think I've grasped all there is to it, but here's what I learned:

- Big O notation is used to describe time and space complexity of an algorithm.

- Time complexity is used to represent how much steps an algorithm will need to execute fully
as we increase the input size. It is only an approximation and is useful to determine which algorithm is better.
It's represented with Big O notation.

- Space complexity is used to represent how much space an algorithm requires to run as the input size becomes bigger.
It is also only an approximation and is useful in combination with time complexity to compare different algorithms.
It's represented with Big O notation.

- Worst-case scenario, average time and best-case scenario are used to choose which algorithms is best suited for your need.
(only for time complexity)

- Learned how to calculate time complexity of an algorithm.

- Learned how to calculate space complexity of an algorithm.

### Exercises:

- Did all of these exercises : https://www.geeksforgeeks.org/practice-questions-time-complexity-analysis/
Had about a 50% - 60% rate. Not too bad but will probably check them out another day again.

- Practiced with these questions : http://curric.rithmschool.com/springboard/exercises/big-o-analysis/

- Also did these : https://kodr.me/en/big-o-exercises

### Todo:

- I decided to follow this comment from Robin Thomas as my roadmap:


![image](https://github.com/BlunderBarry/my-leetcode-journey/assets/115489663/9907b1a0-b28c-4be4-9b98-73e8e9dcd98a)

![image](https://github.com/BlunderBarry/my-leetcode-journey/assets/115489663/4fd64149-6c3e-44a5-864e-38f92ea25c7e)

*Link to comment: https://www.quora.com/Which-book-should-I-read-for-a-complete-beginner-in-data-structures-algorithms?no_redirect=1

So tomorrow I'll be working on arrays, i've worked with arrays plenty of times before, but i'm sure there's still a lot of
stuff to learn about them.


## Day 2

### Goals for today: Get better at working with arrays

### Ressource used:

- https://leetcode.com/tag/array/

 ### What I've learned/practiced:

 - Did a couple medium difficulty array problems on leetcode. Here's the link to the problems I did and the Algorithm I came up with:

1- https://leetcode.com/problems/container-with-most-water
<details>
 <summary>My solution</summary>
 
 ```
 public int maxArea(int[] height) {
        int maxWater = 0; 
        int k = height.length - 1;
        int j = 0;
        int i = 1;
        while(i < height.length){
            int dist = k - j;
            if(height[j] > height[k]){
                if(dist * height[k] > maxWater) {
                    maxWater = dist * height[k];
                }
                k--;
            } else {
                 if(dist * height[j] > maxWater) {
                    maxWater = dist * height[j];
                }
                j++;
            }
            i++;
        }
        return maxWater;
    }
```
Time complexity: O(N) - 
Space complexity: I'm not sure about this one, but my guess would be O(N)
</details>

2- https://leetcode.com/problems/rotate-array

<details>
 <summary>My solution</summary>
 Spent about 5 hours on this problem only to come empty handed.... even after checking the solution I feel like I would've never came up with that.
 Will try to solve it again in a couple of weeks.
</details>

### Todo:

Tomorrow I will continue my work on arrays and try to complete some other medium difficulty problems.









