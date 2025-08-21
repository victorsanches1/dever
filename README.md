# dever
# 1
numero = int(input('Digite o seu primeiro numero: '))
numero2 = int(input('Digite seu segundo numero: '))


def number (numero,numero2):
    
    if numero > numero:
      print(f'o numero maior é {numero}')

    elif numero == numero2:
            print('sao iguais')
    else:
      print(f'o maior numero é {numero2}')
      
number(numero,numero2)


# 2
numero = int(input('digite o numero para tabuada: '))

print(f'\tabuada do {numero}:\')
for i in range(1,11):
resultado  = * i 
print(f'{numero} x {i} = {resultado}')
