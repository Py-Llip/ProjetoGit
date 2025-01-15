Para renomear o branch principal em Git, você pode seguir as etapas abaixo. Antes de começar, certifique-se de que você está no branch que deseja renomear.

### 1. **Renomear o branch localmente**
Use o seguinte comando para renomear o branch localmente:

```bash
git branch -m <nome-atual> <novo-nome>
```

Se você já estiver no branch que deseja renomear, pode simplificar o comando:

```bash
git branch -m <novo-nome>
```

### 2. **Atualizar a referência no repositório remoto**
Depois de renomear o branch localmente, você precisa atualizar o branch remoto.

#### a. Exclua o branch antigo no remoto:
```bash
git push origin --delete <nome-antigo>
```

#### b. Publique o branch com o novo nome:
```bash
git push origin <novo-nome>
```

#### c. Configure o branch para rastrear o branch remoto:
```bash
git branch --set-upstream-to=origin/<novo-nome>
```

### 3. **Alterar o branch padrão no Git remoto (ex: GitHub ou GitLab)**
Acesse a interface do repositório remoto e altere o branch padrão para o novo nome. No GitHub:
1. Vá para **Settings** do repositório.
2. Clique em **Branches**.
3. Mude o branch padrão para o novo nome.

Depois, você pode deletar o branch antigo no repositório remoto se ainda não fez isso.

Se precisar de ajuda para adaptar os comandos ao seu cenário, é só avisar! 😊