// Obtener la hora actual
const horaActual = new Date();
const horaActualEnMilisegundos = horaActual.getTime();

// Generar un número aleatorio de minutos entre 300 (5 horas) y 600 (10 horas)
const minutosAleatorios = Math.floor(Math.random() * (600 - 300 + 1)) + 300;

// Calcular la hora final sumando los minutos aleatorios a la hora actual
const horaFinalEnMilisegundos = horaActualEnMilisegundos + minutosAleatorios * 60000; // 1 minuto = 60000 milisegundos

// Convertir la hora final de milisegundos a una fecha
const horaFinal = new Date(horaFinalEnMilisegundos);

// Formatear la hora actual y la hora final en formato HH:mm
const formatoHora = { hour: '2-digit', minute: '2-digit' };
const horaActualFormateada = horaActual.toLocaleTimeString(undefined, formatoHora);
const horaFinalFormateada = horaFinal.toLocaleTimeString(undefined, formatoHora);

// Imprimir los resultados
console.log(`Hora Actual: ${horaActualFormateada}`);
console.log(`Valor Aleatorio Generado en Minutos: ${minutosAleatorios}`);
console.log(`Hora Final: ${horaFinalFormateada}`);
//Este código obtendrá la hora actual, generará un número aleatorio de minutos entre 300 
//(5 horas) y 600 (10 horas), y luego calculará la hora final sumando esos minutos a la hora actual.
//Finalmente, formateará las horas en un formato legible y las imprimirá.





