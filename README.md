README
Full Counting Sort

Given integer-string pairs, sort the strings according to their integer keys using a stable counting sort. Strings in the first half of the input are replaced with "-" before sorting.

Approach
Create buckets for each possible integer key.
Replace first-half strings with "-".
Insert strings into buckets while maintaining input order.
Concatenate all buckets and print the result.
Algorithm
Find the maximum key.
Create a bucket array.
Traverse the input:
Replace first-half strings with "-".
Append each string to its corresponding bucket.
Print all bucket contents in order.
Complexity
Time: O(n + k)
Space: O(n + k)
Example

Input:

4
0 ab
1 cd
0 ef
1 gh

Output:

- ef - gh

The first half strings (ab, cd) are replaced by "-", and the stable counting sort preserves the relative order of equal keys.
