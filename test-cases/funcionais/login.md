# Casos de Teste - Funcionolidade de Login

## 1. Descrição
Implementar a funcionalidade de login de usuário com campos para entrada de 
email e senha. Os usuários preencherão essas informações e, em seguida, serão redirecionados para 
a página inicial. A validação será realizada para garantir que os campos sejam preenchidos corretamente.

Para o login de usuário, ele precisa ter um email já cadastrado no sistema.
É preciso ter uma senha válida com 8 ou mais dígitos.

**Dados de teste:**  
- [dados válidos e inválidos](../../test-data/login-data.md)

  ## CT-001 - Login com credenciais válidas
  **Prioridade:** Alta

  **Pré-condições:**
- Usuário cadastrado no sistema
- Email e senha válidos
- Usuário não autenticado
- Conta ativa

  **Passos:**
  1. Acessar a página de login
  2. Informar um email válido
  3. Informar uma senha válida
  4. Clicar no botão **Entrar**
 
  **Resultado esperado:**
  - Usuário autenticado com sucesso
  - Redirecionamento para a página inicial do sistema

    ## CT-002 - Login com senha inválida
    **Priodidade:** Alta

    **Pré-condições:**
  - Usuário cadastrado no sistema
  - Senha inválida
  - Usuário não autenticado
  - Conta ativa

  **Passos:**
  1. Acessar a página de login
  2. Informar um email válido
  3. Informar uma senha inválida
  4. Clicar no botão **Entrar**

   **Resultado esperado:**
   - Sistema exibe uma mensagem de erro: *Email ou senha inválidos*
   - Usuário permanece na tela de login

  ## CT-003 - Login com email inválido
  **Prioridade:** Média

  **Pré-condições:**
- Usuário cadastrado no sistema
- Email inválido
- Usuário não autenticado
- Conta ativa

  **Passos:**
  1. Acessar a página de login
  2. Informar um email em formato inválido
  3. Informar uma senha válida
  4. Clicar no botão **Entrar**

  **Resultado esperado:**
  - Sistema exibe validação no campo email
  - Login não realizado

  ## CT-004 - Login com campos obrigatórios vazios
  **Prioridade:** Alta

  **Pré-condições:**
- Usuário cadastrado no sistema
- campos de email e senha vazios
- Usuário não autenticado
- Conta ativa

  **Passos:**
  1. Acessar a página de login
  2. Não preencher email e senha
  3. Clicar no botão **Entrar**

  **Resultado esperado:**
  - Sistema exibe mensagens de campo obrigatótio
  - Nenhuma tentativa de autenticação é realizada

  
