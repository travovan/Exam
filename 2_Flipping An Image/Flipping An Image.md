cclass Solution:
    def flipAndInvertImage(self, A: List[List[int]]) -> List[List[int]]:
        after_list = []
        for line in A:
            line.reverse()
            line = [1 - i for i in line]
            after_list.append(line)
        return after_list
        print(after_list)