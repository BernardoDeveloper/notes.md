Data: 2023-09-26
#tuning

---
- [[CODE - Second Brain]]

Source: [font](https://google.com)
Project: #project/project_name
Areas: #areas/area_name
Related: [[Life]]

# Conteúdo

## Aula 1
[Preparação, acerto de injeções](https://www.youtube.com/watch?v=tZqsY_kKPJ8)

REMAP - reprogramar uma injeção original.
Injeção Programavél - subistitui a original, ela é uma folha em branco.

**TABELAS 3D:**
As colunas são os RPMs - As linhas são pressão de admissão, mais pedal, mais borboleta.
Relacionada a acerto de combustivél.
Programação de injeção programavél é acertar combustivél e ingnição. Parte do acerto, é adicionar ou remover combustivél em determinada região.

**TPS:** Borboleta o quanto da borboleta está aberto -> Entrada de AR no motor
![[Pasted image 20230927124231.png]]

> ⚠️ **IMPORTANTE**: Estudar sobre kPa

**MAP (KPA):** pressão atmosférica, 95 +/- um motor aspirado não passa disso, somente motor turbo. Quando o motor pega ele trabalha em uma pressão menor do que a atmosférica.
![[Pasted image 20230927124607.png]]

Com base nesses dois valores se nessa exata condição eu preferir injetar mais gasolina na tabela eu altero o determinado valor.
![[Pasted image 20230927124851.png]]

## Aula 2
Sonda Lambda - para entender a base dos gráficos 3d;
Conectar computador na injeção: Cada injeção tem seu cabo: algumas são usb, ethernet, etc;

**De onde vem os valores das tabelas?**
- Você precisa testar o seu motor para saber o que ele "quer";

Sonda Lambda: um sensor para *exaustão* ele fica no escape. É um sensor ligado na injeção do carro. Quem ajuda a acertar a quantidade de Injeção ar/combustivél.
![[d63230_23446762e1e64e1491eeffa45a7b39d0~mv2.webp]]

E com base nos valores passados pela sonda podemos informar pela injeção o quanto irá entrar de combustivél, no injetor, através da tabela, porque a injeção controla esses valores.
`+ combustivél` ele deixa o bico injetor aberto por \+ tempo;

Quanto maior o tempo de injeção, de \+ combustivél, menor o valor da sonda. Se eu remover combustivél o valor da sonda subiu. Quando temos valores menores na sonda obtemos uma **mistura RICA (gorda)** e quando o valor da sonda está acima de 1.00 temos uma **mistura POBRE (magra)**.
- *Enriquecer:* mais combustivél no cilindro;
- *Empobrecer:* menos combustivél cilindro;
![[Pasted image 20230927202843.png]]

**Sonda:** também usada para encontrar problemas;
1. Por exemplo um dos cilindros caso eu desativar o mesmo a sonda fica mais pobre o valor fica alta, pois passa muito ar, porque no tempo de aspiração terá somente entrada de ar.
2. Se eu remover o cabo -> a mistura fica mais pobre, pois ainda está saindo *oxigênio*, não teve a explosão o *oxigênio* ainda continua ele não foi transformado em gás, então vai sair mais *oxigênio* do que *gás* com isso mistura **POBRE**

##### Nome técnico:
Sonda Lambda -> Sensor de **oxigênio**;
Ou seja ela mede a quantidade de **oxigênio** que está saindo do escape.

