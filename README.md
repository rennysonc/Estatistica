# Estatística 
Repositório criado com a finalidade de postagem dos códigos e anotações que tive durante as aulas da disciplina de Estatística Aplicada a Computação.

# Utilizando o Jupyter Notebook / Jupyter Lab
# Aula de Estatistica 

Listas

- Mutáveis.
- Ordenadas.
- Heterogêneas.
- Indexada por posição.
- Delimitada por Colchetes.

lista = ['casa', 1.0,3]

type(lista)

lista[0]

lista[1]

lista[2]

lista[-1]

Um problema serio com listas!

a = [1,2,3]

a

a*3

b = []
for i in a:
    b.append(i*3)
b

Dicionarios

- Não mutaveis.
- Não ordenados.
- Heterogeneos .
- Indexada por chaves.
- delimitadas por chaves.

dicionario = {"nome":"rennyson","idade":18,"cidade":"nazarezinho"}

type(dicionario)

dicionario["idade"]

dicionario["nome"]

ndarray - Numpy

- A biblioteca numpy cria uma nova estrutura de dados, tem uma grande capacidade de vetorização que possibilita que qualquer operação feita com estrutura ja feita elemento a elemento sem a necessidade de um laço para acessar esses elementos, tornando, assim, a operação mais eficiente.

import numpy as np

np.array([-2,4.4,7,9])

Existem varias formas de criar arrays, pode ser através do método np.array{}:

1. usando uma lista:

arr = np.array([-2,4,7,9])
arr

**OBS: A lista deve ser homonogenea.**
ORDEM: String > complex > float > int 

ex: se a lista tiver só inteiros o resultado dará só inteiros,
se a lista tiver um float e o resto inteiro ele converte todos para float

2. usando o método arange: **np.arange(inicio, fim , passo)**

arr = np.arange(1,32,2)
arr

3. usando o método linspace: **np.linspace (inicio, fim, quantidade)**

arr = np.linspace(1, 100, 10)
arr

4. outros métodos

arr1 = np.empty((6,4)) ##array vazia com o método empty() normalmente a saída lida
arr1

arr2 = np.eye(4) #eye cria uma array de duas dimensões com 1 na diagonal e 1 linha
arr2

Criar as arrays de A E B para fazer operações com elas

A = np.arange(10)
B = np.arange(10,38,3)
c = np.array([2,3,4,5,6,7,8,9, np.nan , np.nan])
print('\nA:' , A , '\nB:', B, '\nc:',c)

A+c

somar = A + B
subtrair = A - B
multiplicar = A * B
dividir = A / B

print('\n\nsomar: ', somar)
print('\nsubtrair: ',subtrair)
print('\ndividir: ', dividir)
print('\nmultiplicar:', multiplicar)


