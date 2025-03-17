### 📂 Exemplos práticos de uso do Git

#### Criando um Repositório Git  

```sh
# Criar uma pasta e entrar nela
mkdir meu-projeto && cd meu-projeto

# Iniciar o Git no projeto
git init

# Criar um arquivo e adicioná-lo ao repositório
echo "# Meu Projeto" > README.md
git add README.md
git commit -m "Adicionando README inicial"

# Conectar ao repositório remoto no GitHub
git remote add origin https://github.com/seu-usuario/meu-projeto.git

# Enviar para o GitHub
git push -u origin main
```

---
#### Clonando um Repositório Existente  

```sh
# Clonar um repositório do GitHub
git clone https://github.com/usuario/repositorio.git

# Acessar a pasta do repositório clonado
cd repositorio
```

---
 
#### Exemplo de `.gitignore`  

```plaintext
# Ignorar arquivos de log
*.log

# Ignorar pastas do sistema operacional
.DS_Store
Thumbs.db

# Ignorar dependências do Node.js
node_modules/

# Ignorar credenciais privadas
.env
```

---

#### Criando e Gerenciando Branches  

```sh
# Criar uma nova branch
git checkout -b minha-nova-branch

# Verificar todas as branches
git branch

# Alternar entre branches
git checkout main

# Mesclar uma branch na branch principal
git merge minha-nova-branch

# Excluir uma branch
git branch -d minha-nova-branch
```

---


#### Criando Commits Corretamente  

```sh
# Adicionar arquivos ao staging
git add .

# Criar um commit com mensagem clara
git commit -m "Adicionando nova funcionalidade X"

# Editar o último commit (caso não tenha sido enviado ainda)
git commit --amend -m "Nova mensagem do commit"
```

---

#### Resolvendo Conflitos no Git  

1. Faça `git pull origin main` para trazer as mudanças mais recentes.  
2. O Git pode exibir um **conflito** nos arquivos modificados.  
3. Edite os arquivos e escolha as alterações desejadas.  
4. Após resolver os conflitos, execute:  

```sh
git add .
git commit -m "Resolvendo conflito"
git push origin main
```
