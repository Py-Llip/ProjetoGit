Para apagar um **branch** no Git, você pode fazer isso **localmente** ou **remotamente** no repositório GitHub.

Aqui estão os passos:

---

### **1. Apagar um branch localmente**

#### **Comando:**
Para apagar um branch local, use:
```bash
git branch -d nome-do-branch
```

- **`-d`** é para apagar o branch, mas ele **verifica se o branch foi mesclado** (merge) com o branch principal (como o `main`) antes de permitir a exclusão. Se o branch não foi mesclado, o Git vai impedir para evitar perder alterações.

Se você **tem certeza** de que quer excluir o branch, mesmo que não tenha sido mesclado, use:
```bash
git branch -D nome-do-branch
```

#### **Exemplo:**
Para apagar um branch chamado `nova-funcionalidade`:
```bash
git branch -d nova-funcionalidade
```

---

### **2. Apagar um branch remoto (GitHub)**

Para apagar um branch **remoto** (no GitHub), você usa o comando `git push` com o formato de "deletar".

#### **Comando:**
```bash
git push origin --delete nome-do-branch
```

#### **Exemplo:**
Para apagar o branch remoto `nova-funcionalidade`:
```bash
git push origin --delete nova-funcionalidade
```

---

### **3. Verificar se o branch foi apagado**

- Para **verificar os branches locais**, use:
  ```bash
  git branch
  ```

- Para **verificar os branches remotos**, use:
  ```bash
  git branch -r
  ```

---

### **Importante**:
- Não é possível apagar o **branch atual**. Você precisa mudar para outro branch antes de apagá-lo (geralmente, para `main` ou outro branch).
  
Por exemplo:
```bash
git checkout main
git branch -d nome-do-branch
```

Esses são os comandos principais para apagar um branch. Se precisar de mais explicações ou se tiver outra dúvida, só avisar! 😊