# ETL e Dashboard de Análise COVID-19

Este projeto apresenta um processo de ETL (Extract, Transform, Load) realizado com os dados da pandemia de COVID-19, seguido de uma análise visual desenvolvida no Power BI. O objetivo é transformar os dados brutos em informações acionáveis por meio de métricas e visualizações.

![Menu Inicial](https://github.com/user-attachments/assets/2d1faba3-7d7e-4262-9a12-249be4f19b0b)


## 🎯 Objetivo do Projeto
Criar um dashboard informativo que permita acompanhar os principais indicadores relacionados à pandemia de COVID-19, como número de casos, óbitos e taxas de recuperação, extraindo insights estratégicos para tomada de decisão.

---

## 📂 Fonte de Dados
- **Arquivo Utilizado**: `Covid.xlsx`
- **Conteúdo**:
  - Dados brutos sobre a pandemia: número de casos confirmados, óbitos, recuperados e outras informações relevantes.
  - Os dados foram coletados de fontes públicas e consolidados no arquivo Excel fornecido.

---

## ⚙️ Processo ETL
O fluxo de ETL foi realizado no Power BI e seguiu as seguintes etapas:

1. **Extração**:
   - Carregamento do arquivo `Covid.xlsx` no Power BI.

2. **Transformação**:
   - **Limpeza de Dados**: Remoção de linhas duplicadas e tratamento de valores ausentes.
   - **Conversão de Tipos**: Ajuste de colunas como datas e valores numéricos.
   - **Criação de Colunas Calculadas**:
     - Taxa de Mortalidade: `(Óbitos / Casos Confirmados) * 100`
     - Taxa de Recuperação: `(Recuperados / Casos Confirmados) * 100`

3. **Carga**:
   - Dados transformados foram carregados no modelo do Power BI para análise.

---

## 📊 Dashboard
O dashboard foi desenvolvido no Power BI com foco na apresentação clara e objetiva das informações mais relevantes. Abaixo estão os principais elementos e métricas:

### 🧮 Principais Métricas
- **Casos Confirmados**: Total de casos registrados.
- **Óbitos**: Total de mortes registradas.
- **Recuperados**: Total de pessoas recuperadas.
- **Taxa de Mortalidade**: Proporção de óbitos em relação aos casos confirmados.
- **Taxa de Recuperação**: Proporção de recuperados em relação aos casos confirmados.

### ⚡ Medidas DAX Utilizadas
- **Taxa de Mortalidade**:
  ```DAX
  Taxa de Mortalidade = DIVIDE(SUM(Óbitos), SUM(Casos Confirmados)) * 100
  ```
- **Taxa de Recuperação**:
  ```DAX
  Taxa de Recuperação = DIVIDE(SUM(Recuperados), SUM(Casos Confirmados)) * 100
  ```

### 📈 Visualizações
- **Gráficos de Linhas**: Evolução de casos confirmados e óbitos ao longo do tempo.
- **Cartões Resumo**: Exibição de métricas principais.
- **Mapa Interativo**: Distribuição geográfica dos casos.
- **Tabela Dinâmica**: Detalhamento por região e data.

---

![Casos no Mundo](https://github.com/user-attachments/assets/de682300-ab22-4750-a930-77e277b4462c)

![Casos no Brasil](https://github.com/user-attachments/assets/9c427548-faed-4d29-95d7-0b38dfad047e)



## 📌 Conclusão
Este projeto demonstrou como transformar dados brutos em insights valiosos por meio de um processo de ETL eficiente e visualizações intuitivas. O dashboard serve como uma ferramenta poderosa para monitorar e analisar os impactos da COVID-19 de forma prática.


## 🛠️ Tecnologias Utilizadas
- **Power BI**: Para o processo ETL e criação do dashboard.
- **Excel**: Como fonte de dados inicial.

## 🚀 Como Utilizar
1. Baixe os arquivos deste repositório.
2. Abra o arquivo `ETL Covid.pbix` no Power BI.
3. Explore as visualizações e os dados transformados.

---

**Autor:** Lício Martins  

**Contato:** [liciomlima@gmail.com]

**Linkedln:** [https://www.linkedin.com/in/liciolima/]
