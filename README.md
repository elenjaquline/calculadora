# calculadora
codigo de calculadora
# Código de calculadora em Python

def soma(a, b):
    return a + b

def subtracao(a, b):
    return a - b

def multiplicacao(a, b):
    return a * b

def divisao(a, b):
    if b == 0:
        raise ValueError('Não é possível dividir por zero.')
    return a / b

operacao = input('Qual operação você deseja fazer (+, -, *, /)? ')
num1 = float(input('Digite o primeiro número: '))
num2 = float(input('Digite o segundo número: '))

if operacao == '+':
    resultado = soma(num1, num2)
elif operacao == '-':
    resultado = subtracao(num1, num2)
elif operacao == '*':
    resultado = multiplicacao(num1, num2)
elif operacao == '/':
    resultado = divisao(num1, num2)
else:
    print('Operação inválida.')

print('Resultado: ', resultado)
