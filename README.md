//Calcula el promedio de una lista de N datos

Algoritmo Promedio
	
	Escribir "Ingrese la cantidad de datos:"
	Repetir
		
		Leer n
		Si n<=0 Entonces
			Escribir "El número debe ser positivo y distinto de cero."
			Escribir "Introduzca un número válido."
		Fin Si
		Mientras n<-0 Hacer
			Escribir "Valor nulo, por favor intentelo de nuevo"
			Leer n
		Fin Mientras
	Hasta Que n>0
	
	acum<-0
	
	Para i<-1 Hasta n Hacer
		Escribir "Ingrese el dato ",i,":"
		Repetir
			Leer dato
			Si dato<0 Entonces
				Escribir "El dato debe ser positivo."
				Escribir "Ingrese el dato ",i,":"
			Fin Si
		Hasta Que dato>=0
		
		acum<-acum+dato
	Fin Para
	
	prom<-acum/n
	
	Escribir "El promedio es: ",prom
	Escribir "Para salir pulsa 0"
	leer salir
	
FinAlgoritmo
