class Solution:
    def fizzBuzz(self, n: int) -> List[str]:
        result = []
        side = []
        for i in range(1, n+1):
            side.append(i)
        print(side)
        for i in side:
            if (i%3)==0 and (i%5)==0:
                result.append("FizzBuzz")
            elif (i%3)==0 and (i%5)!=0:
                result.append("Fizz")
            elif (i%3)!=0 and (i%5)==0:
                result.append("Buzz")
            elif (i%3)!=0 and (i%5)!=0:
                result.append(str(i))
        return result