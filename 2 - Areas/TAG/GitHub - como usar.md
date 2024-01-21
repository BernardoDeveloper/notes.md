Requisitos: ter o Git instalado no computador.

## Terminal:

Primeiro você precisa estar com o acesso a [organização (um grupo) da Tag System no GitHub](https://github.com/Tag-System)
Depois crie uma pasta no seu computador, e abra o terminal para poder executar os seguintes comandos:

```sh
# clonar o repostitório - baixar a pasta do projeto
git clone https://github.com/Tag-System/Fontes-ADVPL.git

# acesse a pasta criada
cd Fontes-ADVPL
```

Com a pasta do projeto na sua máquina, quando precisar subir um novo arquivo ou código, execute o seguinte:

```sh
# Sincronize a sua pasta com as atualizações do respositório
git pull

# Adicione as alterações que você fez no commit
git add .

# Crie um commit com uma frase que explique o que você alterou
git commit -m "funcionalidade: criada uma função que faz X coisa"

# Envie suas alterações para o respoitório na branch main
git push -u origin main
```

## GitHub Desktop (aplicativo):

Instale o programa executável no [site do GitHub](https://desktop.github.com/) instale o aplicativo e configure a sua conta:
![[Pasted image 20240118081950.png]]

Depois escolhe o projeto que você quer executar:
![[Pasted image 20240118082033.png]]

Em seguida informe o local que irá baixar/copiar o projeto na sua máquina.

No canto superior esquerdo, você pode acessar repostitório > Abrir em Visual Studio Code e terá o seu projeto pronto para codificar.
![[Pasted image 20240118082306.png]]

Quando você alterar uma parte no código no painel esquerdo terá os arquivos que foram alterados, e ao clicar nesse arquivo mostra as alterações que foram realizadas:
![[Pasted image 20240118082438.png]]

Para enviar suas alterações para o repositório do GitHub, clique no botão da imagem acima que está como Fetch origin (ele irá sincronizar seu computador com o respositório).
Em seguida informe o que você alterou, e clique no botão azul.
![[Pasted image 20240118082603.png]]

Na parte superior o botão será atualizado ficando como Push (enviar os arquivos) ao clicar as suas alterações estarão no repositório:
![[Pasted image 20240118082710.png]]