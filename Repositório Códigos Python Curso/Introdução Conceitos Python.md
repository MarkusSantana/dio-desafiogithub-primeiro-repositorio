```python
empresa = 'Google'
print(empresa)
```

    Google
    


```python
nome = 'Marcus'
idade = 37
filhos = 2
print('{} tem {} e possui {}' .format(nome, idade, filhos))
```

    Marcus tem 37 e possui 2
    


```python
preco_gasolina = 6.788
print('O preço da gasolina é R$ {:.2f}'.format(preco_gasolina))
```

    O preço da gasolina é R$ 6.79
    


```python
nome = 'Marcus'
idade = 37
filhos = 2

print ('f {nome} tem {idade} e possui {filhos} filhos.')
```

    f {nome} tem {idade} e possui {filhos} filhos.
    


```python
dia = 1
mes = 11
ano = 21
data1 = '{}/{}/{}'.format(dia, mes, ano)
print(data1)
```

    1/11/21
    

 dados_cidade = {
    'nome': 'São Paulo',
    'estado': 'São Paulo',
    'area_km2': 1521,
    'populacao': 12.18,

}
print(type(dados_cidade))


```python
dados_cidade['pais'] = 'Brasil'
print(dados_cidade)
```

    {'nome': 'São Paulo', 'estado': 'São Paulo', 'area_km2': 1521, 'populacao': 12.18, 'pais': 'Brasil'}
    


```python
dados_cidade_2 = dados_cidade
print(dados_cidade['nome'])
```

    São Paulo
    


```python
dados_cidade_3 = dad
```
