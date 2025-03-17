### 📂 Automação de Tarefas  

#### 📄 `configurar-git.sh`  
✅ **Configura rapidamente nome, email e chave SSH do Git**  

```sh
#!/bin/bash

# Configurar nome e email
echo "Configurando Git..."
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"

# Gerar chave SSH
echo "Gerando chave SSH..."
ssh-keygen -t rsa -b 4096 -C "seu@email.com"

# Exibir chave SSH
echo "Sua chave SSH foi gerada! Copie e adicione ao GitHub:"
cat ~/.ssh/id_rsa.pub
```

📌 **Uso:**  
```sh
chmod +x configurar-git.sh  
./configurar-git.sh  
```

---

#### 📄 `criar-repositorio.sh`  
✅ **Cria um novo repositório, adiciona arquivos e faz o primeiro commit**  

```sh
#!/bin/bash

echo "Criando repositório Git..."
git init

echo "Criando README.md..."
echo "# Novo Projeto" > README.md

git add .
git commit -m "Primeiro commit"

echo "Digite a URL do repositório remoto:"
read repo_url
git remote add origin $repo_url
git push -u origin main

echo "Repositório configurado com sucesso!"
```

📌 **Uso:**  
```sh
chmod +x criar-repositorio.sh  
./criar-repositorio.sh  
```

---

#### 📄 `atualizar-repositorio.sh`  
✅ **Adiciona todas as mudanças, faz commit e envia para o GitHub**  

```sh
#!/bin/bash

echo "Adicionando mudanças..."
git add .

echo "Digite a mensagem do commit:"
read commit_msg

git commit -m "$commit_msg"
git push origin main

echo "Repositório atualizado com sucesso!"
```

📌 **Uso:**  
```sh
chmod +x atualizar-repositorio.sh  
./atualizar-repositorio.sh  
```

---

#### 📄 `clonar-repositorio.sh`  
✅ **Clona um repositório Git informando a URL**  

```sh
#!/bin/bash

echo "Digite a URL do repositório para clonar:"
read repo_url

git clone $repo_url

echo "Repositório clonado com sucesso!"
```

📌 **Uso:**  
```sh
chmod +x clonar-repositorio.sh  
./clonar-repositorio.sh  
```
