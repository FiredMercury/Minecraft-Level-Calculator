def findexp(var):
    if var < 32:
        expval = 2.5 * var ** 2 - 40.5 * var + 360
        if var < 16:
            expval = var ** 2 + 6 * var
    if var > 31:
        expval = 4.5 * var ** 2 - 162.5 * var + 2220
    return expval


def dif(var2, var3):
    expval3 = findexp(int(var2))
    expval4 = findexp(int(var3))
    expdif = expval4 - expval3
    return expdif


def reverse(var4, var5):
    expval5 = findexp(var4)
    expval6 = expval5 + var5
    expval7 = 0
    level = 0
    while expval7 < expval6:
        level = level + 1
        expval7 = findexp(level)
    return level


print('1 - Find the exp required to get to a certain level.')
print('2 - Find the exp required to get to a level from another level')
print('3 - Find which level you get to from another level with a certain amount of exp')
question = int(input('Which would you like to use? '))

if question == 1:
    q1 = int(input('Which level do you want to get to? '))
    print('You need', str(findexp(q1)), 'experience.')

if question == 2:
    q2 = int(input('What is the starting level? '))
    q3 = int(input('Which level do you want to get to? '))
    print('You need', str(dif(q2, q3)), 'experience.')

if question == 3:
    q4 = int(input('Which level are you on? '))
    q5 = int(input('How much experience? '))
    print('You can get to level', str(reverse(q4, q5)), '.')
    
