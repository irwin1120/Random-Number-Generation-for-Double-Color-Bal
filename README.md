# Random-Number-Generation-for-Double-Color-Bal
import random
n = eval(input("请输入组数："))
while n:
    num = []
    n-=1
    for i in range(6):
        redball=random.randint (1,34)
        while redball in num:
            redball=random.randint (1,34)
        num.append(redball)        
    num.sort()
    blueball=random.randint (1,17)
    num.append(blueball)
    print ("您的随机号码是：{0}".format(num))
