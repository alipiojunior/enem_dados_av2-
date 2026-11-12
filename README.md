# Predição do Desempenho em Ciências da Natureza no ENEM 2023

**Universidade de Fortaleza (UNIFOR)**
**Curso:** Ciência da Computação - 2026.2
**Disciplina:** Ciência de Dados - AV2
**Autores:** Alípio Rollo Júnior, Arthur Victor, José Otávio, Thiago Rabelo Cavalcante.

## 🎯 Objetivo do Projeto
Este repositório contém o desenvolvimento de modelos de Aprendizado de Máquina (Regressão) para prever a nota da prova de Ciências da Natureza (`NU_NOTA_CN`) do ENEM 2023. A modelagem foi construída exclusivamente a partir do perfil demográfico, contexto escolar e questionário socioeconômico dos participantes, aplicando um rigoroso protocolo de prevenção de vazamento de dados (*data leakage*).

## 📂 Estrutura do Repositório
* **`dados/`**: Diretório reservado para o arquivo bruto de microdados (ignorado no versionamento devido ao tamanho).
* **`docs/`**: Contém a documentação final do projeto em PDF formatada nos padrões ABNT e os slides do Pitch presencial.
* **`notebooks/`**: Contém o Jupyter Notebook (`.ipynb`) com o código de limpeza, engenharia de *features*, testes estatísticos e treinamento dos modelos.

## 🚀 Como Reproduzir o Projeto
1. Clone este repositório para a sua máquina local.
2. Instale as dependências executando: `pip install -r requirements.txt`
3. Faça o download dos **Microdados do ENEM 2023** no portal oficial do INEP.
4. Extraia o arquivo `MICRODADOS_ENEM_2023.csv` e coloque-o dentro da pasta `dados/`.
5. Execute o notebook presente na pasta `notebooks/` sequencialmente.

## 🏆 Resultados Obtidos
O modelo *HistGradientBoosting* otimizado via *RandomizedSearchCV* apresentou o melhor desempenho geral, extraindo o limite teórico preditivo dos metadados socioeconômicos sem incorrer em sobreajuste (RMSE de 67,06 e $R^2$ de 0,2535 no conjunto de teste).