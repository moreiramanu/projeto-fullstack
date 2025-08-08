# 🛍️ Projeto E-commerce - Maquiagem

**Atividade Avaliativa da UC - Projeto e-commerce**  
**Desenvolvido por: Emanuely e Thaís**

---

## 🎯 Escopo do Projeto

### Objetivo
Desenvolver uma plataforma de e-commerce para venda de maquiagens, permitindo que clientes:
- Naveguem por categorias de produtos
- Visualizem detalhes
- Adicionem ao carrinho
- Realizem compras com segurança

### Funcionalidades principais
- Cadastro e login de clientes
- Catálogo de produtos por categoria
- Sistema de carrinho
- Integração com formas de pagamento (Pix e cartão)
- Painel administrativo para gestão de produtos e pedidos

---

## 📋 Requisitos

### Requisitos Funcionais
- O sistema deve permitir o cadastro de clientes.
- O sistema deve permitir o login por email e senha.
- O cliente deve poder navegar por categorias (batons, bases, sombras, etc.).
- O cliente pode adicionar produtos ao carrinho.
- O cliente pode finalizar a compra e escolher o método de pagamento.
- O administrador pode adicionar, editar ou excluir produtos.
- O administrador pode visualizar todos os pedidos feitos.

### Requisitos Não Funcionais
- A interface deve ser responsiva.
- O sistema deve funcionar em diferentes dispositivos e navegadores.
- O sistema deve estar disponível 24h por dia, 7 dias por semana, com taxa de disponibilidade de 98%.
- O sistema deve seguir a LGPD no uso de dados pessoais.
- O sistema deve ser capaz de lidar com falhas sem afetar a experiência do usuário.

---

## 🎨 Paleta de Cores

🔗 [Ver paleta aqui](https://paletadecores.com/paleta/ffb6c8/ffc8d6/ffdae4/ffedf1/ffffff/)

- **Rosa claro**: suavidade e acolhimento
- **Rosa escuro**: intensidade e estilo (ideal para botões e destaques)
- **Branco**: equilíbrio e limpeza visual
- **Preto**: contraste e legibilidade

---

## 🧩 Wireframes

- Página Inicial  
- Página de Login/Cadastro  
- Página de Detalhes do Produto  
- Carrinho de Compras  

---

## 🗃️ Esquema do Banco de Dados

### Tabelas principais:

#### 🧑‍💼 Usuário (Cliente)
- `usuario_id` (PK)  
- `nome`  
- `email`  
- `senha`  
- `cliente`  

#### 🛍️ Produto
- `produto_id` (PK)  
- `nome`  
- `descricao`  
- `preco`  
- `estoque`  
- `categoria_id` (FK)  
- `imagem_url`  

#### 🗂️ Categoria
- `categoria_id` (PK)  
- `nome`  

#### 🧾 Pedido
- `pedido_id` (PK)  
- `usuario_id` (FK)  
- `data_pedido`  
- `valor_total`  

#### 🧮 Item_Pedido (Tabela Associativa)
- `item_pedido_id` (PK)  
- `pedido_id` (FK)  
- `produto_id` (FK)  
- `quantidade`  
- `preco_unitario`  

---

## 🗓️ Cronograma

| Dia da Semana | Atividades |
|---------------|------------|
| **Sexta-feira (1º dia)** | Levantamento de requisitos, escopo, wireframes, mapa do site, modelo inicial do banco de dados |
| **Segunda-feira** | Modelagem completa do banco de dados e estrutura inicial do projeto (HTML/CSS) |
| **Terça-feira** | Criação das tabelas no SQL, inserção de dados, frontend da página inicial |
| **Quarta-feira** | Ajustes no banco, criação de queries, frontend da página de login e cadastro funcional |
| **Quinta-feira** | Integração com o backend, página de detalhes do produto, carrinho e revisões |
| **Sexta-feira (final)** | Apresentação do projeto |

---

## 🌐 Mapa do Site

- **Página Inicial**: exibe produtos, banners e acesso às demais páginas.  
- **Página de Login/Cadastro**: login ou criação de conta.  
- **Página de Detalhes do Produto**: nome, descrição, imagem, preço e botão para adicionar ao carrinho.  
- **Carrinho de Compras**: produtos adicionados, ajuste de quantidades e finalização da compra.

---
