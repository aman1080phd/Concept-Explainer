Video URL : https://drive.google.com/file/d/1tdRBw_Zm85evKfGRmd8rqETab-leYFOa/view?usp=sharing


  Code: 


    class Solution {
  
      public int search(int[] nums, int target) {
          int start = 0;
          int end = nums.length-1;

          while(start<=end)
          {
              int mid = (start + end)/2;

              if(nums[mid]==target)
              {
                  return mid;
              }
              else if(nums[mid]<target)
              {
                  start = mid+1;
              }
              else{
                  end = mid-1;
              }
          }

          return -1;

       }
    }
