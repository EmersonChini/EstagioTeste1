﻿# EstagioTeste1
def is_fibonacci_number(n):
    if n < 0:
        return False

    # Inicializa a sequência de Fibonacci
    a, b = 0, 1
    
    # Continua gerando números de Fibonacci até que o número informado seja alcançado ou ultrapassado
    while a < n:
        a, b = b, a + b

    # Verifica se o número pertence à sequência
    return a == n

# Número a ser verificado
number = 13

# Verifica se o número pertence à sequência de Fibonacci
if is_fibonacci_number(number):
    print(f"O número {number} pertence à sequência de Fibonacci.")
else:
    print(f"O número {number} NÃO pertence à sequência de Fibonacci.")
