# meu-modelo-predicao

Primeiro, criei um repositório no GitHub para armazenar todo o código e material do projeto. Em seguida, usei o **Azure AI Services** para criar um modelo de previsão de aluguéis de bicicletas com base em dados históricos. Dentro do portal do Azure, configurei um **workspace** do Azure Machine Learning para organizar todos os recursos necessários. No Azure Machine Learning Studio, criei um novo job de **Automated Machine Learning** com o objetivo de prever os aluguéis de bicicletas com base em dados como temperatura, dia da semana e outros fatores meteorológicos.

Durante a configuração do job, selecionei o tipo de tarefa como **Regressão** e fiz o upload do dataset de aluguéis de bicicletas. Escolhi os modelos **RandomForest** e **LightGBM** para o treinamento, e configurei limites como o número de tentativas e o tempo máximo de execução para otimizar o processo. Após submeter o job, o modelo foi treinado automaticamente e, assim que o treinamento foi concluído, analisei o desempenho do melhor modelo, verificando as métricas e gráficos que comparavam as previsões com os valores reais.

Depois disso, configurei um **ponto de extremidade** para o modelo, criando um **endpoint em tempo real** no Azure. Isso me permitiu fazer previsões com o modelo treinado, utilizando dados de entrada no formato JSON. Testei o ponto de extremidade substituindo o JSON de entrada pelos dados de teste e obtive a previsão de aluguéis de bicicletas para um determinado dia.

Por fim, documentei todo o processo no **README.md** do repositório, detalhando como configurei o modelo, os pontos de extremidade e como testar o modelo, para que outras pessoas pudessem entender o fluxo completo.
