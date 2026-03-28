
Dashboard Comercial Global (2022–2024)
🧾 Descrição do Projeto

Este projeto consiste na criação de um Dashboard Comercial interativo no Power BI, desenvolvido para analisar o desempenho de vendas de uma empresa internacional que comercializa produtos em diferentes regiões do mundo.

O dashboard consolida dados dos anos 2022, 2023 e 2024, permitindo análises estratégicas sobre faturamento, volume de vendas, perfil dos clientes, canais de venda e devoluções, com foco em apoiar a tomada de decisão do negócio.

🎯 Objetivo

O principal objetivo do projeto é:

Transformar dados brutos de vendas em informações visuais claras
Identificar padrões e tendências ao longo do tempo
Avaliar o desempenho por marca, continente, gênero e canal de venda
Demonstrar habilidades práticas em Power BI e DAX
🗂️ Fonte e Estrutura dos Dados

Os dados representam informações comerciais fictícias de uma loja internacional e incluem:

Base de Vendas
Faturamento por venda
Quantidade vendida
Quantidade devolvida
Identificação do cliente
Gênero do cliente
Marca do produto
Data da venda
Cadastro de Lojas
Tipo de loja (Online ou Física)
Dimensões
Ano e mês
Continente

📌 KPIs Principais do Dashboard
💰 Receita Total
📦 Produtos Vendidos
👥 Quantidade de Clientes
💳 Ticket Médio
🌐 Participação das Vendas Online
🔄 Percentual de Devoluções
🧮 Medidas DAX Utilizadas
🔹 Faturamento Total
fat total = SUM('Base vendas'[Faturamento na venda])

➡️ Soma total do faturamento gerado pelas vendas.

🔹 Total de Vendas
Total Vendas = SUM('Base vendas'[Qtd. Vendida])

➡️ Quantidade total de produtos vendidos.

🔹 Quantidade de Clientes
qtd clientes = DISTINCTCOUNT('Base vendas'[Id Cliente])

➡️ Número de clientes únicos que realizaram compras.

🔹 Ticket Médio
ticket medio = AVERAGE('Base vendas'[Faturamento na venda])

➡️ Valor médio gasto por venda.

🔹 Total de Devoluções
Total devoluções = SUM('Base vendas'[Qtd. Devolvida])

➡️ Quantidade total de itens devolvidos.

🔹 Percentual de Devoluções
% devoluções = [Total devoluções] / [Total Vendas]

➡️ Percentual de produtos devolvidos em relação ao total vendido.

🔹 Vendas Online
Vendas online =
CALCULATE(
    SUM('Base vendas'[Qtd. Vendida]),
    'cadastro de lojas'[Tipo Loja] = "online"
)

➡️ Quantidade de produtos vendidos pelo canal online.

🔹 Percentual de Vendas Online
% vendas online = [Vendas online] / [Total Vendas]

➡️ Participação do canal online nas vendas totais.

📊 Visualizações do Dashboard

O dashboard contém as seguintes análises:

📅 Evolução do faturamento por Ano e Mês
🌍 Faturamento por Continente (mapa geográfico)
🏷️ Faturamento por Marca
👤 Distribuição das vendas por Gênero
📈 Indicadores consolidados (KPIs)
🔍 Principais Análises Possíveis
Identificar quais continentes geram maior receita
Avaliar crescimento ou queda de faturamento ao longo do tempo
Analisar a importância do canal online
Verificar marcas mais lucrativas
Monitorar a taxa de devoluções
Entender o perfil dos clientes por gênero
🛠️ Ferramentas Utilizadas
Power BI Desktop
DAX (Data Analysis Expressions)
Excel / CSV (base de dados)
GitHub (versionamento e portfólio)
📷 Preview do Dashboard

O print do dashboard está disponível neste repositório para visualização rápida do projeto.


👨‍💻 Autor

Projeto desenvolvido por Philipe L., estudante de Ciência da Computação, com foco em Análise de Dados, Power BI, SQL e Python.

📌 Este projeto faz parte do meu portfólio profissional para vagas de Analista de Dados Júnior.
