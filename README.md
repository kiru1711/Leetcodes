# array-LC
1) Two sum

class Solution {
    public int[] getConcatenation(int[] nums) {
        int n = nums.length;
        int[] ans = new int[2 * n];
        
        for (int i = 0; i < n; i++) {
            ans[i] = nums[i];
            ans[i + n] = nums[i];
        }
        
        return ans;
    }
}
2) Move zeros

class Solution {
public void moveZeroes(int[] nums) {
int pos=0;
for(int i=0;i<nums.length;i++){
if(nums[i]!=0){
nums[pos++]=nums[i];
}
}while(pos<nums.length){
nums[pos++]=0;
}
}
} 

