# meucomecopython
Aqui consegui fazer meu primeiro desafio em Python quase sozinho.


from datetime import datetime
import random

print('- - - - - Olá! Seja muito bem-vindo ao meu GitHub! - - - - -')
nome = input('Qual é o seu nome?')
anosIdade = input('Quantos anos você tem?')
cartoes = ['R$50,00', 'R$250,00', 'R$120,00']
cartao = random.choice(cartoes)
data_cadastro = datetime.now()
aniversario = datetime.strptime(
    input('Digite a sua data de aniversário no formato dd/mm/aaaa: '), '%d/%m/%Y')

print(f'Olá {nome}, seu registro foi concluído com sucesso no dia {data_cadastro.day}/{data_cadastro.month}/{data_cadastro.year}.\nParabéns, houve um sorteio e você ganhou um cartão de compras no valor de {cartao}')
