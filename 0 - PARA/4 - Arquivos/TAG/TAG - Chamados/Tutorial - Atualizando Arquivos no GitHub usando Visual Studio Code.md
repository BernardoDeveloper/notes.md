Este tutorial fornecerá uma introdução passo a passo sobre como atualizar arquivos em um repositório do GitHub usando o Visual Studio Code. Vamos lá!

## Pré-requisitos

1. **Visual Studio Code:** Certifique-se de ter o Visual Studio Code instalado. Você pode baixá-lo aqui.
    
2. **Conta no GitHub:** É necessário ter uma conta no GitHub. Se ainda não tiver, crie uma aqui.
    

## Passos

### 1. Clone o Repositório

- Abra o Visual Studio Code.
- Pressione `Ctrl + Shift + P` (Windows/Linux) ou `Cmd + Shift + P` (Mac) para abrir a paleta de comandos.
- Digite "Git: Clone" e selecione a opção. Cole a URL do repositório e escolha um local para clonar.

### 2. Abra o Projeto

- No Visual Studio Code, vá em "File" > "Open Folder" e selecione a pasta do seu projeto clonado.

### 3. Faça Alterações nos Arquivos

- Faça as alterações necessárias nos arquivos do projeto.

### 4. Salve as Alterações

- Salve os arquivos modificados pressionando `Ctrl + S` (Windows/Linux) ou `Cmd + S` (Mac).

### 5. Abra o Terminal Integrado

- No Visual Studio Code, pressione `Ctrl +` `(Windows/Linux) ou`Cmd + (Mac) para abrir o terminal integrado.

### 6. Adicione as Alterações

- Digite o comando `git add .` para adicionar todas as alterações ao stage.

### 7. Faça um Commit

- Digite o comando `git commit -m "Mensagem do commit"` para realizar um commit com uma mensagem descritiva das alterações feitas.

### 8. Faça o Push para o GitHub

- Digite o comando `git push origin NOME_DA_BRANCH` para enviar as alterações para o repositório no GitHub.

### 9. Autenticação

- Você será solicitado a inserir suas credenciais do GitHub para autenticar o push.

### 10. Verifique as Alterações no GitHub

- Acesse o repositório no GitHub e verifique se as alterações foram refletidas.