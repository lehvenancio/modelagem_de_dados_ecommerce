# 📦 Projeto de Modelagem de Dados – E-commerce  

## 📝 Descrição do Desafio  
Este projeto consiste no desenvolvimento de um **esquema conceitual e lógico de banco de dados para um sistema de e-commerce**, implementado no **SQL Workbench**.  
O objetivo é criar uma base de dados que permita armazenar e organizar informações relacionadas a clientes, pedidos, pagamentos e entregas, garantindo a consistência e flexibilidade do sistema.  

O esquema deverá ser versionado e disponibilizado em um repositório do **GitHub**, para futura avaliação como parte de um **desafio de projeto**.  

---

## 🎯 Objetivos do Projeto  
Refinar o modelo apresentado acrescentando os seguintes pontos:  

1. **Cliente PJ e PF**  
   - Uma conta pode ser **Pessoa Física (PF)** ou **Pessoa Jurídica (PJ)**, mas não pode ter os dois tipos de informação ao mesmo tempo.  

2. **Pagamento**  
   - Cada cliente pode ter **mais de uma forma de pagamento cadastrada** (ex: cartão de crédito, boleto, PIX).  

3. **Entrega**  
   - As entregas devem conter **status** (ex: em preparação, enviado, entregue) e um **código de rastreio** para acompanhamento.  

---

## 📐 Modelo Conceitual  
O modelo conceitual foi desenvolvido utilizando **Entidade-Relacionamento (EER)** para representar as principais entidades do e-commerce e seus relacionamentos.  

### Principais entidades e atributos:  

- **Cliente**  
  - ID_Cliente  
  - Nome  
  - Email  
  - Telefone  
  - Endereço  
  - Tipo (PF ou PJ)  
  - Documento (CPF ou CNPJ)  

- **Pagamento**  
  - ID_Pagamento  
  - Tipo de Pagamento (Cartão, PIX, Boleto, etc.)  
  - Dados de Pagamento  
  - FK → Cliente  

- **Pedido**  
  - ID_Pedido  
  - Data do Pedido  
  - Valor Total  
  - FK → Cliente  

- **Entrega**  
  - ID_Entrega  
  - Status (Preparando, Enviado, Entregue)  
  - Código de Rastreio  
  - FK → Pedido  

- **Produto**  
  - ID_Produto  
  - Nome  
  - Descrição  
  - Preço  
  - Estoque  

## 🛠️ Ferramentas Utilizadas  
- **SQL Workbench** para a modelagem e implementação do esquema.  
- **MySQL** como SGBD de referência.  
- **Git/GitHub** para versionamento e publicação do projeto.  

---

