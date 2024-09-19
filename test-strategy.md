Errores encontrados:
No realizaba random del 1 al 100
Los intentos estaban solo al 5
No validaba los numeros decimales
SOLUCION DEL PROYECTO
se cambio la logica la random del numero para que escogiera un numero del 1 al 100
 let randomNumber = Math.floor(Math.random() * 100) + 1;
 Se cambio el numero de intentos
  const MAX_ATTEMPTS = 10;
 y para solucionar el ultimo error encontrado se implemento la siguiente validacion, la cual valida que si un numero es mayor a 1 o si es
 mayor a 100 o si tiene punto decimal.
 if (isNaN(numero) || numero  < 1 || numero > 100 || numero % 1 !== 0 ) {
        alert('Por favor, ingresa un número entero válido entre 1 y 100.');
        guessField.value = '';
        guessField.focus();
        return;
 



