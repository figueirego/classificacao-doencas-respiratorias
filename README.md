# Classificação de doenças respiratórias

Projeto acadêmico de João Matheus de Figueirêdo Tavares e Caio Moura Portela de Sousa, desenvolvido no curso de Sistemas de Informação da Unifacisa, na disciplina do professor Bruno Rafael Araújo Vasconcelos.

A implementação principal é [projeto_classificacao_doencas.ipynb](projeto_classificacao_doencas.ipynb), mantida neste repositório. Ela compara Árvore de Decisão, Random Forest, Regressão Logística e MLP na classificação de doenças respiratórias a partir de sintomas.

## Versão mantida

O notebook mais recente separa treino e teste antes da seleção de variáveis e utiliza validação cruzada com pipeline no conjunto de treino para selecionar a quantidade de variáveis. Inclui métricas adicionais, análise de erros e discussão de overfitting.

O notebook foi preservado sem alterações nesta consolidação. Não foi reexecutado: o dataset deve ser obtido conforme a referência e o nome de arquivo indicados no próprio notebook. A presença de resultados salvos não significa que tenham sido recalculados nesta reorganização.

## Documentação histórica

- [Artigo da versão anterior](docs/historico/2026-03-jupyter/artigo_classificacao_doencas.pdf)
- [Apresentação da versão anterior](docs/historico/2026-03-jupyter/apresentacao_classificacao_doencas.pptx)
- [Métricas da versão anterior do Jupyter](docs/historico/2026-03-jupyter/metricas_resultados.csv)
- [CSV anteriormente versionado nesta implementação](docs/historico/metricas_resultados-anteriores-att.csv)

Esses documentos e CSVs foram preservados como histórico. Seus valores não representam necessariamente a versão atual do notebook. O antigo CSV da raiz estava desatualizado em relação às células e saídas salvas; ele foi movido para esta área, sem alterar os dados. Ao reexecutar o notebook, a célula de exportação gera `metricas_resultados.csv` na raiz.
