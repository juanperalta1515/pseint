# pseint reloj
Definir hora, minutos, segundoss como Entero;
// SEGUNDOSS ESTA DEFINIDO CON DOBLE "S" YA QUE PSEINT TIENE OTRA DEFINICION PARA "SEGUNDO"
	Escribir "Escribe Hora actual";
	leer hora;
	escribir "Escribe minutos actuales";
	leer minutos;
	Escribir "Escribe segundos";
	leer segundoss;
	
	Mientras hora <=23 hacer
		mientras minutos <=59 hacer
			mientras segundoss <=59 hacer
				Limpiar Pantalla;
				si hora > 9 entonces 
					Escribir hora sin saltar;
				sino
					Escribir "0", hora sin saltar;
				Finsi
				
					si minutos > 9 entonces 
						Escribir ":", minutos sin saltar;
					sino 
						Escribir ":0", minutos sin saltar;
					
					
					FinSi
					si segundoss > 9 entonces
						Escribir ":",segundoss;
					SiNo
						Escribir ":0",segundoss;
						
						
					FinSi
					segundoss <- segundoss+1;
					Esperar 1 segundo;
				
					
				FinMientras
				segundoss <- 0;
				minutos <- minutos +1;
				
			FinMientras
			minutos <- 0;
			hora <- hora +1;
			si hora == 24 entonces
				hora <- 0;
			FinSi
			
	FinMientras
	
