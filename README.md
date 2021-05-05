# Sistemas-Indebidos
/*
 * CAPITULO 2 : PUERTOS DIGUITALES 
 * CODIGO 1 : MANEJO DE PUERTOS CONFIGURADOS COMO SALIDAS 
 * OBJETIVO : ENCENDER Y APAGAR LEDS MEDIANTE EL USO DE DIFERENTES VARIABLES 
 * NOMBRE : ISRAEL ERAZO
 */

 /*VARIABLES: NUMERICAS ENTERAS (int),DECIMALES (float),CARACTERES (chart)
*/
const int led1 = 8; // uso de #define, es una varible que no se puede alterar su valor , no exista uan depuracion de errores*/
 const int led2 = 9; /* se puede considerar como variable normal*/
 const int led3 =10; /*variable constante , es la recomendable*/
 const int led4 =11; // Declara una cuarta variable para que ingrese otro led para el deber

void setup() {
  pinMode(led1,OUTPUT);   /*declaro el pin 8 como salida*/ 
  pinMode(led2,OUTPUT);   /*declaro el pin 9 como salida */
  pinMode(led3,OUTPUT);   /*declaro el pin 10 como salida */
   pinMode(led4,OUTPUT);   /*declaro el pin 11 como salida */

}

void loop() {
  //Para el deber nos pide que sea en forma asincrona entonces se mandara un encendiodo detras del otro al apagarse y asi se encendera de forma como pide el docente
   digitalWrite(led1,HIGH); /*Enviando 5 voltios al pin 8 */
   delay(500);              /*se detiene el microcontrolador por medio segundo */
   digitalWrite(led1,LOW);  /* envia 0 voltios al pin 8 */
   delay(500);              /* deteiene el microcontrolador */
  digitalWrite(led2,HIGH); /*Enviando 5 voltios al pin 9 */
   delay(500);              /*se detiene el microcontrolador por medio segundo */
   digitalWrite(led2,LOW);  /* envia 0 voltios al pin 9 */
   delay(500);             /*se detiene el microcontrolador por medio segundo */
    digitalWrite(led3,HIGH); /*Enviando 5 voltios al pin 10 */
   delay(500);              /*se detiene el microcontrolador por medio segundo */
   digitalWrite(led3,LOW);  /* envia 0 voltios al pin 10 */
   delay(500);              /* deteiene el microcontrolador */
   digitalWrite(led4,HIGH); /*Enviando 5 voltios al pin 10 */
   delay(500);              /*se detiene el microcontrolador por medio segundo */
   digitalWrite(led4,LOW);  /* envia 0 voltios al pin 10 */
   delay(500);              /* deteiene el microcontrolador */
   
}
