# <H1>PROYECTO #1 juego del ahorcado 
<H1><center> PSEINT</CENTER ></H1>

    Algoritmo JuegoDeAdivinanza

    palabra_oculta = "juego"

    intentos = 10
    intentos_realizados = 0
    palabra_clave = ""
	
    Para i desde 1 hasta Longitud(palabra_oculta) hacer
        palabra_clave = palabra_clave + "_"
    Fin Para
	
    Mientras (intentos_realizados < intentos) y (palabra_clave <> palabra_oculta) hacer
        Escribir "Palabra Adivinada:", palabra_clave
        Escribir"Tienes ", intentos - intentos_realizados, " intentos restantes."
        Escribir("Ingrese una Letra: ")
        Leer letra
		
        Para i desde 1 hasta Longitud(palabra_oculta) hacer
            Si palabra_oculta = letra entonces
                palabra_clave = letra
            Fin Si
        Fin Para
		
        Si palabra_clave = palabra_oculta entonces
            Escribir "¡FELICIDADES! GANASTE, ERES MUY BUENO:", palabra_clave
        Sino
            Escribir "HAS PERDIDO. TUS 10 INTENTOS SE AGOTARON. SIGUE PARTICIPANDO. La palabra era:", palabra_oculta
        Fin Si
		
        intentos_realizados = intentos_realizados + 1
    Fin Mientras
Fin Algoritmo

# <H1><center> C++</CENTER ></H1>

#include <iostream>

#include <string>

int main() {
	std::string palabraOculta = "juego";
	int intentos = 10;
	int intentosr = 0;
	
	std::string palabraClave(palabraOculta.length(),'_');
	
		for(; intentosr <intentos && palabraClave != palabraOculta; ++intentosr){
			std::cout<<"palabra Adivinada:"<<palabraClave <<std:: endl;
			char a;
			std::cout<<"Ingrese una Letra: ";
			std::cin >>a;
			
			
			
			
		for(int b = 0; b <palabraOculta.length(); ++b){
				if(palabraOculta[b]==a){
					palabraClave[b] =a;
				}
			}
			
		}
	 
	if (palabraClave == palabraOculta){
		std::cout<<"FELICIDADES GANASTE ERES MUY BUENO: "<<palabraClave <<std::endl;
		
		}
	else{
		std::cout<<"HAS PERDIDO TUS 10 INTENTOS SIGUE PARTICIPANDO. la palabra ERA: "<<palabraOculta<<std::endl; 
		
	}
	
	
	
	
	return 0;
}

# <H1><center> PHYTON</CENTER ></H1>
juego de ahorcado

<h4>

    palabra_oculta = "juego"

    intentos = 10
    intentos_realizados = 0
    palabra_clave = '_' * len(palabra_oculta)

    while intentos_realizados < intentos and palabra_clave != palabra_oculta:
    print("Palabra Adivinada:", palabra_clave)
    letra = input("Ingrese una Letra: ")

    palabra_clave = ''.join(letra if palabra_oculta[i] == letra else palabra_clave[i] for i in range(len(palabra_oculta)))
    intentos_realizados += 1

    if palabra_clave == palabra_oculta:
    print("¡FELICIDADES! GANASTE, ERES MUY BUENO:", palabra_clave)
        else:
    print("HAS PERDIDO. TUS 10 INTENTOS SE AGOTARON. SIGUE PARTICIPANDO. La palabra era:", palabra_oculta)  </h4>#   j _ a h o r c a d o  
 