# Jogo_da_Adivinha
#Exercício Python 028: Escreva um programa que faça o computador "pensar" em um número inteiro entre 0 e 5 e peça para o usuário tentar descobrir qual foi o número escolhido pelo computador. # O programa deverá escrever na tela se o usuário venceu ou perdeu.

from random import randint
from time import sleep
computador = randint(0,5)
print(' Vou pensar em um número entre 0 a 5 ....')
print('-=-' *20 )
jogador =int(input('Em que numero eu pensei?'))
print('-=-' *20 )
print('PROCESSANDO...')
sleep(3)
if jogador == computador:
    print('PARABÉNS! VOCÊ CONSEGUIU ME VENCER!')
else:
    print('GANHEEEEI, EU PENSEI NO NÚMERO {}  E NÃO NO NÚMERO {}'.format(computador,jogador))
