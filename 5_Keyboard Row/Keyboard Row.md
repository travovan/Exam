class Solution:
    def findWords(self, words: List[str]) -> List[str]:
        alphabet_list1 = 'qwertyuiopQWERTYUIOP'
        alphabet_list2 = 'asdfghjklASDFGHJKL'
        alphabet_list3 = 'zxcvbnmZXCVBNM'
        result = []
        for word in words:
            if all(map(lambda x:x in alphabet_list1,word)) or all(map(lambda x:x in alphabet_list2, word)) or all(map(lambda x:x in alphabet_list3, word)):
                result.append(word)
        return result