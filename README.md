# Two sum project
#Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
#You may assume that each input would have exactly one solution, and you may not use the same element twice.

#CODE

def solution(nums, target): 
  for i in range(len(nums)+1):        #first loop ensures every number is tried as an initial number
      target_2 = target - nums[i]    #target_2 is the value to search for to create the final target sum
      for j in range(len(nums)+1):    #second loop ensures every possible pair is tried 
          if not (j == i) and (nums[j] == target_2):
              return [j,i]
 
                


lists = [2,7,11,15]
target = 9
solution_1 = solution(lists, target)
print(lists[solution_1[0]],"and", lists[solution_1[1]], "can be added together to make", target)


#testcases, input any of these numbers to test the code:
#list_1 = [3,3]
#list_2 = [3,2,4]
#list_3 = [2,7,11,15
#target_1 = 6
#target_2 = 6
#target_3 = 9

