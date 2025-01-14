Olá esse projeto ensina você a usar o Git
Isso é uma alteração
Aqui estão os comandos básicos para usar o Git e enviar seu projeto para o GitHub:

Para criar um **novo branch** e voltar para o **branch `main`**, você pode seguir os passos abaixo:

---

### **1. Criar um novo branch:**
Para criar um novo branch, basta usar o comando `git branch`:
```bash
git branch nome-do-novo-branch
```
Por exemplo:
```bash
git branch nova-funcionalidade
```

### **2. Mudar para o novo branch:**
Após criar o branch, você precisa "mudar" para ele com o comando `git checkout`:
```bash
git checkout nova-funcionalidade
```

Agora, você está trabalhando no branch `nova-funcionalidade`. A partir daqui, você pode fazer alterações e commits nesse branch.

---

### **3. Voltar para o branch `main`:**
Quando quiser voltar para o branch `main`, use o comando `git checkout` novamente:
```bash
git checkout main
```

---

### **4. (Opcional) Criar e mudar de branch em uma única linha:**
Você pode criar e já mudar para o novo branch em um único comando:
```bash
git checkout -b nome-do-novo-branch
```
Por exemplo:
```bash
git checkout -b nova-funcionalidade
```

### **5. (Opcional) Verificar os branches existentes:**
Para ver todos os branches no seu repositório, use:
```bash
git branch
```
Isso vai mostrar uma lista de todos os branches e qual está ativo (marcado com `*`).

---

Esses são os passos básicos para trabalhar com branches no Git. Caso tenha mais dúvidas, só perguntar! 😊