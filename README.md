# -
/**
2019.7.22
Leetcode第一题——两数之和
**/

class Solution {
    public int[] twoSum(int[] nums, int target) {
            int m=-1;
            int n=-1;
        for(int i=0;i<nums.length;i++){
            int x=target-nums[i];
            for(int j=i+1;j<nums.length;j++){
                if(nums[j]==x){
                    n=j;
                    m=i;
                }
            }
        }
        return new int[]{m,n};
    }
}
