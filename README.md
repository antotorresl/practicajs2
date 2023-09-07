// Generar un número aleatorio que represente la posición inicial entre 0 y 359 grados.
const posicionInicial = Math.floor(Math.random() * 360);

// Generar un segundo número aleatorio para las vueltas entre 5 y 10 vueltas.
const vueltas = Math.floor(Math.random() * 6) + 5;

// Calcular el ángulo final sumando las vueltas a la posición inicial.
const anguloFinal = (posicionInicial + vueltas * 360) % 360;

// Imprimir los resultados.
console.log(`Posición o ángulo Inicial G.A.: ${posicionInicial}`);
console.log(`Valor Aleatorio Generado en Grados: ${vueltas * 360}`);
console.log(`Ángulo Final: ${anguloFinal}`);
