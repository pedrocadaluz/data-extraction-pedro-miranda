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
| **Lab 01** | ✅ | [Arquivos Planos](./notebooks/lab_01.ipynb) | Ingestão de CSV, JSON e Excel com Pandas. |
| **Lab 02** | ✅ | [Extração SQL](./notebooks/lab_02.ipynb) | Queries complexas e conexões via SQLAlchemy. |
| **Lab 03** | 🔄 | [EDA Inicial](./notebooks/lab_03.ipynb) | Identificação de outliers e análise de distribuição. |

### 🔹 Módulo 2: Limpeza e Transformação (Data Wrangling)
*Tratamento de inconsistências e preparação para modelagem.*

| Lab | Status | Atividade | Competências |
| :--- | :---: | :--- | :--- |
| **Lab 04** | ⏳ | Em breve... | Tratamento de valores nulos e duplicatas. |
| **Lab 05** | ⏳ | Em breve... | Normalização e padronização de escalas. |

### 🔹 Módulo 3: Web Scraping e APIs
*Coleta de dados de fontes externas e dinâmicas.*

| Lab | Status | Atividade | Competências |
| :--- | :---: | :--- | :--- |
| **Lab 06** | ⏳ | Em breve... | Consumo de APIs REST e autenticação. |

---

## 🛠️ Tecnologias e Ferramentas
* **Linguagem:** Python 3.10+
* **Gerenciador de Pacotes:** [uv](https://github.com/astral-sh/uv)
* **Bibliotecas:** Pandas, NumPy, SQLAlchemy, Requests
* **Banco de Dados:** SQLite / PostgreSQL
* **Versionamento:** Git & GitHub

---

## 🚀 Configuração do Ambiente com `uv`

Este projeto utiliza o modo gerenciado do **uv** para garantir que o ambiente seja reprodutível e ultra-rápido.

### 1. Instalação do uv
Caso não tenha o `uv` instalado, utilize o comando:
* **Windows:** `powershell -c "ircl https://astral-sh.uv/install.ps1 | iex"`
* **Linux/macOS:** `curl -LsSf https://astral-sh.uv/install.sh | sh`

### 2. Sincronizando o Projeto
Para criar o ambiente virtual e instalar todas as dependências (baseadas no `pyproject.toml` e `uv.lock`), execute:

```bash
# Sincroniza o ambiente automaticamente
uv sync

[Documentação do uv](https://github.com/astral-sh/uv?tab=readme-ov-file)j