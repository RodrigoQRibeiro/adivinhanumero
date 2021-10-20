# adivinhanumero
Código para gerar número aleatório, usuário adivinhar e mostrar número de tentativas após acertado.
from random import randint
print ('{:-^30}'.format (' Vamos brincar? '))
n = int (input ('Digite um número de 0 a 100: '))
c = int (0)
a = randint(0,100)
while (n!=a):
    if n>a:
        print ('O valor digitado é maior que o número do computador.')
        n = int (input ('Digite novamente o número: '))
        c += 1
    else:
        print ('O valor digitado é menor que o número do computador.')
        n = int (input ('Digite novamente o número: '))
        c += 1
print ('O número escolhido pelo computador foi {}. Você acertou em {} tentativas.'.format(a, c))
