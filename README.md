# 📊 CEAPS Storytelling — Visualização e Análise dos Gastos do Senado Federal

Projeto de análise exploratória e storytelling com dados das despesas de senadores brasileiros (CEAPS — Cota para o Exercício da Atividade Parlamentar dos Senadores), cobrindo o período de **2019 a 2022**.

> **Parte do desafio [#7DaysOfCode](https://7daysofcode.io/) de Data Science — Dia 2/7**

---

## 📋 Sobre o Projeto

Utilizando o dataset limpo gerado no [Dia 1 (Data Wrangling)](https://github.com/Bernardinense/ceaps-data-wrangling), este projeto transforma **69.356 registros** de despesas parlamentares em uma narrativa visual orientada por **5 perguntas-chave**, respondidas com análises estatísticas, gráficos interativos e conclusões fundamentadas.

### Perguntas investigadas

1. **Os gastos estão aumentando ao longo dos anos?** — Impacto da pandemia (2020) e do ano eleitoral (2022)
2. **Com o que os senadores mais gastam?** — Categorias que mais consomem recursos públicos
3. **Quais os 10 senadores que mais gastaram?** — Maiores utilizadores da cota parlamentar
4. **Quais fornecedores mais receberam dinheiro público?** — Empresas que mais se beneficiaram
5. **Existe algum padrão de gasto por mês?** — Sazonalidade e tendências mensais

### Principais descobertas

| Descoberta | Detalhe |
|------------|---------|
| Impacto da pandemia | Queda significativa em 2020, com retomada crescente em 2021–2022 |
| Maior categoria de gasto | Consultorias e assessorias, seguido por viagens, hospedagem e alimentação |
| Top 3 senadores | Telmário Mota, Rogério Carvalho e Mecias de Jesus |
| Top 3 fornecedores | Adria Viagens e Turismo, LATAM e Gol |
| Sazonalidade | Pico de gastos recorrente em dezembro; 2022 com aumento expressivo em todos os meses |

### Visualizações geradas

- 📈 Evolução anual dos gastos (linha)
- 📊 Distribuição por categoria de despesa (barras + pizza)
- 🏆 Top 10 senadores que mais gastaram (barras horizontais)
- 🏢 Top 10 fornecedores que mais receberam (barras horizontais)
- 📅 Padrão mensal de gastos (barras)
- 🗓️ Heatmap de gastos por mês e ano

### Exportações

- **7 gráficos interativos** em HTML (Plotly)
- **6 planilhas Excel** com dados por pergunta
- **1 relatório consolidado** em Excel com múltiplas abas

---

## 🛠️ Tecnologias Utilizadas

- **Python 3.13**
- **Pandas** — Manipulação e agregação de dados
- **NumPy** — Operações numéricas
- **Plotly Express** — Gráficos interativos (linha, barras, pizza)
- **Plotly Graph Objects** — Heatmap e customizações avançadas
- **openpyxl** — Exportação para Excel

---

## 📁 Estrutura do Projeto

```
ceaps-storytelling/
├── storytelling_ceaps.ipynb   # Notebook com análise completa e storytelling
├── README.md                   # Este arquivo
├── requirements.txt            # Dependências do projeto
└── .gitignore                  # Arquivos ignorados pelo Git
```

> Os gráficos HTML, planilhas Excel e o relatório consolidado são gerados automaticamente ao executar o notebook.

---

## 🚀 Como Executar

### 1. Clone o repositório
```bash
git clone https://github.com/Bernardinense/ceaps-storytelling.git
cd ceaps-storytelling
```

### 2. Instale as dependências
```bash
pip install -r requirements.txt
```

### 3. Obtenha o dataset limpo

Este projeto depende do dataset tratado no Dia 1:

1. Baixe os dados originais no [Portal de Dados Abertos do Senado Federal — CEAPS](https://www12.senado.leg.br/transparencia/dados-abertos-transparencia/dados-abertos-ceaps) (anos 2019 a 2022, *caso não o tenha feito ainda*)
2. Execute o pipeline de limpeza do [ceaps-data-wrangling](https://github.com/Bernardinense/ceaps-data-wrangling) para gerar o arquivo `ceaps_4anos_limpo.csv`
3. Coloque o arquivo na raiz do projeto:

```
ceaps-storytelling/
├── ceaps_4anos_limpo.csv   ← aqui
├── storytelling_ceaps.ipynb
└── ...
```

### 4. Execute o notebook
```bash
jupyter notebook storytelling_ceaps.ipynb
```

---

## 🔗 Parte do Desafio #7DaysOfCode

Este projeto é o **Dia 2** de um desafio de 7 dias cobrindo o pipeline completo de Data Science:

| Dia | Projeto | Tema |
|-----|---------|------|
| 1 | [ceaps-data-wrangling](https://github.com/Bernardinense/ceaps-data-wrangling) | Limpeza e Tratamento de Dados |
| **2** | **ceaps-storytelling** | **Visualização e Storytelling** |
| 3 | ceaps-forecasting  | Previsão com Prophet |
| 4 | movie-recommendation-system | Sistema de Recomendação |
| 5 | movie-recommendation-api | API REST com FastAPI |
| 6 | ab-testing-hypothesis | Teste A/B e Validação de Hipóteses |

📌 Veja a jornada completa: [7DaysOfCode-DataScience](https://github.com/Bernardinense/7DaysOfCode-DataScience)

---

## 👤 Autor

**Bruno Corrêa** —  Engenheiro | Especialista em Ciência de Dados

[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/bfpc7/)
[![GitHub](https://img.shields.io/badge/GitHub-black?style=flat&logo=github)](https://github.com/Bernardinense)

---

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.