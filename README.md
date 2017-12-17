inp = input('please enter the file name: ')
fname = open(inp)
lst = list()
for line in fname:
    line =line.strip()
    words = line.split()
    for i in words:
        if i in lst: continue
        else:
            lst.append(i)
lst.sort()
print (lst)
