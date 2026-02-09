# 🛒 Store Manager

Desafio técnico: Sistema de gerenciamento de loja via terminal (CLI) com persistência em JSON e exportação para Excel.

## 📋 Requisitos do Projeto

### 🚀 Etapa 1: Estrutura de Dados
O sistema garante que os dados não sejam perdidos ao fechar.
- [ ] **Verificação Inicial:** Ao iniciar, verifica se `dados_loja.json` existe.
- [ ] **Criação Automática:** Se não existir, cria: `{"produtos": [], "caixa": 0.0}`.
- [ ] **Salvamento:** O JSON é atualizado após cada venda ou cadastro.

### 📦 Etapa 2: Gestão de Estoque (CRUD)
Funcionalidades do menu "Gerenciar Estoque":
- [ ] **Cadastrar:** Nome, Custo, Venda e Quantidade.
- [ ] **Validação:** Impede nomes duplicados e valores negativos.
- [ ] **Listar:** Mostra tabela (ID, Nome, Qtd, Preço).
- [ ] **Remover:** Deleta produto pelo nome.

### 💰 Etapa 3: Vendas (Core)
Lógica da opção "Nova Venda":
- [ ] **Busca:** Procura pelo nome do produto.
- [ ] **Verificação:**
  - *Com Estoque:* Subtrai quantidade e soma valor ao caixa.
  - *Sem Estoque:* Exibe erro.
- [ ] **Recibo:** Mostra o total da venda na tela.

### 📊 Etapa 4: Relatórios (Excel)
Opção "Fechar Caixa e Exportar" (usa `openpyxl`):
1. **Aba Estoque:** Lista produtos e total investido.
2. **Aba Resumo:** Mostra o saldo final do caixa.

---
*Desenvolvido em Python.*
