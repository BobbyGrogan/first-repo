import math


def quadratic(a, b, c):
    d = b**2-4*a*c
    if d < 0:
        print("No real solutions")
    elif d == 0:
        x = (-b+math.sqrt(b**2-4*a*c))/2*a
        print("This equation has one solution: ", x)
    else:
        x1 = (-b+math.sqrt(b**2-4*a*c))/2*a
        x2 = (-b-math.sqrt(b**2-4*a*c))/2*a
        print("This equation has two solutions: ", x1, " and", x2)

quadratic(1, 8, 16)
