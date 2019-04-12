class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        k = 0
        for i in range(len(nums)):
            if target-nums[i] in nums:
                print(i)
                print(nums.index(target - nums[i]))
                if i != nums.index(target - nums[i]):
                    return [i, nums.index(target - nums[i])]