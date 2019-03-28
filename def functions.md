
# Funções

Funções são definidas com o uso da palavra reservada `def`. 


```python
def mostra_nome():
    print('Newton Calegari')
    
mostra_nome()
mostra_nome()
mostra_nome()
```

    Newton Calegari
    Newton Calegari
    Newton Calegari
    

Uma função é executada somente quando ela é acionada.
Para declarar uma função utilizamos **def** *nome_da_funcao()*, mas para aciona-las somente percisamos chamar pelo nome *nome_da_funcao()*.

No contexto de programação, **função** é uma sequência nomeada de instruções ou comandos, que realizam uma oper- ação desejada. Esta operação é especificada numa **definição de função**.

A função pode ter qualquer nome que você escolher, mas não pode ter uma palavra reservada do Python.

** Importante lembrar que todo o conteúdo da função, ou seja, as intruções que foram criadas dentro da função devem ser INDENDATAS**


```python
def nome_da_minha_funcao():
    numero = 10
    soma = numero + 20
    texto = input('Digite algum texto: ')
    print(texto)
```

### Usando Docstring para documentar as funções


```python
def fatorial(n):
    '''
    Objetivo: Recebe um número inteiro e retorna o seu fatorial
    Parâmetros de entrada: n (int)
    Retorno: fat (int)
    Pré-condição: numero n é inteiro e positivo.
    '''
    # em seguida vem o código para o cálculo do fatorial.
    
    return fat
```

### Funções frutíferas

As funções frutíferas são as que retornam algum valor, ou seja, que possuem o a instrução **`return`**.

As funções que não retornam nenhum valor são chamadas, em alguns contextos, de **procedimentos**.

### Escopo das variáveis nas funções

As variáveis utilizadas dentro de um função possuem seu escopo restrito à execução da função. Ou seja, ela é válida somente no escopo da função.


```python
nome = "Newton"

def mostra_nome():
    nome = "Calegari"
    print(id(nome))

print(nome)
```

    Newton
    

## Exercícios

- Faça um programa que receba a partir de `input` o nome e o salário dos funcionários de uma empresa para exibi-los na tela juntamente com a alíquota e valor de IRPF. Ex:

```
        Funcionário(a)     Salário         Alíquota    IR
        Warren Buffet      R$ 3980,00      22,5%       R$ 995,00```

- Faça uma função que receba como entrada um salário e devolva o valor da alíquota do IRPF de acordo com os critérios abaixo:

    - Até 1.903,98 - isento
    - De 1.903,99 até 2.826,65 - Aliquota de 7,5%
    - De 2.826,66 até 3.751,05 - Aliquota de 15%
    - De 3.751,06 até 4.664,68 - Aliquota de 22,5%
    - Acima de 4.664,68 - Aliquota de 27,5%





```python

```
