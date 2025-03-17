
### 📄 **`.gitignore`**  
💡 **Define quais arquivos e pastas devem ser ignorados pelo Git**  

```plaintext
# 🔹 Arquivos do sistema operacional
.DS_Store
Thumbs.db

# 🔹 Logs
*.log
npm-debug.log*
yarn-debug.log*
yarn-error.log*

# 🔹 Dependências do Node.js
node_modules/
package-lock.json
yarn.lock

# 🔹 Dependências do Python
__pycache__/
*.pyc
*.pyo
*.pyd
venv/

# 🔹 Ambientes virtuais do Pipenv e Poetry
.Python
pip-log.txt
pip-delete-this-directory.txt
poetry.lock

# 🔹 Arquivos de compilação do Java
*.class
*.jar
*.war
*.ear
target/

# 🔹 Arquivos de configuração do JetBrains IDEs (IntelliJ, PyCharm, WebStorm, etc.)
.idea/
*.iml

# 🔹 Configurações do VS Code
.vscode/

# 🔹 Arquivos do Linux e MacOS
*.swp
*~
```

---

### 📌 **Como usar**  
Basta adicionar este arquivo na raiz do seu projeto e o Git ignorará automaticamente os arquivos listados.  
