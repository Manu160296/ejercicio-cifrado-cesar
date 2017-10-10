# "Cifrado Cesar"

##### En este archivo encontraremos:
##### 1.-Breve descripción acerca del proyecto.
##### 2.-Pseudocódigo.
##### 3.-Diagrama de flujo.
***
#### 1.-Breve descripción del proyecto :
###### Este proyecto tiene como principal finalidad el cifrado y decifrado de cadenas de texto ;pide al usuario mediante un menú lo que desea hacer, este programa no admite espacios en blancos por lo que para ser más especificos cifra y descifra palabras.

***
#### 2.- Pseudocódigo :
###### A continuación presentaré el pseudocódigo de mi programa :
***NOMBRE DEL PRIMER PROCESO: cipher***

***VARIABLES : newPosition,newString***

***función*** cipher (string)    
***si***(el valor no es de tipo string)   
***retornar*** "Debe ingresar una cadena de texto"  
***si no ***
* string = ***convertir a mayúscula*** string;
newPosition = vacío;
***para*** todas las letras del string ***hacer***  
* ***agregar*** la posición de las letras del string del codigo ASCII a newPosition //con (string.charCodeAt(contador-65+33)%26+65)    
* newString= vacio;  
***para***
 todas las posiciones de newPosition ***hacer**
*  ***concatenar*** las nuevas posiciones cifradas ( codigo ASCII) de newPosition a newString
* ***retornar*** newString **fin**   


***NOMBRE DEL SEGUNDO  PROCESO: decipher***

***VARIABLES : newPosition,newString***

***función*** decipher (string)    
***si***(el valor no es de tipo string)   
***retornar*** "Debe ingresar una cadena de texto"  
***si no ***
* string = ***convertir a mayúscula*** string;
newPosition = vacío;
***para*** todas las letras del string ***hacer***  
* ***agregar*** la posición de las letras del string del codigo ASCII a newPosition //con (string.charCodeAt(contador-13-33)%26+65)  
* newString= vacio;  
***para***
 todas las posiciones de newPosition ***hacer**
*  ***concatenar*** las nuevas posiciones descifradas ( codigo ASCII) de newPosition a newString
* ***retornar*** newString **fin**   


***NOMBRE DEL SEGUNDO  PROCESO: decipher***

***VARIABLES :menu, string , secondString***  

***HACER:***     
menu="Cifrado Cesar ***salto de línea*** 1.Cifrar ***salto de línea*** 2.Descifrar ***salto de línea*** ";   
option = ***valor absoluto***(***pedir***(menu,0));
***si*** (option es absolutamente igual a 1)   
***hacer***
* string = ***pedir*** "Escriba la frase que desea cifrar";
***mientras***(el dato recibido  sea diferente de un string ***o*** se trate de un número);
***llamar*** cipher(string);  
***si no entonces*** (option es absolutamente igual a 2)   
***hacer***   
* secondString= ***pedir*** "Escriba la frase a descifrar"   
***mientras*** (el dato recibido  sea diferente de un string ***o*** se trate de un número);
***llamar*** decipher(secondString);   
***si no ***    
***alerta*** ( "Escoga una opcion del menu" );   

***MIENTRAS***(no haya una opción);    
***   
#### 3.- Diagrama de flujo :   

![diagrama tarjeta 1][1]  ![diagrama tarjeta 2][2]  ![diagrama tarjeta 3][3]

   [1]: assets/docs/diagrama_cifrado1.png
   [2]:assets/docs/diagrama_cifrado2.png   
   [3]: assets/docs/diagrama_cifrado3.png
