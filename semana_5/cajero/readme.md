Funcion balance <- cashier ()

	Definir balance Como Real;
	balance = 1000;
	Repetir
		Imprimir "select an option:";
		Imprimir "a. to deposit.";
		Imprimir "b. withdraw.";
		Imprimir "c. go out.";
		leer option
		Si option = 'a' Entonces
			balance = balance + deposit()
		FinSi
		Si option = 'b' Entonces
			balance = balance - withdraw()
		FinSi
	Mientras Que option = "a" | option = "b"
Fin Funcion

Funcion value <- deposit()
	Imprimir "how much do you want to deposit:";
	leer value
FinFuncion

Funcion value <- withdraw()
	Imprimir "how much do you want to withdraw:";
	leer value
FinFuncion

Algoritmo exampleCashier
	Imprimir cashier()
FinAlgoritmo
