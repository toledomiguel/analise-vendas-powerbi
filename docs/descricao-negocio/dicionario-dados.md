# Dicionário de Dados

## Objetivo
Documentar as principais tabelas que serão utilizadas no projeto de BI para análise de vendas em e-commerce.

## Tabelas previstas

### 1. orders
Tabela com informações gerais dos pedidos realizados no e-commerce.

**Principais campos esperados:**
- order_id
- customer_id
- order_status
- order_purchase_timestamp
- order_delivered_customer_date
- order_estimated_delivery_date

**Finalidade na análise:**
- acompanhar volume de pedidos
- analisar datas de compra e entrega
- medir atrasos
- calcular indicadores de tempo

---

### 2. customers
Tabela com informações dos clientes.

**Principais campos esperados:**
- customer_id
- customer_unique_id
- customer_city
- customer_state

**Finalidade na análise:**
- analisar distribuição geográfica dos clientes
- identificar regiões com maior volume de pedidos
- apoiar análise por estado e cidade

---

### 3. order_items
Tabela com os itens de cada pedido.

**Principais campos esperados:**
- order_id
- product_id
- seller_id
- shipping_limit_date
- price
- freight_value

**Finalidade na análise:**
- calcular faturamento
- analisar produtos vendidos
- medir valor de frete
- identificar volume por item

---

### 4. products
Tabela com informações dos produtos.

**Principais campos esperados:**
- product_id
- product_category_name
- product_name_lenght
- product_description_lenght
- product_photos_qty
- product_weight_g

**Finalidade na análise:**
- analisar categorias de produtos
- identificar produtos mais relevantes
- relacionar características do produto com performance de vendas

---

### 5. payments
Tabela com informações de pagamento dos pedidos.

**Principais campos esperados:**
- order_id
- payment_sequential
- payment_type
- payment_installments
- payment_value

**Finalidade na análise:**
- analisar formas de pagamento
- acompanhar valor pago
- entender comportamento de parcelamento

---

### 6. reviews
Tabela com avaliações dos clientes.

**Principais campos esperados:**
- review_id
- order_id
- review_score
- review_creation_date
- review_answer_timestamp

**Finalidade na análise:**
- medir satisfação do cliente
- calcular nota média
- analisar relação entre atraso e avaliação

---

### 7. sellers
Tabela com informações dos vendedores.

**Principais campos esperados:**
- seller_id
- seller_city
- seller_state

**Finalidade na análise:**
- analisar distribuição dos vendedores
- relacionar localização do vendedor com entregas e vendas

---

### 8. geolocation
Tabela com dados geográficos.

**Principais campos esperados:**
- geolocation_zip_code_prefix
- geolocation_lat
- geolocation_lng
- geolocation_city
- geolocation_state

**Finalidade na análise:**
- enriquecer análises geográficas
- apoiar visualizações por localização