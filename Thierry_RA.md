# 📄 Sistema Integrado de Gestão de Farmácia “Saúde & Vida”

## 👤 Aluno
Nome:Thierry Antonello Pengo
RA:24000073

---

## 📌 1. Regras de Negócio

- Produtos sem estoque não podem ser vendidos  
- Toda venda deve gerar um comprovante  
- Vendas a prazo devem gerar contas a receber  
- Compras devem atualizar automaticamente o estoque  
- O sistema deve alertar produtos com estoque mínimo  
- Apenas farmacêuticos podem validar receitas  

---

## ⚙️ 2. Requisitos Funcionais

- RF01: O sistema deve permitir cadastrar clientes  
- RF02: O sistema deve registrar vendas  
- RF03: O sistema deve consultar produtos por nome ou código  
- RF04: O sistema deve controlar o estoque  
- RF05: O sistema deve registrar compras  
- RF06: O sistema deve gerar contas a pagar  
- RF07: O sistema deve gerar contas a receber  
- RF08: O sistema deve emitir relatórios  
- RF09: O sistema deve permitir cadastro de produtos  

---

## 🔒 3. Requisitos Não Funcionais

- RNF01: O sistema deve ser acessível via navegador  
- RNF02: O sistema deve possuir autenticação de usuários  
- RNF03: O sistema deve responder em até 2 segundos  
- RNF04: O sistema deve garantir segurança dos dados  

---

## 🎭 4. Casos de Uso

- Realizar venda  
- Cadastrar cliente  
- Consultar produto  
- Registrar compra  
- Atualizar estoque  
- Gerar relatório  
- Registrar conta a pagar  
- Registrar conta a receber  
- Validar receita  
- Gerenciar usuários  

### Relações

**Include:**
- Realizar venda → inclui → Consultar produto  
- Realizar venda → inclui → Verificar estoque  

**Extend:**
- Realizar venda → estende → Validar receita  
- Realizar venda → estende → Venda a prazo  

---

## 📊 5. Diagrama de Casos de Uso

### Atores:
- Atendente  
- Farmacêutico  
- Gerente  
- Administrador  

### Casos:
- Atendente: Realizar venda, consultar produto, cadastrar cliente  
- Farmacêutico: Validar receita  
- Gerente: Gerenciar estoque, cadastrar produtos, registrar compras  
- Administrador: Gerenciar usuários  

---

## 🧱 6. Diagrama de Classes

### Classes:

- Cliente (id, nome, cpf)  
- Produto (id, nome, preço, estoque)  
- Venda (id, data, valorTotal)  
- ItemVenda (quantidade, subtotal)  
- Fornecedor (id, nome)  
- Compra (id, data, valor)  
- ContaPagar (id, valor, status)  
- ContaReceber (id, valor, status)  

### Relacionamentos:

- Cliente realiza Venda  
- Venda possui ItemVenda  
- ItemVenda referencia Produto  
- Compra está ligada ao Fornecedor  
- Compra gera ContaPagar  
- Venda gera ContaReceber  

---

## 🔄 7. Diagrama de Atividade

Fluxo de Venda:

Início  
→ Atendente inicia venda  
→ Consultar produto  
→ Verificar estoque  

Produto disponível?  

Se NÃO:  
→ Informar indisponibilidade  
→ Fim  

Se SIM:  
→ Adicionar produto  

Cliente possui receita?  

Se SIM:  
→ Validar receita  

Cliente deseja pagar a prazo?  

Se SIM:  
→ Gerar conta a receber  

→ Finalizar venda  
→ Gerar comprovante  
→ Fim  

---
- Cliente realiza Venda  
- Venda possui ItemVenda  
- ItemVenda referencia Produto  
- Compra está ligada a Fornecedor  
- Compra gera ContaPagar  
- Venda gera ContaReceber  
