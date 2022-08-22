# 超简单练手题

本分类收录了Easy题中正确率大于60%的题目(正确率统计时间：2020-12-16)，即基本无任何算法元素，完全是对语言知识进行入门学习的方式。考虑到读者已经有一定的C++基础，故而不对题目算法做过多分析而是直接进行语言的相关补充。

## 1672 Richest Customer Wealth

>  题意：给定一个二维数组，给出二维数组每一行的和中的最大值。

- 函数参数中二维数组的表示：`int[][] accounts`

- for循环写法可以与C++中保持一致

- 对数组长度的访问直接使用`.length`

- 比较较大值`Math.max()`, 支持同为double，float，int，long的参数

一种内存占用更小的写法：

```java
class Solution {
    public int maximumWealth(int[][] accounts) {
        int max = 0;
        for (int[] a : accounts) {
            max = Math.max(max, Arrays.stream(a).sum());
        }
        return max;
    }
}

------------分隔线-------------------
    
 public int maximumWealth(int[][] accounts) {
        return Arrays.stream(accounts).map(ints ->
                Arrays.stream(ints).sum()
        ).max(Integer::compareTo).get();
    }
```

里面使用到了Java8 的**流式接口（Fluent Interface）**。

## 1480 Running Sum of 1d Array 

## 剑指 Offer 58 - II 左旋转字符串 LCOF   	

1678 Goal Parser Interpretation   	

面试题 02.03 Delete Middle Node LCCI   	

1470 Shuffle the Array   	

1512 Number of Good Pairs   	

1431 Kids With the Greatest Number of Candies   	

771 Jewels and Stones   	

1684 Count the Number of Consistent Strings   	

1486 XOR Operation in an Array   	

1603 Design Parking System   	

LCP 01Guess Numbers   	

1108 Defanging an IP Address   	

LCP 06 拿硬币   	

237 Delete Node in a Linked List   	

1662 Check If Two String Arrays are Equivalent   	

1281Subtract the Product and Sum of Digits of an Integer   	

1389 Create Target Array in the Given Order   	

1313 Decompress Run-Length Encoded List   	

1365 How Many Numbers Are Smaller Than the Current Number   	

1614 Maximum Nesting Depth of the Parentheses   	

1266 Minimum Time Visiting All Points   	

1342 Number of Steps to Reduce a Number to Zero   	

1295 Find Numbers with Even Number of Digits   	

1572 Matrix Diagonal Sum   	

129  0 Convert Binary Number in a Linked List to Integer   	

1588 Sum of All Odd Length Subarrays   	

145  0 Number of Students Doing Homework at a Given Time   	

1688 Count of Matches in Tournament   	

LCP 17 速算机器人   	

137  0 Increasing Decreasing String   	

182 Duplicate Emails   	

627 Swap Salary   	

1528 Shuffle String   	

面试题 04.02 Minimum Height Tree LCCI   	

595 Big Countries   	

1221Split a String in Balanced Strings   	

剑指 Offer 27 二叉树的镜像  LCOF   	

剑指 Offer 55 - I	
二叉树的深度 LCOF   	

剑指 Offer 22 链表中倒数第k个节点 LCOF   	

617 Merge Two Binary Trees   	

1534 Count Good Triplets   	

1436 Destination City   	

461Hamming Distance   	

剑指 Offer 17 打印从1到最大的n位数 LCOF   	

面试题 02.02 Kth Node From End of List LCCI   	

1021Remove Outermost Parentheses   	

657 Robot Return to Origin   	

938 Range Sum of BST   	

226 Invert Binary Tree   	

1656 Design an Ordered Stream   	

1299 Replace Elements with Greatest Element on Right Side   	

1464 Maximum Product of Two Elements in an Array   	

62  0 Not Boring Movies   	

804 Unique Morse Code Words   	

剑指 Offer 05 替换空格 LCOF   	

709 To Lower Case   	

1351Count Negative Numbers in a Sorted Matrix   	

1252 Cells with Odd Values in a Matrix   	

832 Flipping an Image   	

104 Maximum Depth of Binary Tree   	

1323 Maximum 69 Number   	

剑指 Offer 06 从尾到头打印链表 LCOF   	

1309 Decrypt String from Alphabet to Integer Mapping   	

59  0 N-ary Tree Postorder Traversal   	

700	Search in a Binary Search Tree   	

728 Self Dividing Numbers   	
	
108 Convert Sorted Array to Binary Search Tree   	

1002 Find Common Characters   	
1304 Find N Unique Integers Sum up to Zero   	
146  0 Make Two Arrays Equal by Reversing Sub-arrays   	
剑指 Offer 24 反转链表 LCOF   	
1051Height Checker   	
剑指 Offer 54 二叉搜索树的第k大节点  LCOF   	
344 Reverse String   	
589 N-ary Tree Preorder Traversal   	
175 Combine Two Tables   	
511Game Play Analysis I   	
557 Reverse Words in a String III   	
1356 Sort Integers by The Number of 1 Bits   	
977 Squares of a Sorted Array   	
349 Intersection of Two Arrays   	
面试题 16.07 Maximum LCCI   	
1374 Generate a String With Characters That Have Odd Counts   	
1207 Unique Number of Occurrences   	
897 Increasing Order Search Tree   	
1502 Can Make Arithmetic Progression From Sequence   	
剑指 Offer 25 合并两个排序的链表  LCOF   	
164  0 Check Array Formation Through Concatenation   	
剑指 Offer 15 二进制中1的个数 LCOF   	
1148 Article Views I   	
561Array Partition I   	
剑指 Offer 09 用两个栈实现队列 LCOF   	
138  0 Lucky Numbers in a Matrix   	
942 DI String Match   	
面试题 01.01Is Unique LCCI   	
1475 Final Prices With a Special Discount in a Shop   	
1636 Sort Array by Increasing Frequency   	
933 Number of Recent Calls   	
922 Sort Array By Parity II   	
463 Island Perimeter   	
1025 Divisor Game   	
103  0 Matrix Cells in Distance Order   	
577 Employee Bonus   	
893 Groups of Special-Equivalent Strings   	
面试题 03.04 Implement Queue using Stacks LCCI   	
206 Reverse Linked List   	
559 Maximum Depth of N-ary Tree   	
1122 Relative Sort Array   	
359 Logger Rate Limiter   	
1086 High Five   	
293 Flip Game   	
191Number of 1 Bits   	
852 Peak Index in a Mountain Array   	
136 Single Number   	
1385 Find the Distance Value Between Two Arrays   	
1237 Find Positive Integer Solution for a Given Equation   	
1619 Mean of Array After Removing Some Elements   	
181Employees Earning More Than Their Managers   	
1652 Defuse the Bomb   	
944 Delete Columns to Make Sorted   	
521Longest Uncommon Subsequence I   	
876 Middle of the Linked List   	
1426 Counting Elements   	
50  0 Keyboard Row   	
118 Pascal's Triangle   	
905 Sort Array By Parity   	
面试题 05.07 Exchange LCCI   	
476 Number Complement   	
389 Find the Difference   	
剑指 Offer 57 - II	
和为s的连续正数序列 LCOF   	
1327 List the Products Ordered in a Period   	
292 Nim Game   	
80  0 Similar RGB Color   	
346 Moving Average from Data Stream   	
面试题 02.01Remove Duplicate Node LCCI   	
999 Available Captures for Rook   	
1403 Minimum Subsequence in Non-Increasing Order   	
剑指 Offer 68 - II	
二叉树的最近公共祖先 LCOF   	
811Subdomain Visit Count   	
1047 Remove All Adjacent Duplicates In String   	
1196 How Many Apples Can You Put into the Basket   	
908 Smallest Range I   	
762 Prime Number of Set Bits in Binary Representation   	
1217 Minimum Cost to Move Chips to The Same Position   	
剑指 Offer 68 - I	
二叉搜索树的最近公共祖先 LCOF   	
682 Baseball Game   	
637 Average of Levels in Binary Tree   	
面试题 02.07 Intersection of Two Linked Lists LCCI   	
116  0 Find Words That Can Be Formed by Characters   	
171Excel Sheet Column Number   	
剑指 Offer 32 - II	
从上到下打印二叉树 II LCOF   	
1413 Minimum Value to Get Positive Step by Step Sum   	
965 Univalued Binary Tree   	
821Shortest Distance to a Character   	
258 Add Digits   	
面试题 08.03 Magic Index LCCI   	
603 Consecutive Available Seats   	
1427 Perform String Shifts   	
1075 Project Employees I   	
1022 Sum of Root To Leaf Binary Numbers   	
剑指 Offer 39 数组中出现次数超过一半的数字  LCOF   	
120  0 Minimum Absolute Difference   	
107 Binary Tree Level Order Traversal II   	
575 Distribute Candies   	
1598 Crawler Log Folder   	
1518 Water Bottles   	
183 Customers Who Never Order   	
1491Average Salary Excluding the Minimum and Maximum Salary   	
1294 Weather Type in Each Country   	
剑指 Offer 03 数组中重复的数字 LCOF   	
607 Sales Person   	
867 Transpose Matrix   	
155  0 Three Consecutive Odds   	
961N-Repeated Element in Size 2N Array   	
766 Toeplitz Matrix   	
669 Trim a Binary Search Tree   	
1582 Special Positions in a Binary Matrix   	
883 Projection Area of 3D Shapes   	
1485 Group Sold Products By The Date   	
1407 Top Travellers   	
61  0 Triangle Judgement   	
1332 Remove Palindromic Subsequences   	
LCP 02 Deep Dark Fraction   	
1394 Find Lucky Integer in an Array   	
257 Binary Tree Paths   	
225 Implement Stack using Queues   	
496 Next Greater Element I   	
509 Fibonacci Number   	
1511Customer Order Frequency   	
806 Number of Lines To Write String   	
1399 Count Largest Group   	
566 Reshape the Matrix   	
235 Lowest Common Ancestor of a Binary Search Tree   	
1661Average Time of Process per Machine   	
122 Best Time to Buy and Sell Stock II   	
剑指 Offer 57 和为s的两个数字 LCOF   	
1633 Percentage of Users Attended a Contest   	
1064 Fixed Point   	
面试题 01.02 Check Permutation LCCI   	
232 Implement Queue using Stacks   	
1211Queries Quality and Percentage   	
412 Fizz Buzz   	
243 Shortest Word Distance   	
169 Majority Element   	
1337 The K Weakest Rows in a Matrix   	
266 Palindrome Permutation   	
196 Delete Duplicate Emails   	
面试题 08.06 Hanota LCCI   	
LCP 11期望个数统计   	
1694 Reformat Phone Number   	
21Merge Two Sorted Lists   	
1608 Special Array With X Elements Greater Than or Equal X   	
884 Uncommon Words from Two Sentences   	
面试题 17.04 Missing Number LCCI   	
1114 Print in Order   	
剑指 Offer 21调整数组顺序使奇数位于偶数前面 LCOF   	
1441Build an Array With Stack Operations   	
303 Range Sum Query - Immutable   	
929 Unique Email Addresses   	
892 Surface Area of 3D Shapes   	
1189 Maximum Number of Balloons   	
1455 Check If a Word Occurs As a Prefix of Any Word in a Sentence   	
1667 Fix Names in a Table   	
剑指 Offer 62 圆圈中最后剩下的数字 LCOF   	
1118 Number of Days in a Month   	
1133 Largest Unique Number   	
283 Move Zeroes   	
1435 Create a Session Bar Chart   	
242 Valid Anagram   	
1103 Distribute Candies to People   	
剑指 Offer 52 两个链表的第一个公共节点  LCOF   	
19  0 Reverse Bits   	
1624 Largest Substring Between Two Equal Characters   	
872 Leaf-Similar Trees   	
119 Pascal's Triangle II   	
1179 Reformat Department Table   	
面试题 17.12 BiNode LCCI   	
696 Count Binary Substrings   	
13 Roman to Integer   	
LCP 07 传递信息   	
812 Largest Triangle Area   	
1279 Traffic Light Controlled Intersection   	
1078 Occurrences After Bigram   	
868 Binary Gap   	
1046 Last Stone Weight   	
115  0 Check If a Number Is Majority Element in a Sorted Array   	
1317 Convert Integer to the Sum of Two No-Zero Integers   	
117  0 Compare Strings by Frequency of the Smallest Character   	
448 Find All Numbers Disappeared in an Array   	
1287 Element Appearing More Than 25% In Sorted Array   	
202 Happy Number   	
1185 Day of the Week   	
1408 String Matching in an Array   	
693 Binary Number with Alternating Bits   	
53  0 Minimum Absolute Difference in BST   	
126  0 Shift 2D Grid   	
788 Rotated Digits   	
面试题 03.02 Min Stack LCCI   	
824 Goat Latin   	
剑指 Offer 5  0 第一个只出现一次的字符  LCOF   	
10  0 Same Tree   