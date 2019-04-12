class Solution:
    def canWinNim(self, n: int) -> bool:
        result = True
        if n%4 == 0:
            result = False
        return result