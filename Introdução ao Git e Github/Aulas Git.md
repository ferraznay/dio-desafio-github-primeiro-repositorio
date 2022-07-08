# Introdução ao Git :computer:

### Comando para o windowns 

- DIR - LISTAR TODAS AS PASTAS

- CD .. - DESCER O NIVEL DA PASTA

- CD WINDOWS - ENTRA NA PASTA Q EU QUERO

- DIR MOSTRA TODO O CONTEUDO DA PASTA

- MKDIR WORKPACE - CRIA UMA PASTA

- CLS - LIMPA O PROMPT

- echo hello > hello.txt - para criar um arquivo txt dentro da pasta

- dell workspace - deleta todos os arquivos que estão dentro do repositorio

- rmdir workspace /S /Q - remove o diretorio workspace

  

### Tópico fundamentais para o funcionamento do Git

SHA1

A sigla SHA significa Secure Hash Algorithm. É um conjunto de funçõe criptográficas pela NA (de segurança nacional dos EUA) Essa encriptação gera um conjunto único de 40 caractere que erve como identificador.Cada mudança gera um novo conjunto.



### Objetos fundamentais :open_file_folder:

Tipos básicos de objetos responsáveis por versionamento de código:

* Blobs: Contém o tamanho da string/arquivo, uma \0 e o conteúdo do arquivo. obs: gera metadados, por isso os componentes extras.

* Árvores: Armazenam os blobs metadados, Também vai conter: \0, apontar para blobs, com sha1 e guardando artigos, diferentes do blobs sha1.

* Commits: o mais importante é o objeto que vai se juntar a todos, datá sentido a tudo que está sendo feito, pois:

  1. Aponta para uma árvore;
  2. realizado para o parente (último commit realizado antes dele)
  3. aponta para um autor 
  4. aponta para uma mensagem

  ### Chaves SSH e Tokens :closed_lock_with_key:

* Chave ssh: forma de estabelecer conexão seguyra e criptografada entre duas máquinas.

Criando comandos ssh:

1. ssh-keygen -t ed25591 -C **"**seu e-mail**"**
2. digitar senha
3. ir até a massa salva
4. verificar os arquivoss: dir, deve retornar a chave publica e privada
5. cat para exibir o conteúdo das chaves
6. copiar a saída, deve sser sua chave pública e colar no github
7. iniciar o ssh-agent apartir do código ssh-add(chave)
8. após entrar com a senha retornará o resultado de identidade e-mail, e seu usuario 
9. está feito a ligação



### Criando um diretorio 

(TODO COMANDO DO GIT LEVA O TERMO **"**GIT**"** NA FRENTE)

- git init = inicia o git 

- ls -a = exibe pasta ocultas

  ### Configurando o git

  git config --global user email **"**seu e-mail do github**"**

  git config --global user.name **"**seu nome de usuario no git**"**

  git commit -m **"**commit inicial**"**

  

- Empurrar os arquivos do ambiente de desenvolvimento para o remoto

  1.  git remote add origin **"**link do seu apelido conhecido**"**
  2. git push origin main/master

## Resolvendo conflito

Conflito de fusão: quando xistem duas mudanças na mesma linha e tentar ubir. o github aciona o erro para que o programador resolve. Ao tentar comitar uma nova versão, uma mensagem de conflito será dada.

Processo de resolução:

1. git pull = função irá trazer o conteúdo do GitHub para a máquina

2. as possibilidades feitas no arquivo

3. o processo de impulso deve ser iniciado novamente

   