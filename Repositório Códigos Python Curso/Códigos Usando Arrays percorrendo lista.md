```python
salario_mensal = input('Digite seu salário mensal:' )
salario_mensal = float(salario_mensal)

gastos_mensais = input('Digite seu gasto mensal:')
gastos_mensais = float(gastos_mensais)

salario_anual = salario_mensal * 12
gastos_anuais = gastos_mensais * 12

montante_anual = salario_anual - gastos_anuais
print('Vc pode economizar por ano R$', montante_anual)

```

    Digite seu salário mensal:1350
    Digite seu gasto mensal:1300
    Vc pode economizar por ano R$ 600.0
    


```python
valor_passagem = 4.40

valor_corrida = input('Digite o valor da corrida')
if float (valor_corrida) <= valor_passagem * 5:
        print ('pague a corrida')
else:
        print('vá de ônibus')
```

    Digite o valor da corrida30
    vá de ônibus
    


```python
valor_passagem = 4.40

valor_corrida = input('Digite o valor da corrida')
if float (valor_corrida) <= valor_passagem * 5:
        print ('pague a corrida')
else:
    if float (valor_corrida) <= valor_passagem * 6: 
        print('aguarde, valor pode baixar')
    else:
        print('vá de onibus')
```

    Digite o valor da corrida23
    aguarde, valor pode baixar
    


```python
idade = int(input('Digite sua idade:'))
if idade >= 12:
    print('Legal, vc já tem altura.')


altura = float(input('Digite sua altura, em metros:'))
if idade >= 12 and altura >= 1.60:
    print('Você pode entrar na montanha russa.')
print('Obrigado por participar.')
```

    Digite sua idade:11
    Digite sua altura, em metros:1.50
    Obrigado por participar.
    


```python
idade = int(input('Quantos anos vc tem?: '))
altura = float(input('Qual é a sua altura?: '))

if idade >= 15 and altura >=1.60:
    print('Acesso ao briquedo liberado!')
else:
    print('Vc não atendeu um dos requisitos para acesso!')
        
```

    Quantos anos vc tem?: 14
    Qual é a sua altura?: 1.60
    Vc não atendeu um dos requisitos para acesso!
    


```python
idade = int(input('Digite sua idade:'))
if idade >= 12:
    resposta = input('Você gostaria de entrar nesta montanha russa?')
    if (resposta == 'sim'):
        print('Por favor, entre!')
    else:
        print('Ok então')
else:
    print('Você não tem idade suficiente para entrar nesse brinquedo.')
```

    Digite sua idade:12
    Você gostaria de entrar nesta montanha russa?não
    Ok então
    


```python
exercicio = int(input('Quantos tempo de academia vc fez?: '))
if exercicio > 35:
    print('Vc está perto do seu objetivo!')
elif exercicio >= 20:
    print('Está bom, mas pode melhorar!')
elif exercicio >= 15:
    print('Precisa ajustar seu tempo')
else:
    print('Dessa forma, não atingirá seus objetivos')
```

    Quantos tempo de academia vc fez?: 20
    Está bom, mas pode melhorar!
    


```python
contador = 0

while contador < 10:
    contador = contador + 1
    if contador == 1:
        print(contador, 'item limpo')
    else:
        print(contador, 'itens limpos')
        
print('Fim da repetição do bloco')
```

    1 item limpo
    2 itens limpos
    3 itens limpos
    4 itens limpos
    5 itens limpos
    6 itens limpos
    7 itens limpos
    8 itens limpos
    9 itens limpos
    10 itens limpos
    Fim da repetição do bloco
    


```python
texto = input('Digite sua senha: ')

while texto != 'mvcsantana':
    texto = input('Senha Inválida, tente novamente:   ')
        
print('Acesso Permitido')
        
   
```


    ---------------------------------------------------------------------------

    KeyboardInterrupt                         Traceback (most recent call last)

    ~\AppData\Local\Temp/ipykernel_10472/3444885308.py in <module>
    ----> 1 texto = input('Digite sua senha: ')
          2 
          3 while texto != 'mvcsantana':
          4     texto = input('Senha Inválida, tente novamente:   ')
          5 
    

    ~\AppData\Local\Programs\Python\Python310\lib\site-packages\ipykernel\kernelbase.py in raw_input(self, prompt)
       1004                 "raw_input was called, but this frontend does not support input requests."
       1005             )
    -> 1006         return self._input_request(
       1007             str(prompt),
       1008             self._parent_ident["shell"],
    

    ~\AppData\Local\Programs\Python\Python310\lib\site-packages\ipykernel\kernelbase.py in _input_request(self, prompt, ident, parent, password)
       1049             except KeyboardInterrupt:
       1050                 # re-raise KeyboardInterrupt, to truncate traceback
    -> 1051                 raise KeyboardInterrupt("Interrupted by user") from None
       1052             except Exception:
       1053                 self.log.warning("Invalid Message:", exc_info=True)
    

    KeyboardInterrupt: Interrupted by user



```python
horario = int(input('Que horas são?  '))
#testando o laço com o if...
if 0 < horario < 6:
        print('Vc está na madrugada')
else:
        print('Não é de madrugada')
```

    Que horas são?  5
    Vc está na madrugada
    


```python
horario = 9
#testando o laço com while

while 0 < horario < 6:
    print('Vc está na madrugada')
    break
    
else:
        print('Não é de madrugada')
```

    Não é de madrugada
    


```python
salario = float(input('Digite o salário atual válido: '))
    
while salario < 998.0:
        salario = input('Digite um salário maior que o mínimo 998.0:  ')
        
else:
        print('Faixa Salarial Aprovada!')
```

    Digite o salário atual válido: 1000.00
    Faixa Salarial Aprovada!
    


```python
# Declaramos um contador como 0:
contador = 0
# Definimos o número de repetições:
numero = int(input('Digite um numero: '))
# Rodamos o while até o contador se igualar ao número de repetições:
while contador < numero:
    print(contador)
    contador = contador + 1
```

    Digite um numero: 5
    0
    1
    2
    3
    4
    


```python
lista_paises = ['Brasil', 'Portugual', 'Alemanha']
print(lista_paises)
```

    ['Brasil', 'Portugual', 'Alemanha']
    


```python
print('Tamanho da lista:', len(lista_paises))
```

    Tamanho da lista: 3
    


```python
print('País:', lista_paises[2])

```

    País: Alemanha
    


```python
print('País:', lista_paises[-1])
```

    País: Alemanha
    


```python
print(lista_paises[1:2])
```

    ['Portugual']
    


```python
print('Brasil' in lista_paises)
```

    True
    


```python
lista_capitais = []
lista_capitais.append('Brasilia')
lista_capitais.append('São Paulo')

print(lista_capitais)
```

    ['Brasilia', 'São Paulo']
    


```python
lista_capitais.remove('Brasilia')
print(lista_capitais)
```

    ['São Paulo']
    


```python
lista_capitais.pop(0)
print(lista_capitais)
```

    []
    


```python
numeros = [1, 2, 3, 4, 5]
indice = 0
while indice < 3:
    print(numeros[indice])
    indice = indice + 1
```

    1
    2
    3
    


```python
numeros = [1, 2, 3, 4, 5]
indice = 0
while indice < len(numeros):
    print(numeros[indice])
    indice = indice + 1
```

    1
    2
    3
    4
    5
    

      


```python
pessoas = []
resposta = 's'
while resposta == 's':
    resposta = input('Deseja adicionar alguém (s/n)?')
    if (resposta == 's' or resposta =='S'):
        nome = input('Qual o nome desta pessoa:  ')
        pessoas.append(nome) #adiciona um nome pessoa /á lista
        print(pessoas, 'Adicionada')  
```


```python
print(pessoas)
```


```python
 print(pessoas)
```

    []
    


```python
empresa = 'Google'
print(empresa)
```


```python

```
