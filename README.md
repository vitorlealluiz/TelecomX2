# 📊 TelecomX: Inteligência Artificial para Prevenção de Churn

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)

Este projeto utiliza **Machine Learning** para identificar padrões de comportamento e prever a evasão de clientes (Churn) na empresa **TelecomX**. O objetivo é transformar dados brutos em inteligência estratégica para reduzir a perda de receita.

---

## 📂 Estrutura do Projeto

- **Análise Exploratória (EDA):** Identificação de correlações e outliers.
- **Pré-processamento:** One-Hot Encoding, Normalização e tratamento de desbalanceamento com **SMOTE**.
- **Modelagem:** Implementação e comparação entre Regressão Logística e Random Forest.
- **Avaliação:** Foco em métricas de negócio (Recall e F1-Score).

---

## 📈 Resultados e Performance

Para o setor de Telecom, identificar o máximo de clientes em risco é mais importante do que a acurácia total. Por isso, focamos no **Recall**.

| Modelo | Acurácia | Recall (Sensibilidade) | F1-Score |
| :--- | :---: | :---: | :---: |
| **Regressão Logística** | 75% | **81%** | **0.62** |
| **Random Forest** | **78%** | 49% | 0.54 |

> **Veredito:** A **Regressão Logística** foi selecionada como o modelo ideal para produção, pois consegue capturar 81% dos clientes que realmente pretendem cancelar o serviço, permitindo uma ação preventiva eficaz.

---

## 🔍 Principais Drivers de Evasão

Através da análise de correlação e importância de variáveis, identificamos os 3 maiores fatores que levam ao Churn:

1.  **Tipo de Contrato:** Clientes com contrato mensal (`month-to-month`) são os mais propensos a sair.
2.  **Tecnologia:** Usuários de Fibra Óptica apresentam uma taxa de evasão curiosamente superior aos de DSL.
3.  **Tempo de Casa (Tenure):** Clientes nos primeiros 6 meses de contrato possuem o maior risco crítico.

---

## 💡 Recomendações Estratégicas

Com base nos dados, propomos as seguintes ações para a diretoria:

* **Fidelização Ativa:** Criar campanhas de upgrade para planos anuais focadas em clientes de planos mensais.
* **Qualidade da Fibra:** Realizar uma auditoria técnica e de satisfação com usuários de fibra óptica para entender a fricção.
* **Barreira de Saída:** Oferecer serviços de *Suporte Técnico* e *Segurança Online* como bônus, dado que clientes com esses serviços ativos evadem menos.

---

## 🚀 Como Executar

1.  Clone o repositório:
    ```bash
    git clone [https://github.com/vitorlealluiz/telecomX2.git](https://github.com/vitorlealluiz/telecomX2.git)
    ```
2.  Abra o arquivo `.ipynb` no [Google Colab](https://colab.research.google.com/).
3.  Certifique-se de realizar o upload do arquivo `Telecom_tratado.csv`.
4.  Execute as células para visualizar os gráficos e métricas.

---

## 👤 Autor

**Vitor Leal** *Estudante de Análise e Desenvolvimento de Sistemas - UNICAMP*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vitorluizleal/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vitor.lealprof@gmail.com)

---
*Este projeto faz parte do meu portfólio de estudos em Inteligência Artificial e Ciência de Dados.*
