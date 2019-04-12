class Solution:
    def reverseWords(self, s: str) -> str:
        new=[i[::-1] for i in s.split(" ")]
        return " ".join(new)