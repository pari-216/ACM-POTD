#POTD Day1
#Name: Pari Garg
#Date: 22-03-26
#Problem Name: Remove Duplicate from Sorted Array
Source Code:
class Solution {
public:
    int removeDuplicates(vector<int>& nums) {
        int n = nums.size();
        if(n==0){
            return 0;
        }
        int count=0;
        for(int i=1;i<n;i++){
            if(nums[i]!=nums[count]){
                count++;
                nums[count]=nums[i];
            }
        }
        return count+1;
    }
};
Screenshot:
<img width="1919" height="942" alt="Screenshot_2026-03-22_Day1" src="https://github.com/user-attachments/assets/28085221-2a60-419f-88fe-947b1a929f10" />
