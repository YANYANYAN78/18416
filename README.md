# 18416
素数



题目：判断101-200之间有多少个素数，并输出所有素数。
程序分析：判断素数的方法：用一个数分别去除2到这个数，如果能被整除，则表明此数不是素数，反之是素数。



l = []
for i in range(101,200):
    for j in range(2,i):
        if i%j ==0:
            break
    else:
        l.append(i)

print(len(l))





def a(n):
   L = []
   for i in range(2,n-1):
       L.append(n%i)
   if  0 not in L:
      return True
print filter(a,range(101,200))
