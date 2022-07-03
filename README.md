# Image-multilabel-classification

Avanços no campo da inteligência artificial têm se mostrado promissores. O desenvolvimento computacional permitiu que algoritmos e técnicas, antes inviáveis de serem implementadas, tornasem-se passível de implementação.

Algoritmos de aprendizado de máquina passaram a ser usados em diversos campos, como o setor financeiros, saúde, educação e diversos outros. Uma aplicação com grande potencial de benefícios é a identificação de imagens.

A complexidade dentro do trabalho com imagens é alto, além do custo computacional de processamento e armazenamento, o pré processamento das imagens exige técnicas intrincadas. Ao longo dos anos vários trabalhos tem sido desenvolvidos com a intenção de classificar corretamente imagens, e os algoritmos implementados são tão caros computacionalmente quanto o pré processamento das imagens. Com isso, obtêm-se uma combinação traiçoeira: técnicas computacionais de processamento e análise altamente avançadas e custosas.

Este trabalho foi desenvolvido para a disciplina de IHC do mestrado em computação aplicada da UDESC-CTT e tem como objetivo propor a utilização de um algoritimo  ensemble de árvores de decisão para a classificação de imagens.O dataset utilizado para a validação do experimento é o MNIST, este dataset contém 60 mil amostras em tamanho 28x28 de digitos numéricos escritos à mão, variando de números de 0 à 9. O dataset está disponível gratuitamente na biblioteca TensowFlow, criada pelo Google.

Este modelo, por sua vez, oferece um custo computacional melhor sem comprometer a qualidade das predições.

Os dados foram divididos em um conjunto de treino e outro conjunto de teste, em seguida os labels dos conjuntos foram criados.

Uma técnica de cross validation também foi aplicada.

O algoritmo utilizado na classificação foi o LightGBM um modelo ensamble formado por árvores de decisão, e outro algoritmo chamado Bayesian search  foi utilizado para a otimização dos hiperparâmetros.

As métricas de utilizadas para avaliar a qualidade do modelo foram: acurácia, precisão, f1-score e recall.

A primeira versão do modelo foi feita sem a utilização de qualquer otimização nos hiperparâmetros ou validação dos dados.Para o segundo modelo uma etapa de cross validation foi implementada, com o parâmetro cv=5, que indica que o modelo será dividido em cinco grupos, onde quatro serão usados como treinamento e um para teste.

O resultado obtido não foi superior ao modelo baseline, alcançando os mesmos 0.97 na acurácia.

Para a última versão do modelo foram testados diversas combinações de hiperparâmetros utilizando o algoritmo Bayesian search.Após a otimização o modelo atingiu acurácia de 0.9812.
