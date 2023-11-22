# studious-JR
import random

def gerar_numeros_loteria(qtd_numeros, minimo, maximo):
    numeros_loteria = set()

    while len(numeros_loteria) < qtd_numeros:
        numero_sorteado = random.randint(minimo, maximo)
        numeros_loteria.add(numero_sorteado)

    return sorted(list(numeros_loteria))

# Exemplo de uso
qtd_numeros = 6
minimo = 1
maximo = 60

numeros_sorteados = gerar_numeros_loteria(qtd_numeros, minimo, maximo)
print(f'Números da loteria: {numeros_sorteados}')
