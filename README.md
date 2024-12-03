# Projeto Conceitual de Banco de Dados E-COMMERCE

## 🔑 Entidades Principais

O diagrama de relacionamento abrange as seguintes entidades:

- **Cliente:** Representa os clientes, com tipos Pessoa Física (PF) ou Pessoa Jurídica (PJ).

**Pedido:** Registra os pedidos realizados pelos clientes.

**Fornecedor:** Gerencia os fornecedores dos produtos.

**Produto:** Contém os produtos disponíveis para venda.

**Estoque:** Gerencia a quantidade de produtos em estoque.

**Vendedor:** Representa os vendedores terceirizados que realizam as vendas.

**Pagamento:** Define as formas de pagamento associadas aos pedidos.

**Entrega:** Controla o status e o código de rastreio das entregas de pedidos.<br><br>

## 🔄 Relacionamentos no Banco de Dados

O modelo de dados define vários relacionamentos, incluindo: <br>

**Relacionamentos N:M (Muitos para Muitos):**

**Vendedor e Produto:** Um vendedor pode vender vários produtos e um produto pode ser vendido por vários vendedores.

**Fornecedor e Produto:** Um fornecedor pode fornecer vários produtos e um produto pode ser fornecido por vários fornecedores.

**Produto e Estoque:** Um produto pode estar presente em vários estoques e um estoque pode conter vários produtos. <br>

**Relacionamentos 1:N (Um para Muitos):**

**Cliente e Pedido:** Um cliente pode realizar vários pedidos.

**Pedido e Pagamento:** Um pedido pode ter múltiplos pagamentos (ex: parcelado).

**Pedido e Entrega:** Um pedido pode ter múltiplas entregas (ex: entregas parciais).<br><br>

## 📊 Estrutura do Banco de Dados

Cada tabela no banco de dados foi projetada para representar uma entidade, com os seguintes detalhes:

**Chaves Primárias (PK) e Chaves Estrangeiras (FK)** para garantir a integridade referencial.

Tabelas de junção para os relacionamentos muitos-para-muitos, como **Fornecedor_Produto, Vendedor_Produto e Produto_Estoque**.

**Tabelas Criadas:**

*Cliente:* Dados do cliente (PF ou PJ).

*Pedido:* Informações sobre o pedido e seu status.

*Fornecedor:* Informações do fornecedor.

*Produto:* Dados do produto.

*Estoque:* Informações sobre a quantidade de produtos disponíveis.

*Vendedor:* Informações do vendedor.

*Pagamento:* Formas de pagamento associadas ao pedido.

*Entrega:* Status e rastreio de entrega.<br><br><br>

## 📈 Diagrama de Entidade-Relacionamento (ER)

O diagrama ER foi criado no **MySQL Workbench** e visualiza todos os relacionamentos e a estrutura do banco de dados.<br><br>

## ⚙️ Tecnologias Utilizadas

**MySQL:** Para o banco de dados relacional.

**MySQL Workbench:** Para modelagem de banco de dados e criação do diagrama ER.<br><br>

## 📥 Como Usar
1- **Clonar o repositório:**
git clone https://github.com/usuario/repositorio.git

2- **Importar o Diagrama no MySQL Workbench:** Abra o arquivo do diagrama ER (.mwb) no MySQL Workbench para visualizar e editar a estrutura do banco de dados.

3- **Criar o Banco de Dados:** Após importar o diagrama, você pode executar as instruções SQL no MySQL Workbench para criar as tabelas no seu banco de dados local.

