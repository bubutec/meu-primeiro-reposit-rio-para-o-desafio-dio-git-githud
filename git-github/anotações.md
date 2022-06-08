# Anotações úteis do curso de git/github.



### Comandos básico para criar uma chave SSH

- **ssh-keygen -t ed25519 -C email cadastrado no github** - cria uma chave SSH.
- **cat nome da chave criada.pub** - mostra o conteudo da chave publica criada.
- **eval $(ssh-agent -s)** - inicia o agente de cheves ssh.
- **ssh-add nome da chave **- insere a chave no agente ssh. obs. pedirá pra criar uma senha no processo.



### Comandos básico de terminal git:

- **git init ** - para iniciar um novo repositório git local.
- **git status** - para verificar se há modificaçoes a serem feitas antes de adicionar a lista de commit.
- **git add** "os arquivos a serem adicionados" - para adicionar os arquivos modificados a lista para commit.
- **git commit -m "mensagem da commit"** - faz o verionamento dos arquivos modificados (um snap).
- **git config --global user.email "email cadastrado no github" ** - configura o email que está na sua conta github no seu git.
- **git config --golbal user.name "nome cadastrado no github" ** - configura o nome que está na sua conta github.
- **git remote add [nome desejado para essa entrada] [endereço do repositório remoto desajado]** - faz com que congiure um repositorio remoto ao seu repositório local para depois fazer um push.
- **git remote -v ** - lista todos os repositórios remotos configurados para aquele repositório local.
- **git push [nome do endereço do repositório remoto adicionado] [nome da branch]** - empurra as modificações do seu repositório git local para o remoto github.
- **git pull [nome do endereço do repositório remoto adicionado] [nome da branch]** - pucha a versão que está no repositório remoto para o repositório local para fazer comparações de alterações.
- **git clone [endereço do repositório remoto]** - clona o repositório remoto para maquina local. **obs:** se o repositório não for publico, irá pedir login e senha; se for um endereço ssh, deverá antes configurar uma chave ssh na maquina local.
