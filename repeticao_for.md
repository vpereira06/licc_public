
# Estruturas de repetição: for

Conteúdo:
- Repetição com `for i in range()`
- Repetição com `for c in "string"`
- Tipo **String** e comprimento `len()`

Diferentemente do loop com `while`, que depende necessariamente de uma condição, o loop com `for` gera uma repetição por um número definido de vezes.


```python
# exemplo de funcionamento de loop while
while condição == True:
    print('repete até que condição seja falsa')
```

O loop `for` gera a repetição por um número N de vezes.


```python
for i in range(10):
    print(i)
```

    0 1 2 3 4 5 6 7 8 9 


```python
for i in range(1, 9):
    print(i)
```

    1 2 3 4 5 6 7 8 


```python
for i in range(1, 10, 2):
    print(i)
```

    1 3 5 7 9 


```python
inicio = 10
fim = 100
passo = 5

for i in range(inicio, fim, passo):
    print(i)
```

    10 15 20 25 30 35 40 45 50 55 60 65 70 75 80 85 90 95 


```python
for i in range(1, 11):
    for j in range(1, 11):
        print('{} * {} = {} \t'.format(i, j, i*j))
```

    1 * 1 = 1 	
    1 * 2 = 2 	
    1 * 3 = 3 	
    1 * 4 = 4 	
    1 * 5 = 5 	
    1 * 6 = 6 	
    1 * 7 = 7 	
    1 * 8 = 8 	
    1 * 9 = 9 	
    1 * 10 = 10 	
    
    
    2 * 1 = 2 	
    2 * 2 = 4 	
    2 * 3 = 6 	
    2 * 4 = 8 	
    2 * 5 = 10 	
    2 * 6 = 12 	
    2 * 7 = 14 	
    2 * 8 = 16 	
    2 * 9 = 18 	
    2 * 10 = 20 	
    
    
    3 * 1 = 3 	
    3 * 2 = 6 	
    3 * 3 = 9 	
    3 * 4 = 12 	
    3 * 5 = 15 	
    3 * 6 = 18 	
    3 * 7 = 21 	
    3 * 8 = 24 	
    3 * 9 = 27 	
    3 * 10 = 30 	
    
    
    4 * 1 = 4 	
    4 * 2 = 8 	
    4 * 3 = 12 	
    4 * 4 = 16 	
    4 * 5 = 20 	
    4 * 6 = 24 	
    4 * 7 = 28 	
    4 * 8 = 32 	
    4 * 9 = 36 	
    4 * 10 = 40 	
    
    
    5 * 1 = 5 	
    5 * 2 = 10 	
    5 * 3 = 15 	
    5 * 4 = 20 	
    5 * 5 = 25 	
    5 * 6 = 30 	
    5 * 7 = 35 	
    5 * 8 = 40 	
    5 * 9 = 45 	
    5 * 10 = 50 	
    
    
    6 * 1 = 6 	
    6 * 2 = 12 	
    6 * 3 = 18 	
    6 * 4 = 24 	
    6 * 5 = 30 	
    6 * 6 = 36 	
    6 * 7 = 42 	
    6 * 8 = 48 	
    6 * 9 = 54 	
    6 * 10 = 60 	
    
    
    7 * 1 = 7 	
    7 * 2 = 14 	
    7 * 3 = 21 	
    7 * 4 = 28 	
    7 * 5 = 35 	
    7 * 6 = 42 	
    7 * 7 = 49 	
    7 * 8 = 56 	
    7 * 9 = 63 	
    7 * 10 = 70 	
    
    
    8 * 1 = 8 	
    8 * 2 = 16 	
    8 * 3 = 24 	
    8 * 4 = 32 	
    8 * 5 = 40 	
    8 * 6 = 48 	
    8 * 7 = 56 	
    8 * 8 = 64 	
    8 * 9 = 72 	
    8 * 10 = 80 	
    
    
    9 * 1 = 9 	
    9 * 2 = 18 	
    9 * 3 = 27 	
    9 * 4 = 36 	
    9 * 5 = 45 	
    9 * 6 = 54 	
    9 * 7 = 63 	
    9 * 8 = 72 	
    9 * 9 = 81 	
    9 * 10 = 90 	
    
    
    10 * 1 = 10 	
    10 * 2 = 20 	
    10 * 3 = 30 	
    10 * 4 = 40 	
    10 * 5 = 50 	
    10 * 6 = 60 	
    10 * 7 = 70 	
    10 * 8 = 80 	
    10 * 9 = 90 	
    10 * 10 = 100 	
    
    



```python
for i in range(10, 0, -1):
    print(i)
```

    10 9 8 7 6 5 4 3 2 1 


```python
for letra in 'palavra':
    print(letra)
```

    p
    a
    l
    a
    v
    r
    a


Como saber o tamanho de uma **String**?


```python
len('Newton')
```




    6




```python
frase = 'O scrum é uma metodologia para desenvolvimento de software'
tamanho = len(frase)

print('O comprimento da frase é', tamanho)
```

    O comprimento da frase é 58


## Imprimindo tabelas


```python
print('{}\t {}\t {}\t {}'.format('n', 'n2', 'n3', 'n4'))
for i in range(11):
    print('{}\t {}\t {}\t {}'.format(i, i**2, i**3, i**4))
```

    n	 n2	 n3	 n4
    0	 0	 0	 0
    1	 1	 1	 1
    2	 4	 8	 16
    3	 9	 27	 81
    4	 16	 64	 256
    5	 25	 125	 625
    6	 36	 216	 1296
    7	 49	 343	 2401
    8	 64	 512	 4096
    9	 81	 729	 6561
    10	 100	 1000	 10000


Para fazer a tabulação entre uma coluna e outra é bem simples: só utilizar `\t` no `print`

# Exercícios

1. Desenvolva um script para mostrar todos os números pares e seus respectivos valores ao quadrado menores que 100.
2. Faça um programa que mostre o resultado final da soma de todos os números ímpares entre 100 e 500.
3. Faça um programa que leia 5 números e informe a soma e a média dos números. 
4. O Sr. Manoel Joaquim possui uma grande loja de artigos de R\$ 1,99, com cerca de 10 caixas. Para agilizar o cálculo de quanto cada cliente deve pagar ele desenvolveu um tabela que contém o número de itens que o cliente comprou e ao lado o valor da conta. Desta forma a atendente do caixa precisa apenas contar quantos itens o cliente está levando e olhar na tabela de preços. Você foi contratado para desenvolver o programa que monta esta tabela de preços, que conterá os preços de 1 até 50 produtos, conforme o exemplo abaixo: 
<pre>
Lojas Quase Dois - Tabela de preços
1 - R$ 1.99
2 - R$ 3.98
...
50 - R$ 99.50</pre>

5. Faça um programa que leia uma frase digitada pelo usuário e imprima essa frase ao contrário.
<pre>A aula de hoje acabará tarde
edrat árabaca ejoh ed alua A
</pre>


```python

```
