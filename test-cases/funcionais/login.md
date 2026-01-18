# Casos de Teste - Funcionolidade de Login

## 1. Objetivo
Validar o comportamento de funcionalidade de login do sistema, garantindo que apenas usuários autorizados 
tenham acesso e que menssagens de erro sejam exibidas de forma correta em cenários inválidos.

## 2. Escopo
- Validação de campos obrigatórios
- Autenticação com credenciais válidas
- Mensagens de erro para credenciais inválidas

## 3. Pré-condições
- Usuário cadastrado no sistema
- Sistema disponível e acessível
- Usuário não autenticado

**Dados de teste:**  
- [dados válidos e inválidos](../../test-data/login-data.md)

  ## CT-001 - Login com credenciais válidas
  **Tipo:** Funcional
  **Prioridade:** Alta

  **Passos:**
  1. Acessar a página de login
  2. Informar um email válido
  3. Informar uma senha válida
  4. Clicar no botão **Entrar**
 
  **Resultado esperado:**
  - Usuário autenticado com sucesso
  - Redirecionamento para a página inicial do sistema

    ## CT-002 - Login com senha inválida
    **Tipo:** Funcional
    **Priodidade:** Alta

  **Passos:**
  1. Acessar a página de login
  2. Informar um email válido
  3. Informar uma senha inválida
  4. Clicar no botão **Entrar**

   **Resultado esperado:**
   - Sistema exibe uma mensagem de erro: *Email ou senha inválidos*
   - Usuário permanece na tela de login

  ## CT-003 - Login com email inválido
  **Tipo:** Funcional
  **Prioridade:** Média

  **Passos:**
  1. Acessar a página de login
  2. Informar um email em formato inválido
  3. Informar uma senha válida
  4. Clicar no botão **Entrar**

  **Resultado esperado:**
  - Sistema exibe validação no campo email
  - Login não realizado

  ## CT-004 - Login com campos obrigatórios vazios
  **Tipo:** Válidação
  **Prioridade:** Alta

  **Passos:**
  1. Acessar a página de login
  2. Não preencher email e senha
  3. Clicar no botão **Entrar**

  **Resultado esperado:**
  - Sistema exibe mensagens de campo obrigatótio
  - Nenhuma tentativa de autenticação é realizada

  
