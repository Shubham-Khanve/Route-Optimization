# Route-Optimization

import itertools
Aa=20
Ab=18
Ba=19
Bb=22
per=list(itertools.permutations([Aa,Ab,Ba,Bb],4))
A=20
B=30
a=15
b=35
n=0
m=0
x=0
while m<24:
	while n<4:
		if per[m][n]==20:
			if A==0 and B==0 and a==0 and b==0:
				x=x
			else:
				x=x+20
			if A>a:
				A=A-a
				a=0
			elif A<a:
				a=a-A
				A=0
			else:
				A=0
				a=0
			if A==0 and B==0 and a==0 and b==0:
				print (x)
		if per[m][n]==18:
			if A==0 and B==0 and a==0 and b==0:
				x=x
			else:
				x=x+18
			if A>b:
				A=A-b
				b=0
			elif A<b:
				b=b-A
				A=0
			else:
				A=0
				b=0
			if A==0 and B==0 and a==0 and b==0:
				print (x)
		if per[m][n]==19:
			if A==0 and B==0 and a==0 and b==0:
				x=x
			else:
				x=x+19
			if B>a:
				B=B-a
				a=0
			elif B<a:
				a=a-B
				B=0
			else:
				B=0
				a=0
			if A==0 and B==0 and a==0 and b==0:
				print (x)
		if per[m][n]==22:
			if A==0 and B==0 and a==0 and b==0:
				x=x
			else:
				x=x+22
			if B>b:
				B=B-b
				b=0
			elif B<b:
				b=b-B
				B=0
			else:
				B=0
				b=0
			if A==0 and B==0 and a==0 and b==0:
				print (x)
		n+=1
	n=0
	A=20
	B=30
	a=15
	b=35
	x=0
	m+=1
