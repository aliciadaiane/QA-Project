# Casos de teste - Funcionalidade de Cadastro


## 1. Descrição

Implementar a funcionalidade de cadastro de usuário com campos para entrada de nome, data de nascimento, email e senha. Os usuários preencherão essas informações e, em seguida, serão registrados no sistema. A validação será realizada para garantir que os campos sejam preenchidos corretamente.

Para o cadastro de novo usuário, ele não pode ter um email já cadastrado no sistema. 
A senha precisa ter 8 ou mais dígitos.

**Dados de teste:**
- [dados válidos e inválidos](../../test-data/login-data.md)

## CT-001 - Cadastro com dados válidos
**Prioridade:** Alta

**Objetivo do teste**
Verificar se o sistema permite o cadastro de novo usuário quando todos os campos obrigatórios são preenchidos corretamente.

**Pré-condições:**
- Usuário não cadastrado no sistema
- Email informado não cadastrado

**Passos:**
1. Acessar página de cadastro
2. Preencher o campo de Nome
3. Informar data de nascimento válida
4. Informar Email válido
5. Informar senha com 8 ou mais caracteres

**Reesultados esperados:**
- Usuário cadastrado com sucesso 
- Sistema exibe mensagem de cadastro realizado com sucesso

## CT-002 - Cadastro com email já existente

