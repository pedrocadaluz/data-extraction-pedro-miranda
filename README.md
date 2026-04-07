# Portfólio de Extração e Preparação de Dados

**Aluno:** Pedro Arthur da Luz Miranda
**Curso:** Ciência de Dados & IA | IBMEC-DF
**Semestre:** 2026.1
**Disciplina:** Extração e Preparação de Dados (IBM8915)
**Professor:** Luís Aramis

---

## 📋 Sobre Este Repositório
Este repositório armazena as atividades práticas e laboratórios desenvolvidos durante a disciplina. O foco é dominar as técnicas de ingestão, tratamento e estruturação de dados para alimentar modelos de Inteligência Artificial e dashboards analíticos.

---

## 🗂️ Cronograma de Atividades

### 🔹 Módulo 1: Extração e Análise Exploratória (Raw Data)
*Foco na obtenção de dados e diagnóstico inicial.*

| Lab | Status | Atividade | Competências |
| :--- | :---: | :--- | :--- |
| **Lab 01** | ✅ | [Arquivos Planos](./notebooks/lab_01_flat_files.ipynb) | Ingestão de CSV, JSON e Excel com Pandas. |
| **Lab 02** | ✅ | [Extração SQL (Chinook)](./notebooks/lab_02_sql_extraction.ipynb)<br>[Extração SQL (Northwind)](./notebooks/lab_02_extra_northwind.ipynb) | Queries complexas e conexões via SQLAlchemy. |
| **Lab 03** | ✅ | [EDA Básico](./notebooks/lab_03_eda_basics.ipynb)<br>[EDA Avançado](./notebooks/lab_03_eda_advanced.ipynb) | Identificação de outliers, análise de distribuição e exploração avançada. |

### 🔹 Módulo 2: Limpeza e Transformação (Data Wrangling)
*Tratamento de inconsistências e preparação para modelagem.*

| Lab | Status | Atividade | Competências |
| :--- | :---: | :--- | :--- |
| **Lab 04** | ✅ | [Visualização de Nulos — Titanic](./notebooks/lab_04_missing_values_viz_Tinanic.ipynb)<br>[Visualização de Nulos — IRIS/DATASUS](./notebooks/Lab_04_missing_values_viz_iris_datasus.ipynb)<br>[Script Dataset Sujo](./scripts/lab_04_dataset_sujo.py) | Diagnóstico visual de valores ausentes com heatmaps e análise de padrões de nulidade. |
| **Lab 05** | ✅ | [Imputação Univariada e Multivariada](./notebooks/lab_05_imputation.ipynb) | `dropna`, `fillna` com mediana/moda, `KNNImputer` do Scikit-Learn. |
| **Lab 06** | ✅ | [Alta Cardinalidade](./notebooks/lab_06_cardinality.ipynb) | Diagnóstico de cauda longa, agrupamento de categorias raras em `'Outros'`. |
| **Lab 07** | ✅ | [Encoders — Parte 1](./notebooks/lab_07_encoders.ipynb)<br>[Encoders — Parte 2 (Avançado)](./notebooks/lab_07_parte_02_advanced.ipynb) | Ordinal Encoding com `.map()`, One-Hot Encoding com `pd.get_dummies()` e armadilha da variável dummy. |
| **Lab 08** | ✅ | [Binning / Discretização](./notebooks/lab_08_binning.ipynb) | `pd.cut` (cortes absolutos) vs `pd.qcut` (quantis) em dados com distribuição assimétrica. |
| **Lab 09** | ✅ | [Engenharia de Datas (Datetime)](./notebooks/lab_09_datetime.ipynb) | `pd.to_datetime`, acessor `.dt`, extração de sazonalidade e cálculo de deltas temporais. |
| **Lab 10** | ✅ | [Feature Engineering Numérico](./notebooks/lab_10_feature_engineering.ipynb) | Criação de ratios, flags booleanas e encadeamento funcional com `.assign()`. |
| **Lab 11** | ✅ | [Detecção e Tratamento de Outliers](./notebooks/lab_11_outliers.ipynb) | Boxplot, Regra do IQR, Winsorization com `.clip()` e `IsolationForest` multivariado. |
| **Lab 12** | ✅ | [Escalonamento e Desbalanceamento](./notebooks/lab_12_scaling_smote.ipynb) | `StandardScaler`, split seguro e geração sintética de minoria com `SMOTE`. |

### 🔹 Módulo 3: Feature Selection e Pipelines
*Redução dimensional e automação do fluxo de pré-processamento.*

| Lab | Status | Atividade | Competências |
| :--- | :---: | :--- | :--- |
| **Lab 13** | ✅ | [SelectFromModel](./notebooks/lab_13_select_model.ipynb) | Seleção de atributos por importância com `RandomForestClassifier` e `SelectFromModel`. |
| **Lab 14** | ✅ | [RFE — Eliminação Recursiva](./notebooks/lab_14_rfe.ipynb) | `RFE` (Recursive Feature Elimination) com controle preciso de `n_features_to_select`. |
| **Lab 15** | ✅ | [Pipelines do Scikit-Learn](./notebooks/lab_15_pipelines_intro.ipynb) | Arquitetura de `Pipeline`, encadeamento de transformadores e proteção contra Data Leakage. |

---

## 🛠️ Tecnologias e Ferramentas
* **Linguagem:** Python 3.13+
* **Gerenciador de Pacotes:** [uv](https://github.com/astral-sh/uv)
* **Bibliotecas:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, imbalanced-learn, SQLAlchemy, Requests
* **Banco de Dados:** SQLite (Chinook, Northwind)
* **Versionamento:** Git & GitHub

---

## 🚀 Configuração do Ambiente com `uv`

Este projeto utiliza o modo gerenciado do **uv** para garantir que o ambiente seja reprodutível e ultra-rápido.

### 1. Instalação do uv
Caso não tenha o `uv` instalado, utilize o comando:
* **Windows:** `powershell -c "irm https://astral.sh/uv/install.ps1 | iex"`
* **Linux/macOS:** `curl -LsSf https://astral.sh/uv/install.sh | sh`

### 2. Sincronizando o Projeto
Para criar o ambiente virtual e instalar todas as dependências (baseadas no `pyproject.toml` e `uv.lock`), execute:

```bash
# Sincroniza o ambiente automaticamente
uv sync
```

[Documentação do uv](https://github.com/astral-sh/uv?tab=readme-ov-file)
