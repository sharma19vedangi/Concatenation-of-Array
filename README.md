# Concatenation-of-Array
#Array Leetcode Problem Solution
class Solution {
    public int[] getConcatenation(int[] nums) {
        int n=nums.length*2;
        int a[]=new int[n];
        int i;
        for(i=0;i<nums.length;i++)
        {
            a[i]=nums[i];
        }
        int j=0;
        while(i!=n)
        {
            a[i]=a[j];
            j++;
            i++;
        }
        return a;
    }
}
