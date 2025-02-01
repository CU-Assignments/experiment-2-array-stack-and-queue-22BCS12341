import java.util.HashMap;

class Solution {
    public int[] twoSum(int[] nums, int target) {
        HashMap<Integer, Integer> map = new HashMap<>();
        
        for (int i = 0; i < nums.length; i++) {
            int complement = target - nums[i]; 
            
            if (map.containsKey(complement)) {
                return new int[]{map.get(complement), i};
            
            map.put(nums[i], i); 
        }
        
        return new int[]{}; 
    }
}

OutPut
![image](https://github.com/user-attachments/assets/4c5e01e3-ef7b-4ef7-9049-08181b38d136)

