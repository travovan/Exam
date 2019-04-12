class Solution:
    def selfDividingNumbers(self, left: int, right: int) -> List[int]:
        result =[]
        for i in range(left, right+1):
            l= list(str(i))
            if '0' not in l:
                if all(i%int(l[j]) ==0 for j in range(len(l))):
                    result.append(i)
        return result