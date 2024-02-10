Source: Bernardo
Related: [[1 - Aprendizado, Treinamentos]]

---

Funções em *advpl*

- Function: função da totvs - fontes padrão que a TOTVS criam
- User Function: função criada por programadores
- Static Function: função estática que pode ser chamada por outra - uma auxiliar que pode ser executada por outras, enxergada dentro do fonte criado.

> `#include` código fontes com funções para ser usadas

*tlpp* arquivos para programar, criar programas no Protheus.

### Variaveis
Local: Somente dentro da função
Private: Em todo código fonte
Public: Disponivél para todos os outros programas

Uma variavél *pública* com o mesmo nome de uma *privada* a *privada* irá derrubar a pública;

Syntaxe:

```prw
// Instanciar: topologia nome as tipo (tipo opcional)
Local nNota1 as Integer
Local nNota2

// Atribuir valor
nNota1 := 10
nNota2 := 8.5
```

#### Tipos de variaveis:

```prw
/**
Numérico: 3 / 21.000 / 0.4 / 2000
Boolean: .T. / .F.
Caractere: "D" / "C"
Data: DATE()
Array: {"Val1", "Val2", "Val3"}
Bloco: {||VALOR := 1,MsgAlert("Valor: " + cValToChar(valor))}
*/
```

#### Funções para manipular array
AADD() -> Inserir um item em um array
AINS() -> Inserir um elemento em qualquer posição do array
ACLONE() -> Copia um array para outro
ADEL() -> Exclui um elemento do array, subistituindo seu valor por `null`
ASIZE() -> Redefine a estrutura de array pre-existente
LEN() -> tamanho do array

Seguem o padrão de parâmetro -> (array_name, value)

### Definições do ADVPL, Protheus e Fluig
PRW: advpl
TLPP: advpl maior abordagem
RPO: Repositórios
RDMAKE: conjunto de fontes
ICMS: Imposto

SF4: tabela de cadastro de TES