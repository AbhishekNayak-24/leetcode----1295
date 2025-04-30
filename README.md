# leetcode----1295
Find Numbers with Even Number of Digits
//code in java
class Solution {
  public int findNumbers(int[] nums) {
    int ans = 0;

    for (int num : nums)
      if (9 < num && num < 100 || 999 < num && num < 10000 || num == 100000)
        ++ans;

    return ans;
  }
}
