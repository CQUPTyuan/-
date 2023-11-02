//两数之和
class Solution {
    public int[] twoSum(int[] nums, int target) {
    for(int i = 0; i < nums.length; i++){
        for(int j = i + 1; j < nums.length; j++){
            if(nums[i] + nums[j] == target ){
                return new int[]{i,j};
            }
        }
    }
    return new int[0];
    } 
}


//回文数
class Solution {
    public boolean isPalindrome(int x) {
        int a = x;
       int b = 0;
        if(x < 0){
            return false;
        }while(x>0){
            b = b*10 + x%10;
            x = x/10;
        }
            if(b == a){
                return true;
            }else{
                return false;
            }

    }  
}

















