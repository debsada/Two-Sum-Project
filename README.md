# Two sum project
#Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
#You may assume that each input would have exactly one solution, and you may not use the same element twice.

def solution(nums, target):
  for i in range(len(nums)+1):
      target_2 = target - nums[i]
      for j in range(len(nums)+1):
          print(j)
          if not (j == i) and (nums[j] == target_2):
              return [j,i]
                


list_1 = [3,3]
list_2 = [3,2,4]
list_3 = [2,7,11,15
target_1 = 6
target_2 = 6
target_3 = 9
print(solution(list_1, target_1))


