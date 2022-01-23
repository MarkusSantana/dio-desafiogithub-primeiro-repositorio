```python
nomes_cidades = ['são paulo', 'londres', 'tóquio', 'paris']
for nome in nomes_cidades:
    print(nome)
```

    são paulo
    londres
    tóquio
    paris
    


```python
contador = 0 
nome_cidades = ['são paulo', 'londres', 'tóquio', 'paris']
while contador < len(nomes_cidades):
    print(nome_cidades[contador])
    contador = contador + 1
```

    são paulo
    londres
    tóquio
    paris
    


```python
for numero in range(10):
    print(numero)
```

    0
    1
    2
    3
    4
    5
    6
    7
    8
    9
    


```python
for numero in range(10, 0, -1):
    print(numero)
    
```

    10
    9
    8
    7
    6
    5
    4
    3
    2
    1
    


```python
def hello():
    print('Olá, Mundo')
    
hello()
```

    Olá, Mundo
    


```python
def calcula_media(valor1, valor2, valor3):
    soma = valor1 + valor2 + valor3
    media = soma / 3
    return media
resultado = calcula_media(9, 10, 8)
print(resultado)
```

    9.0
    


```python
resultado2 = calcula_media(valor1 = 9, valor2 = 10, valor3 = 9)
print(resultado2)
```

    9.333333333333334
    


```python
def dadospessoais(nome, idade, cidade):
    print("Seu nome é {}, você tem {} anos e mora em {}.".format(nome, idade, cidade))
dadospessoais("Marcus", 37, "Salvador")
```

    Seu nome é Marcus, você tem 37 anos e mora em Salvador.
    


```python
def somatorio(lista):
    soma = 0
    for item in lista:
        soma = soma + item
        
    return soma

numeros = [1, 2, 3, 4, 5]
soma_dos_numeros = somatorio(numeros)
print("A soma dos elementos da lista vale: ", soma_dos_numeros)


```

    A soma dos elementos da lista vale:  15
    


```python
if somatorio(numeros) > 50:
    print("Valor Alto!")
else:
    print("Valor Baixo!")
    
```

    Valor Baixo!
    


```python
def funcaorecursiva(numero):
    if (numero != 1):
        funcaorecursiva(numero - 1)
    print(numero)
    
print("Testando função recursiva: ")
funcaorecursiva(10)
```

    Testando função recursiva: 
    1
    2
    3
    4
    5
    6
    7
    8
    9
    10
    


```python

```
