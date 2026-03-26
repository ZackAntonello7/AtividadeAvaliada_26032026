# 🏥 Sistema Integrado de Gestão de Farmácia “Saúde & Vida”

## 📌 Descrição do Projeto
Este projeto tem como objetivo desenvolver um sistema integrado para gestão de farmácias da rede **Saúde & Vida**, permitindo o controle eficiente das operações administrativas e comerciais.

O sistema visa substituir processos manuais por uma solução digital, integrando setores como vendas, estoque e financeiro.

---

## 🎯 Objetivo do Sistema
O sistema deve:

- Aumentar a eficiência do atendimento  
- Garantir integridade no controle de estoque  
- Reduzir erros manuais  
- Integrar vendas, compras e financeiro  
- Fornecer dados confiáveis para tomada de decisão  

---

## 👥 Usuários do Sistema

O sistema será utilizado por diferentes perfis:

- **Atendentes**: realizam vendas e cadastro de clientes  
- **Farmacêuticos**: validam receitas e autorizam vendas controladas  
- **Gerentes**: gerenciam produtos, estoque e preços  
- **Administradores**: controlam usuários e permissões  

---

## 🧩 Funcionalidades do Sistema

### 🛒 1. Vendas e Atendimento
- Registro de vendas de medicamentos e produtos  
- Busca de produtos por nome, código ou código de barras  
- Verificação de receita médica quando necessário  
- Cadastro rápido de clientes  
- Controle de vendas a prazo  
- Emissão de comprovante de venda  

---

### 📦 2. Gestão de Estoque
- Controle de quantidade de produtos  
- Atualização automática após:
  - vendas  
  - devoluções  
  - perdas  
  - transferências  
- Alerta de estoque mínimo  
- Cadastro e atualização de produtos  

---

### 🚚 3. Compras e Fornecedores
- Registro de compras de produtos  
- Associação com fornecedores  
- Atualização automática do estoque  
- Integração com contas a pagar  

---

### 💰 4. Financeiro

#### Contas a Receber
- Geradas por vendas a prazo ou convênios  
- Controle de vencimentos  
- Status:
  - Aberta  
  - Recebida  
  - Atrasada  

#### Contas a Pagar
- Pagamentos a fornecedores e despesas  
- Controle de vencimento e pagamento  
- Status:
  - Aberta  
  - Paga  
  - Atrasada  

---

### 📊 5. Relatórios
O sistema deve gerar relatórios como:

- Produtos mais vendidos  
- Situação do estoque  
- Vendas por período  
- Compras por fornecedor  
- Contas a pagar e receber  
- Produtos sem venda  

---

### 🔐 6. Controle de Acesso
O sistema deve possuir controle de permissões baseado no tipo de usuário.

---

### 🔗 7. Integração de Processos
O sistema deve integrar automaticamente:

- Vendas → Estoque → Financeiro  
- Compras → Estoque → Contas a pagar  
- Vendas a prazo → Contas a receber  

---

## 🧠 Regras de Negócio

- Produtos sem estoque não podem ser vendidos  
- Toda venda deve gerar um comprovante  
- Vendas a prazo geram contas a receber  
- Compras atualizam automaticamente o estoque  
- Sistema deve alertar estoque mínimo  
- Apenas farmacêuticos podem validar receitas  

---

## 🛠️ Tecnologias
Projeto focado em modelagem e documentação de sistema.

---

## 🚀 Execução
Este projeto tem caráter acadêmico e não possui execução prática, sendo voltado à documentação e modelagem de sistema.

---
