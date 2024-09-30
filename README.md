# par e ímpar

from random import randint

computador = randint(1,10)
jogador = int(input('Escolha um número entre 1 e 10: '))

if jogador < 0 or jogador > 10:
    print('Jogue novamente. 1 a 10')
    exit()

soma = jogador + computador
jogadas = ('Ìmpar','Par')
jogadas_pi = int(input('Escolha 0 pra ÍMPAR OU 1 PARA par'))
computador_pi = ()

if jogadas_pi == 0 or jogadas_pi == 1:
    if jogadas_pi == 0:
        jogadas_pi = jogadas[0]
        computador_pi = jogadas[1]
    else:
        jogadas_pi = jogadas[1]
        computador_pi = jogadas[0]
else:
    print('Jogue novamente! Somente 0 ou 1')
    exit()

print(f'Você escolheu:{jogador_pi} e o computador:{computador_pi}')
