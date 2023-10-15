Source: Microcontroladores - PIC
Project: #project/studies 
Areas: #areas/microcontroller
Related: [[C - Notes]]

---

Tipos short em microcontroladores são bem-vindo pois utilizam menos memória, por exemplo o int ao invés de ocupar 8 bits irá ocupar 1 lógico com seu range de valores mais reduzidos, também conhecido como *flag* ou *sinalizador*.

**Compilador CCS:** existem tipos próprios para microcontroladores:

| Tipo | Valor |
| --- | --- |
| Int1 | 1 bit |
| boolean | bit equivalente short int - baseados no shor int e int |
| int8 | 8 bits |
| byte | int e int8 |
| int16 | long int |
| int 32 | 32 bits |

Diretiva `#type` modifica o tamanho dos tipos;
Nome de variavél não pode exceder: 31 caracteres;
