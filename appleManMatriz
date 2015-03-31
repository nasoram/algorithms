import sys

def appleMan(casillas,p):
	conteo = 0
	for i in xrange(1,p-1):
		for j in xrange(1,p-1):
			if casillas[(i*p)+j-1] == 'o':
				conteo += 1
			if casillas[(i*p)+j+1] == 'o':
				conteo += 1
			if casillas[p*(i-1)+j] == 'o':
				conteo += 1
			if casillas[p*(i+1)+j] == 'o':
				conteo += 1
			if conteo%2 != 0:
				return "NO"
	return "YES"
	
n=input()
while n!=0:
	tablero = []
	for i in xrange(n+2):
		tablero.append('x')
	for i in xrange(n):
		linea=sys.stdin.readline().strip()
		linea='x'+linea+'x'
		for j in xrange(n+2):
			tablero.append(linea[j])
	for i in xrange(n+2):
		tablero.append('x')
	print appleMan(tablero,n+2)
	n=input()
