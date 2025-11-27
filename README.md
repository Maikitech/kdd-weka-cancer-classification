# kdd-weka-cancer-classification
Aplicação do processo KDD para classificação de tumores de mama (Benigno/Maligno) utilizando o algoritmo J48 (Árvore de Decisão) no Weka com 93% de acurácia.


# 🎗️ Análise Preditiva de Câncer de Mama com KDD

## 📋 Sobre o Projeto

Este projeto consiste na aplicação prática do processo de **Descoberta de Conhecimento em Bases de Dados (KDD)** para auxiliar no diagnóstico médico de câncer de mama.

O objetivo foi treinar um modelo de Inteligência Artificial capaz de classificar tumores como **Benignos** ou **Malignos** com base em características geométricas de células extraídas por exames de imagem (PAAF).

## 🗃️ A Base de Dados

Utilizamos o dataset clássico **Breast Cancer Wisconsin (Diagnostic)**.

* **Fonte:** UCI Machine Learning Repository.
* **Registros:** 569 instâncias (pacientes).
* **Atributos:** 30 características numéricas (Raio, Textura, Área, etc.) + 1 Classe.
* **Origem:** Medições computacionais extraídas de imagens digitais de núcleos celulares.

## ⚙️ Metodologia (Processo KDD)

O projeto seguiu rigorosamente as etapas de mineração de dados utilizando o software **Weka**:

1. **Seleção:** Escolha da base de dados sem valores ausentes.
2. **Pré-processamento:** Remoção de identificadores (`id`) e tradução dos dados para melhor interpretabilidade.
3. **Mineração (Data Mining):** Utilização do algoritmo **J48** (implementação do C4.5) para gerar uma Árvore de Decisão.
4. **Avaliação:** Validação do modelo via **10-Fold Cross-Validation**.

## 📊 Resultados Alcançados

O modelo final obteve um desempenho excelente, validando o uso de IA como ferramenta de apoio ao diagnóstico.

| Métrica | Resultado |
| :--- | :--- |
| **Acurácia Geral** | **93,32%** |
| Instâncias Corretas | 531 |
| Instâncias Incorretas | 38 |
| Precision (Maligno) | 89,5% |
| Recall (Maligno) | 92,9% |

### 🧠 Descoberta de Conhecimento

A árvore de decisão revelou que a **Área da Célula** e a **Textura** são os fatores mais determinantes para o diagnóstico.

> **Regra Principal Descoberta:** Se `pior_area <= 880.8`, a probabilidade de o tumor ser Benigno é altíssima.

## 🚀 Como Visualizar

Este repositório contém uma **página web interativa** (`index.html`) que apresenta todo o estudo, a árvore de decisão completa e a análise detalhada.

1. Baixe este repositório.
2. Abra o arquivo `index.html` no seu navegador.

## 👨‍💻 Autor

**Maiki Scalvi**
Projeto desenvolvido para a disciplina de Banco de dados 3 IFRS - 2025/2.

*Este projeto utiliza dados públicos para fins educacionais e de pesquisa.*
