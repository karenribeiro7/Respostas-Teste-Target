# Questão 2: 
Dado a sequência de Fibonacci, onde se inicia por 0 e 1 e o próximo valor sempre será a soma dos 2 valores anteriores (exemplo: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34...), escreva um programa na linguagem que desejar onde, informado um número, ele calcule a sequência de Fibonacci e retorne uma mensagem avisando se o número informado pertence ou não a sequência.

IMPORTANTE:
Esse número pode ser informado através de qualquer entrada de sua preferência ou pode ser previamente definido no código;


## Resposta: 

sequencia_fibonacci = []
primeiro_valor = 0
segundo_valor = 1

termo_inicial = 3

termo_final = int(input("Digite quantos termos a sequência deve ter: "))

sequencia_fibonacci.append(primeiro_valor)
sequencia_fibonacci.append(segundo_valor)

while termo_inicial <= termo_final:

    proximo_valor = primeiro_valor + segundo_valor
    primeiro_valor = segundo_valor
    segundo_valor = proximo_valor
    sequencia_fibonacci.append(proximo_valor)
    termo_inicial = termo_inicial + 1


numero = int(input("Digite um valor: "))

if numero in sequencia_fibonacci:

    print("O numero pertence à Sequencia de Fibonacci!")
else:

    print("O número não pertence à Sequencia de Fibonacci!")