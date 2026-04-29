# CT-001 — Testes de Login

## Informações gerais
| Campo | Detalhe |
|-------|---------|
| **Módulo** | Autenticação |
| **Versão** | 1.0 |
| **Autor** | [Seu Nome] |
| **Data** | 2024 |

---

## CT-001.01 — Login com credenciais válidas

| Campo | Detalhe |
|-------|---------|
| **Pré-condição** | Usuário cadastrado no sistema |
| **Prioridade** | Alta |
| **Tipo** | Funcional |

### Passos
1. Acessar a página de login
2. Inserir e-mail válido no campo "E-mail"
3. Inserir senha correta no campo "Senha"
4. Clicar no botão "Entrar"

### Resultado esperado
Usuário redirecionado para o dashboard. Mensagem de boas-vindas exibida.

### Resultado obtido
> _Preencher após execução_

### Status
- [ ] Passou ✅
- [ ] Falhou ❌
- [ ] Bloqueado 🚫

---

## CT-001.02 — Login com senha incorreta

| Campo | Detalhe |
|-------|---------|
| **Pré-condição** | Usuário cadastrado no sistema |
| **Prioridade** | Alta |
| **Tipo** | Negativo |

### Passos
1. Acessar a página de login
2. Inserir e-mail válido
3. Inserir senha **incorreta**
4. Clicar em "Entrar"

### Resultado esperado
Mensagem de erro: "E-mail ou senha inválidos". Usuário permanece na tela de login.

### Resultado obtido
> _Preencher após execução_

### Status
- [ ] Passou ✅
- [ ] Falhou ❌
- [ ] Bloqueado 🚫

---

## CT-001.03 — Login com campo e-mail vazio

| Campo | Detalhe |
|-------|---------|
| **Prioridade** | Média |
| **Tipo** | Negativo / Validação |

### Passos
1. Acessar a página de login
2. Deixar o campo "E-mail" em branco
3. Preencher a senha
4. Clicar em "Entrar"

### Resultado esperado
Campo destacado em vermelho. Mensagem: "O campo e-mail é obrigatório."

### Resultado obtido
> _Preencher após execução_

### Status
- [ ] Passou ✅
- [ ] Falhou ❌
- [ ] Bloqueado 🚫
