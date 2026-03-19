# notas-estudo
minhas notas de estudo do téc SENAC 2026

markdown

> ## Configurando git
> 

- para utilizar o git na minha máquina eu preciso configurar determinados passos e comandos, sendo eles:

- 1° abrir a aba do Windows e digitar "CMD"
    

2° digitar:

```bash

git config --global user.name "meu nome"

```

 ## 3°  enter

 ## 4° digitar

 ```bash
Git config --global user.email "meu email do GitHub"
```

 ## 5°  enter

> **## SSH- Como configurar a máquina para o GitHub**
> 
  *1° verificar se já há uma chave SSH com o comando:*

```bash

ls -al ~/.ssh

```

*2° abrir o git bash e criar nova chave com o comando:*

```bash

ssh-keygen -t ed25519 -C "meu email do GitHub"

```

 *3°  > enter 4x*

  *4° digitar*

```bash

eval "$(ssh-agent -s)"

ssh-add ~/ .ssh/id (tab)

```

 *5°  > enter*



 *6° copiar chave ssh com o comando:*

```bash

clip < ~/.ssh/id(tab).(tab)

```

- 7° entre no GitHub -> configurações -> SSH => nova chave -> cole a chave
- 8° testar conexão com o comando:

```bash

ssh -T git@github.com

```

> **## Como criar um repositório no GitHub**
> 
- Repositório é um projeto de git e para criar um é necessário os seguintes passos:

abrir o GitHub -> clicar na foto de perfil no canto superior direito -> selecionar repositórios -> clique em "New" no canto superior direito -> dê um nome ao repositório -> crie uma descrição -> defina se será público ou privado -> sempre ative o README

> **## Como clonar o repositório**
> 

abrir um repositório -> clicar em "<> code" -> selecionar "SSH" -> copiar -> abrir o Git blash -> digitar :

---

cd Documents/

**> enter -> *digitar*:**

git clone (clicar botão direito e selecionar "paste")

> enter 2x -> ***digitar***:

cd 'nome do repositório'

> enter -> *digitar:*

code .

*> enter*

## Index.Html 
ao entrar no vscode, você clica com o botão direito e clica em 'new file' 
e escreva: 'Index.html' e clica em enter;
ao entrar, você troca o 'en' por 'pt-br' 
e escreva 'src' dentro do body
após isso, você clica novamente com o botão direito e clica em 'new folder' e escreva: 'scripts' e enter
após isso você cria um arquivo com o nome: 'avaliação.js' e enter. 


## Alert e Prompt 

alert(): mostra mensagem na tela.
Prompt(): abre uma caixinha pro usuário comentar
*EXEMPLO:*
```bash
 alert('Olá!')
 const nome = prompt('Qual o seu nome?)
```

 ## Manipulação de DOM 
 o dom é a estrutura da página HTML 
 manipular o DOM: usar JavaScript para mudar elementos da páginas (cores, imagens.. etc)
 *EXEMPLO:* 
 ```bash
  document.getElementById('titulo').innerTex
  t = 'Novo titulo'
  ```
  ou seja, você faz o site mudar sem recarregar a página. 

  ## Estrutura de condição 
  server para tomar decisões no código 
  Usar IF, ELSE, ELSE IF 
*EXEMPLO:*
```bash
const idade = 18;
if(idade >= 18) {
    console.log('Maior de idade')
} else {
    console.log('Menor de idade'):
}
```
resumindo: O código escolhe o que fazer dependendo da situação.