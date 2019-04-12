class Solution:
    def canWinNim(self, n: int) -> bool:
        result = True
        take_stone = (1, 2, 3)
        for i in take_stone:
            k = n-i
            if ((k+i)%4) == 0:
                result = False
        return result