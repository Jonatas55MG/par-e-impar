# par e ímpar

from random import randint

computador = randint(1,10)
jogador = int(input('Escolha um número entre 1 e 10: '))

if jogador < 0 or jogador > 10:
    print('Jogue novamente. 1 a 10')
    exit()

soma = jogador + computador
jogadas = ('Ìmpar','Par')
jogadas_pi = int(input('Escolha 0 pra ÍMPAR OU 1 PARA par: '))
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
                              # ÍMPAR
if jogadas_pi == 'Ìmpar' and soma%2==1:
    print('Você venceu!')
    print(f'Você:{jogador}, o computador{computador}, a soma:{soma}.')
                               #PAR
elif jogadas_pi == 'Par' and soma%2==0:
    print('Você venceu!')
    print(f'Você:{jogador}, o computador:{computador}, a soma:{soma}.')
                                    #ÍMPAR
elif computador_pi == 'ìmpar' and soma%2==1:
    print('Computador venceu!')
    print(f'Você:{jogador}, o computador:{computador}, a soma:{soma}.')
    
else:
    print('Computador venceu!')
    print(f'Você:{jogador}, o computador:{computador}, a soma:{soma}.')
