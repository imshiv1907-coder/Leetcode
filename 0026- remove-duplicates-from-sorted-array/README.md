
<h2><a href="https://leetcode.com/problems/remove-duplicates-from-sorted-array/description/">26. Remove Duplicates from Sorted Array
</a></h2><h3>Easy</h3><hr><p>Given an integer array nums sorted in non-decreasing order, remove the duplicates in-place such that each unique element appears only once. The relative order of the elements should be kept the same..</p>

<p>
Consider the number of unique elements in nums to be k​​​​​​​​​​​​​​. After removing duplicates, return the number of unique elements k.</p>
<p>The first k elements of nums should contain the unique numbers in sorted order. The remaining elements beyond index k - 1 can be ignored.</p>

<h3>Custom Judge:</h3

<p1>The judge will test your solution with the following code:</p1></br>
<p2>int[] nums = [...]; // Input array</br>
int[] expectedNums = [...]; // The expected answer with correct length</br>
int k = removeDuplicates(nums); // Calls your implementation</br>

assert k == expectedNums.length;</br>
for (int i = 0; i < k; i++) {</br>
    assert nums[i] == expectedNums[i];</br>
}</p2>
<p1>If all assertions pass, then your solution will be **accepted**.</p1>

<p>&nbsp;</p>
<p><strong class="example">Example 1:</strong></p>

<pre>
<strong>Input:</strong> nums = [1,1,2]
<strong>Output:</strong> 2, nums = [1,2,_];
<strong>Explanation:</strong> Your function should return k = 2, with the first two elements of nums being 1 and 2 respectively.
It does not matter what you leave beyond the returned k (hence they are underscores).
</pre>

<p><strong class="example">Example 2:</strong></p>

<pre>
<strong>Input:</strong> nums = [0,0,1,1,1,2,2,3,3,4]
<strong>Output:</strong> 5, nums = [0,1,2,3,4,_,_,_,_,_]
<strong>Explanation:</strong> our function should return k = 5, with the first five elements of nums being 0, 1, 2, 3, and 4 respectively.
It does not matter what you leave beyond the returned k (hence they are underscores).
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code> 1 <= nums.length <= 3 * 104</code></li>
	<li><code>-100 <= nums[i] <= 100</code></li>
	<li><code>nums is sorted in non-decreasing order.[i]</code></li>
</ul>
