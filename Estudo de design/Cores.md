RGB o led da tela, sendo: RED - GREEN - BLUE
para ficar mais fácil criamos o sistema hexadecimal nesse sistema através de um código podemos definir o quanto queremos de azul, verde e vermelho somente com 6 caracteres.
Temos um sistema de 0-15 a partir do 9 utilizamos letras:
![[Pasted image 20240122211836.png]]

Conta para transformar em RGB:
![[Pasted image 20240122211923.png]]

Sempre multiplica o primeiro *número* por 16, no exemplo do primeiro 16x8 e depois somamos o restante red: $16*8+4$ green: $16*13+5$ blue: $16*0+2$

HSB: realmente todas as caracteristicas da cor com três elementos, a cor a saturação da cor e o brilho dessa cor.

## Função das cores em um site
#### Contraste
Uma das partes mais **importantes da web**. Por exemplo um site preto tem um botão amarelo, ele irá ter um contraste muito forte em relação ao fundo, um título eu contrasto com um texto na tela.

#### Acessibilidade
Um bom **contraste** é muito importante para ter uma boa acessibilidade pois sem contraste fica tudo muito parecido, temos as diretrizes da [WCAG](https://www.w3.org/Translations/WCAG20-pt-br/) - [[Resumo sobre a diretriz de contraste WCAG]] - um cálculo que verfica as cores para saber se tem um bom contraste, por exemplo o maior contraste Branco com preto, o cálculo retorna notas como AAA, AA ou FAIL:

![[Pasted image 20240124203521.png]]

Temos muitas ferramentas para verificar se o contraste entre as cores está bom uma de exemplo é o [Contrast Ratio](https://www.siegemedia.com/contrast-ratio). No ==figma== podemos utilizar o **plugin contrast** com um texto selecionado, podemos executar o plugin e receberemos a nota:

![[Pasted image 20240124204332.png]]

> Ponto Importante: sempre ter **contraste**;

#### Hierarquia:
Com as cores, podemos definir a hirarquia das informações, um exemplo seria dar enfase a algum elemento da tela, para isso podemos definir uma cor que não é utilizada na página por exemplo.

#### Informação:
As cores servem com uma informação ao usuário, por exemplo:

![[Pasted image 20240124205431.png]]

#### Identidade:
A cor é utilizada para criar uma identidade, um projeto por exemplo pode associar uma cor a marca como o vermelho da Coca-Cola, dar identidade ao site é uma função da cor.
No inspetor de elementos do navegador podemos saber qual a nota do WCAG.

[[Como definir uma paleta de cores]]
