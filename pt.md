Phương trình bậc 2 python



from math import sqrt

a = float(input("Nhập a = "))
b = float(input("Nhập b = "))
c = float(input("Nhập c = "))

if a == 0:
	if b == 0:
		if c == 0:
			print("Phương trình vô nghiệm")
		else:
			print("Phương trình vô nghiệm")
	else:
		print("Phương trình có một nghiệm", -c/a)
else:
	delta = (b*b - 4*a*c)
	if delta < 0:
		print("Phương trình vô nghiệm")
	elif delta == 0:
		print("Phương trình có một nghiệm kép x1=x2=", (-b/2*a))
	else:
		print("Phương trình có 2 nghiệm phân biệt:")

		x1 = (-b + sqrt(delta))/2*a
		x2 = (-b - sqrt(delta))/2*a
		print("x1 =", x1)
		print("x2 =", x2)
