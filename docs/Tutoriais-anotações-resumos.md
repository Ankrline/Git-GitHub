
### 📂 Documentação  

## Introdução ao Git  

O **Git** é um sistema de controle de versão distribuído que permite rastrear mudanças em arquivos, facilitando o trabalho em equipe e a organização do código. Criado por **Linus Torvalds**, ele é amplamente utilizado por desenvolvedores.  

### 🔹 Benefícios do Git  
✅ Versionamento de código  
✅ Trabalho colaborativo  
✅ Histórico de alterações  
 
## Comandos Básicos do Git  

```sh
# Configurar nome e email
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"

# Criar um repositório
git init

# Clonar um repositório
git clone <URL_DO_REPO>

# Adicionar arquivos ao staging
git add .

# Criar um commit
git commit -m "Mensagem do commit"

# Enviar mudanças para o repositório remoto
git push origin main

# Atualizar código do repositório remoto
git pull origin main
```

## Trabalhando com Branches  

Branches permitem desenvolver novas funcionalidades sem afetar o código principal.  

```sh
# Criar uma nova branch
git branch minha-branch

# Alternar para a branch criada
git checkout minha-branch

# Criar e mudar para a nova branch
git checkout -b minha-branch

# Mesclar uma branch na principal
git checkout main
git merge minha-branch

# Deletar uma branch
git branch -d minha-branch
```

## Fluxos de Trabalho no GitHub  

O GitHub utiliza diferentes fluxos de trabalho para gerenciar projetos:  

🔹 **Git Flow** – Utiliza branches para organizar o desenvolvimento.  
🔹 **GitHub Flow** – Processo simplificado, focado em integração contínua.  

### 🔄 **Passos do GitHub Flow**  
1️⃣ Criar uma branch para a funcionalidade.  
2️⃣ Desenvolver e commitar as alterações.  
3️⃣ Criar um **Pull Request** para revisão.  
4️⃣ Mesclar a branch no `main`.  
5️⃣ Deletar a branch após a fusão.  

## O que é um Pull Request?  

No GitHub, um **Pull Request (PR)** é um pedido para mesclar mudanças de uma branch para outra.  

### ✅ **Como Criar um PR?**  
1️⃣ Subir as alterações para o GitHub.  
2️⃣ Acessar o repositório e clicar em **New Pull Request**.  
3️⃣ Escolher a branch de origem e a branch de destino.  
4️⃣ Adicionar uma descrição e enviar o PR.  
5️⃣ Esperar a aprovação e realizar o merge.  
 
## Configuração Inicial do Git  

```sh
# Definir nome e email
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"

# Verificar configurações
git config --list

# Criar uma chave SSH para autenticação com o GitHub
ssh-keygen -t rsa -b 4096 -C "seu@email.com"

# Exibir chave SSH para adicionar ao GitHub
cat ~/.ssh/id_rsa.pub
```
