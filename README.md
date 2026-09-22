# Classificação de doenças respiratórias

Um estudo de aprendizado de máquina que compara quatro modelos para distinguir **asma, bronquite aguda e pneumonia** a partir de sintomas. O notebook reúne a análise dos dados, a seleção de variáveis e a avaliação dos resultados.

[Abrir notebook](projeto_classificacao_doencas.ipynb) · [Dataset no Kaggle](https://www.kaggle.com/datasets/dhivyeshrk/diseases-and-symptoms-dataset)

**Python · Jupyter · scikit-learn · pandas · NumPy · Matplotlib · Seaborn**

## O estudo

- Exploração e filtragem do dataset para as três doenças respiratórias.
- Separação estratificada dos dados: **70% para treino e 30% para teste**.
- Seleção de sintomas com `SelectKBest` e qui-quadrado; escolha da quantidade de variáveis por pipeline e validação cruzada no treino.
- Comparação entre Árvore de Decisão, Random Forest, Regressão Logística e Rede Neural MLP.
- Avaliação com matrizes de confusão, métricas de classificação, análise de erros e discussão de overfitting.

## Resultados

As saídas salvas no notebook apresentam estes resultados para **999 amostras de teste**:

| Modelo | Acurácia | F1 ponderado |
|---|---:|---:|
| **Regressão Logística** | **90,19%** | **0,9026** |
| Árvore de Decisão | 89,99% | 0,9010 |
| Random Forest | 89,79% | 0,8983 |
| Rede Neural MLP | 89,79% | 0,8976 |

[Baixar métricas completas (CSV)](metricas_resultados.csv). As métricas correspondem às saídas salvas no notebook. Este é um estudo acadêmico, sem validação clínica.

## Executar localmente

Requer Python 3 e acesso ao repositório.

```bash
git clone https://github.com/figueirego/classificacao-doencas-respiratorias.git
cd classificacao-doencas-respiratorias
python3 -m venv .venv
source .venv/bin/activate
python -m pip install notebook numpy pandas scikit-learn matplotlib seaborn
```

No Windows, crie o ambiente com `python -m venv .venv` e ative-o no PowerShell com `.venv\Scripts\Activate.ps1`.

Baixe o dataset pelo link do Kaggle e coloque o arquivo **`Final_Augmented_dataset_Diseases_and_Symptoms.csv`** na raiz do repositório, ao lado do notebook. O dataset não está incluído no projeto.

```bash
python -m notebook projeto_classificacao_doencas.ipynb
```

Execute as células em ordem, do início ao fim. A etapa de comparação exporta **`metricas_resultados.csv`** na raiz. As versões das dependências ainda não estão fixadas; resultados podem variar entre ambientes.

## Autores

**João Matheus de Figueirêdo Tavares** e **Caio Moura Portela de Sousa**.

Sistemas de Informação · Unifacisa.

Professor: Bruno Rafael Araújo Vasconcelos.
