# Seasonal Rainfall Data Cleaning

Este repositório apresenta um **exercício completo de limpeza e preparação de dados** utilizando Python e Pandas, aplicado a um conjunto de dados de **chuvas sazonais médias** nas regiões do **Lake Victoria** e **Simiyu (Tanzânia)**.

O foco do projeto é demonstrar boas práticas de **data cleaning**, **organização semântica**, **tipagem correta** e **preparação para análise exploratória (EDA)**.

---

## 📂 Estrutura do Repositório

```text
├── data/
│   ├── raw/
│   │   └── messy-data.xlsx
│   └── processed/
│       └── seasonal_rainfall_clean.csv
│
├── notebooks/
│   └── Messy_Data_for_Data_Cleaning_Exercise.ipynb
│
├── README.md
```

### 📁 `data/raw/`

Contém o **dataset original**, exatamente como fornecido, incluindo:

* cabeçalhos desalinhados
* colunas desnecessárias (`Unnamed`)
* mistura de tipos (strings + números)
* unidades embutidas nos valores (`mm`)

### 📁 `data/processed/`

Contém o **dataset limpo e padronizado**, pronto para:

* análise exploratória
* visualização
* modelagem simples

### 📁 `notebooks/`

Notebook com todo o **processo passo a passo**, incluindo:

* inspeção inicial
* limpeza
* transformação
* validação final

---

## 🧪 Descrição do Dataset

### Dataset original (`messy-data.xlsx`)

Dados de **chuva média mensal** no período **2001–2019**, com problemas típicos de dados reais:

* cabeçalho fora do lugar
* colunas sem nome
* valores com unidades misturadas
* tipos incorretos

### Dataset limpo (`seasonal_rainfall_clean.csv`)

Após o processo de limpeza, o dataset final possui o seguinte schema:

| Coluna                      | Tipo     | Descrição                                |
| --------------------------- | -------- | ---------------------------------------- |
| `month`                     | category | Mês (Jan–Dec), ordenado cronologicamente |
| `period_start`              | int      | Ano inicial do período                   |
| `period_end`                | int      | Ano final do período                     |
| `rainfall_mm_lake_victoria` | float    | Chuva média mensal (mm) no Lake Victoria |
| `rainfall_mm_simiyu`        | float    | Chuva média mensal (mm) em Simiyu        |

---

## 🔧 Etapas de Limpeza Realizadas

* Remoção de colunas irrelevantes (`Unnamed`)
* Correção do cabeçalho
* Separação da coluna `Month, period`
* Padronização de unidades (remoção de `mm`)
* Conversão de tipos (`float`, `category`, `int`)
* Ordenação categórica dos meses
* Organização semântica das colunas
* Validação de valores e tipos finais

---

## 🛠️ Tecnologias Utilizadas

* Python
* Pandas
* Jupyter Notebook

---

## 🎯 Objetivo do Projeto

Demonstrar domínio de:

* limpeza de dados reais (“messy data”)
* boas práticas em Pandas
* organização de projetos de dados
* preparação de datasets para análise e visualização

Este projeto pode ser facilmente expandido para:

* análise exploratória (EDA)
* visualizações climáticas
* estudos de sazonalidade

---

## 📌 Observações

Os dados representam **valores médios agregados**, não séries temporais completas por ano.
Por isso, os meses foram tratados como **variável categórica ordenada**, e não como `datetime`.

---

## 📜 Licença

Uso educacional e demonstrativo.

```

---

## ✅ Próximo passo recomendado (opcional)
Para deixar **ainda mais forte no GitHub**:
- adicionar **1 ou 2 gráficos** no notebook
- incluir **insights escritos** (ex: meses mais chuvosos)
- linkar esse projeto no seu README principal ou LinkedIn

Se quiser, posso:
- revisar o notebook com **comentários de portfólio**
- sugerir **gráficos que impressionam recrutador**
- adaptar esse README para **vaga de dados específica**

Só dizer 🚀
```
