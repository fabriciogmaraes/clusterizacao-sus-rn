# 🏥 Clusterização de Unidades de Saúde do SUS (Rio Grande do Norte)
*Análise de Agrupamento de Dados Geográficos e Estruturais*

[![Language](https://img.shields.io/badge/Language-Python-blue.svg)](https://www.python.org/)
[![Course](https://img.shields.io/badge/Course-Data_Science-success.svg)]()
[![Institution](https://img.shields.io/badge/Institution-UFRN_|_PPgTI-red.svg)](https://www.imd.ufrn.br/)

> 🇧🇷 Para a versão em Português, continue lendo.
> 🇬🇧 [For the English version, click here](#-english-version).

---

## 🇧🇷 Sobre o Projeto

Este projeto é o Trabalho Prático Final da disciplina de **Ciência de Dados**, do **Mestrado Profissional em Inovação em Tecnologias da Informação (PPgTI)** do Instituto Metrópole Digital da Universidade Federal do Rio Grande do Norte (IMD/UFRN).

O objetivo principal é aplicar técnicas de **Aprendizado de Máquina Não Supervisionado** para descobrir padrões estruturais e geográficos nas unidades de saúde (UBS, UPAs, Hospitais) do Sistema Único de Saúde (SUS) localizadas no estado do Rio Grande do Norte.

### ⚙️ Metodologia e Fases

O projeto está estruturado nas seguintes etapas:

* **Fase 1: Pré-processamento de Dados**
    * Filtragem geográfica para o estado do RN (IBGE 24).
    * Tratamento de dados faltosos (Missing Values).
    * Limpeza espacial e remoção de outliers utilizando o Intervalo Interquartil (IQR) nas coordenadas de latitude e longitude.
    * Transformação de variáveis categóricas utilizando *One-Hot Encoding*.
    * Normalização de escala utilizando `StandardScaler`.
* **Fase 2: Algoritmos de Clusterização (Em Desenvolvimento)**
    * K-Means (com variações de inicialização).
    * Hierárquico Aglomerativo (com variações de *linkage*).
    * Expectation Maximization / Gaussian Mixture (com variações de covariância).
* **Fase 3: Validação**
    * Avaliação da qualidade dos grupos utilizando os índices **Silhouette** e **Davies-Bouldin (DB)**.

### 🚀 Como Executar

1. Clone este repositório.
2. Certifique-se de ter as bibliotecas `pandas`, `numpy` e `scikit-learn` instaladas.
3. Baixe os microdados do CNES (Cadastro Nacional de Estabelecimentos de Saúde) no portal OpenDataSUS.
4. Execute os notebooks na ordem numérica.

---

<a id="-english-version"></a>
## 🇬🇧 English Version

## 🏥 SUS Healthcare Facilities Clustering (Rio Grande do Norte)

This project is the final practical assignment for the **Data Science** course in the **Professional Master's Program in Information Technology Innovation (PPgTI)** at the Federal University of Rio Grande do Norte (IMD/UFRN), Brazil.

The main objective is to apply **Unsupervised Machine Learning** techniques to discover structural and geographical patterns in the Brazilian Unified Health System (SUS) facilities located in the state of Rio Grande do Norte.

### ⚙️ Methodology and Phases

The pipeline is structured as follows:

* **Phase 1: Data Preprocessing**
    * Geographical filtering for the state of RN.
    * Missing values imputation.
    * Spatial cleaning and outlier removal using the Interquartile Range (IQR) on latitude and longitude coordinates.
    * Categorical feature transformation using *One-Hot Encoding*.
    * Feature scaling using `StandardScaler`.
* **Phase 2: Clustering Algorithms (WIP)**
    * K-Means (with initialization variations).
    * Agglomerative Hierarchical (with linkage variations).
    * Expectation Maximization / Gaussian Mixture (with covariance variations).
* **Phase 3: Validation**
    * Cluster quality evaluation using **Silhouette** and **Davies-Bouldin (DB)** indexes.

### 🚀 How to Run

1. Clone this repository.
2. Ensure you have `pandas`, `numpy`, and `scikit-learn` installed in your environment.
3. Download the CNES microdata from the OpenDataSUS portal.
4. Run the Jupyter Notebooks in numerical order.

---
**Autor / Author:** Fabrício Guimarães
