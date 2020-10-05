# b01lers
b01lers crypto world, on this write-up i'am using python 2 or 3 for solve this challenge.

# G1
for number in range(1,1000):
    if(number % 5 == 2):
        if(number % 7 == 6):
            if(number % 13 == 9):
                print number
                number -= 1
                
Flag: mini{G1_92e9a33c80ca7666c7f4b704}

# K1
for x in range(1,100000):
    for y in range (1,100000):
        if ((76*x + 221*y) % 281 == 85):
            if ((171*x + 190*y) % 281 == 138):
                print str(x) + ',' + str(y)
                x -= 1
                y -= 1
                
Flag: mini{K1_cc1c3c9a5695228061017a76}

# D1
for x in range(1,1000):
    if (11**x % 101 == 27):
        print(x)
        x += 1

Flag: mini{D1_77858210bb3c8f6f90642947}

# C1
for x in range(1,1000):
    if (x**2 % 97 == 88):
        print x

Flag: mini{C1_4c88b7b4c11a9ee43f33e130}

# J1
for x in range(1,1000,1):
    for y in range(1,1000,1):
        if(x**2 + 22*y**2 == 8383):
            print(str(x) + ' , ' + str(y))

ans 21 , 19
ans 45 , 17
Flag: mini{J1_c9d7861b2635ebb151b71351}

# G2
print("FIRST STAGE")
xmod5 = []
for x in range(1000000000,10000000000,1):
    if (x % 1277 == 616):
        xmod5.append(x)
print("SECOND STAGE")
xmod3911 = []
for y in xmod5:
    if (y % 3911 == 1892):
        xmod3911.append(y)
print("THIRD STAGE")
xmod6833 = []
for z in xmod3911:
    if (z % 6833 == 3267):
        xmod6833.append(z)
print("RESULT")
print(xmod6833)

ans 6429412122
output:
FIRST STAGE
SECOND STAGE
THIRD STAGE
RESULT
[6429412122]

Flag: mini{G2_9aa73c3f86221f07d9b789a9}
