# Find the Winner of the Circular Game

LeetCode Q # 1823.

There are n friends that are playing a game. The friends are sitting in a circle and are numbered from 1 to n in clockwise order. More formally, moving clockwise from the ith friend brings you to the (i+1)th friend for 1 <= i < n, and moving clockwise from the nth friend brings you to the 1st friend.

The rules of the game are as follows:

- Start at the 1st friend.</br>
- Count the next k friends in the clockwise direction including the friend you started at. The counting wraps around the circle and may count some friends more than once.</br>
- The last friend you counted leaves the circle and loses the game.</br>
- If there is still more than one friend in the circle, go back to step 2 starting from the friend immediately clockwise of the friend who just lost and repeat.</br>
- Else, the last friend in the circle wins the game.</br>
- Given the number of friends, n, and an integer k, return the winner of the game.

Example 1:

<div align = "center">

  ![image](https://github.com/xo-azeem/Find-the-Winner-of-the-Circular-Game-LeetCode/assets/171427226/11f73091-18fd-4323-aff0-41882aa8cb54)

</div>

> Input: n = 5, k = 2</br>
> Output: 3</br>
> Explanation: Here are the steps of the game:</br>
> 1) Start at friend 1.</br>
> 2) Count 2 friends clockwise, which are friends 1 and 2.</br>
> 3) Friend 2 leaves the circle. Next start is friend 3.</br>
> 4) Count 2 friends clockwise, which are friends 3 and 4.</br>
> 5) Friend 4 leaves the circle. Next start is friend 5.</br>
> 6) Count 2 friends clockwise, which are friends 5 and 1.</br>
> 7) Friend 1 leaves the circle. Next start is friend 3.</br>
> 8) Count 2 friends clockwise, which are friends 3 and 5.</br>
> 9) Friend 5 leaves the circle. Only friend 3 is left, so they are the winner.

Example 2:

> Input: n = 6, k = 5</br>
> Output: 1</br>
> Explanation: The friends leave in this order: 5, 4, 6, 2, 3. The winner is friend 1.

My Solution Analysis:

<div align = "center">

  ![image](https://github.com/xo-azeem/Find-the-Winner-of-the-Circular-Game-LeetCode/assets/171427226/504d2271-3d78-4aa0-a731-3e05029b0b0e)

  Time complexity: O(n).</br>Space complexity: O(1).
</div>
