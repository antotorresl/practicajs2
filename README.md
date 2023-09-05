import random

def simular_tirada_ruleta():
    # Generar un número aleatorio entre 5 y 10 vueltas
    vueltas = random.randint(5, 10)
    
    # Inicializar la posición en 0
    posicion = 0
    
    # Realizar las vueltas
    for _ in range(vueltas):
        # Generar un número aleatorio entre 0 y 36
        numero = random.randint(0, 36)
        # Actualizar la posición
        posicion = (posicion + numero) % 37
    
    return posicion

# Simular 10 tiradas
for i in range(10):
    resultado = simular_tirada_ruleta()
    print(f"Nro de juego: {i + 1}")
    print(f"Valor Aleatorio Generado: {resultado}")
    print(f"Nro que cayó en la ruleta: {resultado}")
    print()
