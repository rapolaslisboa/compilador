# AC2 - Compiladores
Mateus Daemon - 171043
<br />
Rápolas Lisboa Senwaitis - 163057

## Definição da linguagem (Marie#)
Nesta seção é feita a definição da linguagem.

### Função principal equivalente

```
none Entry()
~

~
```

### Operadores aritméticos, relacionais e lógicos

Os operadores da linguagem **Marie#** são:

**Aritméticos**: +, -, *, /, %, ^, ++ (incremento).

**Relacionais**: eq (igual a), dt (diferente de), lt (menor que), gt (maior que), lte (menor igual) e gte (maior igual).

**Lógicos**: && (E lógico), || (OU lógico), ! (NÃO lógico).


### Tipos de variáveis

| Tipo (Marie#)  | Equivalente (TypeScript) |
| :-------------: |:-------------:|
| none     | void     |
| word    | string     |
| number      | number     |

### Declaração e atribuição de valor à variável

Exemplos de atribuição de valor à variável:

```
number Numero: 0
```

```
word Palavra: 'Compiladores'
```

### Estrutura (s) de decisão

```
if (A gt B)
~
  return A
~
```

```
else if (A eq B)
~
  return A + B
~
```

```
else
~
  return B
~
```

### Estrutura (s) de repetição

```
loop (number i: 1 to 100)
~
  log(i)
~
```

### Declaração de função

```
none PrintaCemAUm()
~
  loop (number i: 1 to 100)
  ~
    log(i)
  ~
~
```

###  Exemplos de código

**Exemplo 1**:

```
none Entry
~
  number Resultado: 0
  number Numero1: 10
  number Numero2: 20
  
  Resultado: DivideNumeros(Numero1, Numero2)
  log(Resultado)
~

number DivideNumeros(number N1; number N2)
~
  if (N1 gt N2)
  ~
    return N1 / N2
  ~
  else
  ~
    return N2 / N1
  ~
~
```

**Exemplo 2**:

```
none Entry
~
  number Resultado: 0
  number Numero1: 5
  number Numero2: 3
  
  Resultado: SomaNumeros(Numero1, Numero2)
  log(Resultado)
~

number SomaNumeros(number N1; number N2)
~
  return N1 + N2
~
```

**Exemplo 3**:

```
none Entry
~
  PrintaCemAUm()
~

none PrintaCemAUm()
~
  loop (number i: 1 to 100)
  ~
    log(i)
  ~
~
```

