# Sort-Array-by-Increasing-Frequency
class Solution:
    def frequencySort(self, nums: list[int]) -> list[int]:
        if nums is None:
            return none
        count=Counter(nums)
        r=[]
        for i,c in count.items():
            for j in range(c):
                r.append(i)
        r.sort(reverse=True)
        r.sort(key=lambda x:count[x])
        return r
