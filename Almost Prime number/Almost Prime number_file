import math
# import time


def mnoj(num):
    j = 2
    while num > 1:
        for i in range(j, int(math.sqrt(num + 0.05)) + 1):
            if num % i == 0:
                num //= i
                j = i
                yield i
                break
        else:
            if num > 1:
                yield num
            break


it = []
a, b = list(map(int, input().split()))
# s_t = time.time()
for num in range(a, b + 1):
    rez = []
    for y in mnoj(num):
        if y in rez:
            rez = []
            break
        rez.append(y)
    if len(rez) > 1 and (len(rez) == len(set(rez))):
        it.append(str(num))
if it:
    print(" ".join(it))
else:
    print("NO")
# print("--- %s seconds ---" % (time.time() - s_t))
