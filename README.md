# Case 4 – Classificador Supervisionado de Perfis

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/)
[![Databricks](https://img.shields.io/badge/Databricks-Notebook-orange)](https://databricks.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/status-active-success)]()

---

## 📌 Índice

1. [Sobre o Projeto](#-sobre-o-projeto)
2. [Arquitetura do Case](#-arquitetura-do-case)
3. [Instalação e Uso](#-instalação-e-uso)
4. [Resultados e Métricas](#-resultados-e-métricas)
5. [Exemplos de Saída](#-exemplos-de-saída)
6. [Estrutura do Repositório](#-estrutura-do-repositório)
7. [Contribuição](#-contribuição)
8. [Licença](#-licença)

---

## 📖 Sobre o Projeto

Este repositório contém o **Case 4 da Série “5 Cases Avançados de Data Science na Prática”**, onde transformamos **perfis latentes** (obtidos via clusterização) em um **classificador supervisionado** robusto e escalável.

* Algoritmo principal: **Random Forest Classifier**
* Avaliação com: **Kappa, F1-score, ROC-AUC**
* Explicabilidade: **Feature Importance**

---

## 🏗 Arquitetura do Case

* **Input**: Base de clientes + rótulos de perfis (Cases 1–3).
* **Modelagem**: Random Forest supervisionado.
* **Outputs**:

  * Relatório de métricas
  * Gráficos de curva ROC
  * Importância de features
  * Modelo exportado para deploy

---

## ⚙️ Instalação e Uso

### Clonar o repositório

```bash
git clone https://github.com/seuusuario/case4-classificador-perfis.git
cd case4-classificador-perfis
```

### Requisitos

* Python 3.9+
* Databricks ou ambiente local com PySpark
* Instalar dependências:

```bash
pip install -r requirements.txt
```

### Execução

* Importar o notebook `Case4_ClassificadorPerfis.ipynb` no **Databricks**
* Ajustar o caminho da base de dados em `config.py`
* Rodar pipeline completo para:

  * Treinar
  * Avaliar
  * Exportar resultados

---

## 📊 Resultados e Métricas

* **F1-score médio**: 0.87
* **Kappa**: 0.81
* **ROC-AUC médio**: 0.90

(Valores ilustrativos – a execução gera resultados atualizados)

---

## 📂 Estrutura do Repositório

```
├── notebooks/
│   └── Case4_ClassificadorPerfis.ipynb
├── src/
│   ├── preprocessing.py
│   ├── train_model.py
│   ├── evaluate.py
│   └── utils.py
├── data/
│   └── exemplo_data.csv
├── requirements.txt
├── config.py
├── LICENSE
└── README.md
```

---

## 🤝 Contribuição

Contribuições são bem-vindas!

1. Faça um fork do projeto
2. Crie sua feature branch (`git checkout -b feature/minha-feature`)
3. Commit suas alterações (`git commit -m 'Minha nova feature'`)
4. Faça push para a branch (`git push origin feature/minha-feature`)
5. Abra um Pull Request

---

## 📜 Licença

Distribuído sob a licença MIT. Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.
