# Análise de Best-Sellers em E-Commerce

## Descrição
Este projeto analisa quais características de produtos tornam-os best-sellers em plataformas de e-commerce. Usando dados da Wish, identifico padrões entre produtos que vendem muitas unidades e os que vendem pouco, para orientar decisões de vendedores e afiliados.

## Pergunta Central
Quais características de um produto (preço, rating, badges, anúncios) estão associadas a altas vendas?

## Dataset
**Fonte:** Kaggle - Summer Products Sales Performance  
**Tamanho:** 1.573 produtos  
**Período:** Dados de verão 2020  
**Colunas principais:**
- `units_sold`: unidades vendidas (variável alvo)
- `price`: preço do produto
- `rating`: avaliação média (0-5)
- `badge_fast_shipping`: produto com entrega rápida
- `badge_product_quality`: distintivo de qualidade
- `uses_ad_boosts`: usa anúncios pagos

## Metodologia
1. **Exploração:** análise descritiva dos dados e distribuição de vendas
2. **Definição:** classificação de best-sellers (vendas > 600 unidades)
3. **Análise Comparativa:** comparação de características entre best-sellers e não best-sellers
4. **Visualização:** gráficos mostrando padrões principais

## Principais Descobertas
- **925 produtos (59%)** são classificados como best-sellers (>600 vendas)
- **Distribuição de vendas:** altamente concentrada — maioria vende pouco, poucos explodem em vendas (máximo: 100.000 unidades)
- **Preço:** best-sellers têm preço máximo de R$24, enquanto não best-sellers chegam a R$49. Indica que produtos muito caros dificilmente viram sucesso

## Como Usar
1. Clone o repositório
2. Instale as dependências: `pip install pandas matplotlib jupyter`
3. Abra o notebook: `jupyter notebook notebooks/01_exploracao.ipynb`
4. Execute as células na sequência

## Estrutura do Projeto
portfolio-dados/
├── README.md
├── dados/
│ └── summer-products-...csv
├── notebooks/
│ ├── 01_exploracao.ipynb
│ ├── 02_limpeza.ipynb
│ └── 03_analise_final.ipynb
└── graficos/

## Tecnologias
- Python 3.14
- Pandas (manipulação de dados)
- Matplotlib (visualização)
- Jupyter Notebook (análise interativa)

## Próximos Passos
- Explorar impacto de rating e badges nas vendas
- Criar modelo preditivo de vendas
- Analisar diferenças por categoria de produto