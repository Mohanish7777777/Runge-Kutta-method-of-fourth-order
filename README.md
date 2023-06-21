# Runge-Kutta-method-of-fourth-order

Find 𝒚(𝟎. 𝟐), given that 𝒅𝒚 = 𝒙 + 𝒚𝟐, 𝒚(𝟎) = 𝟏 using Runge-Kutta fourth order method

Program:
```python3
def f (x, y):
return x+y**2
x0=float (input ("Enter initial point of x: "))
y0=float (input ("Enter initial point of y: "))
h=float (input ("Enter step value h: "))
k1=h*f (x0, y0)
k2=h*f (x0+h/2,y0+k1/2)
k3=h*f (x0+h/2,y0+k2/2)
k4=h*f (x0+h,y0+k3)
y=y0+(k1+2*k2+2*k3+k4)/6
print ("The value of y using RK method is %.4f"%y)
```
Output:
Enter initial point of x: 0
Enter initial point of y: 1
Enter step value h: 0.2
The value of y using RK method is 1.2735
