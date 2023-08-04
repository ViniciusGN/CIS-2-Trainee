# 2º Fase Trainee CIS
Este projeto faz parte do processo Trainee do Computational Inteligence Society (CIS) - IEEE, Capítulo Estudantil, - da Universidade de Brasília (UnB): Semana 2. Aluno: Vinicius Nascimento

## a) "Classificação binária para prever se o vinho é tinto ou não":
O dataset designado foi "Qualidade do Vinho" disponível no link [(Fonte)]([https://drive.google.com/file/d/14Y6ZJYI-sB_T9tHexlg2GCSfLCmC6eQE/view)). Utilizei o método KNN (K-Nearest Neighbours) para verificar se o vinho era tinto com base na classificação binária. A coluna de referência foi a Wine_Is_Red, sendo a última coluna do dataset. O método KNN está disponível através da biblioteca SKLearn do Python, obtendo uma acurácia de 93% com um conjunto de 80% de treinamento e 20% de teste do conjunto de dados fornecido.

## b) "Classificação multiclasse para prever a qualidade do vinho":
Para prever a qualidade do vinho, verifiquei que alguns autores de fontes de consulta emitiam uma matriz de correlação dos dados. Após emitir a matriz, é possível observar quais são os fatores que possuem uma correlação de dados com a qualidade do vinho (última coluna). O mapeamento do parâmetro é feito através da relação Número da Coluna-Nome.
Em seguida, utilizei os conceitos de Randon Forest para verificar o que foi solicitado, já atuando no item d. proposto.

## d) "Feature Importance - Aplicar ao algoritmo Random Forest e determinar quais features do dataset são mais importantes para o problema":
Após obter uma acurácia de 68%, verificamos que o modelo é insuficiênte para realizar a predição. Extraí a matriz de confusão dos dados para verificar quais classes foram mais acertivas dentro do conjunto de dados, observando que, em geral, o modelo foi capaz de acertar mais os vinhos de classe 3.
Em seguida, emiti a importância das features do modelo, conforme solicitado.

## e) "Aplicar a normalização nos dados e verificar os efeitos nos modelos":
Realizei a normalização dos dados e verifiquei que o KNN possuía acurácia de 58.15% e o Randon Forest possuía uma acuáracia de 69%. Verifiquei que alguns autores avaliaram a quantidade de vinhos de cada tipo de classificação de qualidade, e observei que há mais vinhos de classe 6, 5 e 7 respectivamente. Entendi, posteriomente, a importância de verificar o equilibrio no conjunto de dados ao aplicar os conceitos apresentados no item f. 

## f) "Aplicar as técnicas de undersampling e oversampling nos dados. Verificar e explicar os efeitos":
- _"Oversampling (superamostragem): É uma técnica que consiste em aumentar artificialmente o número de instâncias da classe minoritária, para tornar as proporções das classes mais equilibradas. Isso é geralmente feito através da replicação de amostras existentes da classe minoritária ou da geração de novas instâncias sintéticas baseadas nas amostras existentes."_
- _"Undersampling (subamostragem): É uma técnica que consiste em reduzir o número de instâncias da classe majoritária para alcançar um equilíbrio com a classe minoritária. Isso é realizado removendo aleatoriamente ou selecionando estrategicamente um subconjunto das amostras da classe majoritária."_
Como as amostras mais próximas da borda do gráfico de frequência do nível de qualidade eram muito menores que os valores das classes 5, 6 e 7, optei por realizar o procedimento de oversampling, que seria mais adequado para o conjunto de dados. Para isso utilizei a biblioteca imblearn que realiza os procedimentos de amostragem (sampling) através de um import.

## g) "Aplicar um dos métodos de Ensemble Learning e comparar os resultados":
- _"Ensemble Learning, ou aprendizado em conjunto, é uma abordagem no campo de aprendizado de máquina em que múltiplos modelos são combinados para realizar uma tarefa preditiva ou classificatória. Em vez de confiar em um único modelo para fazer uma previsão, o ensemble learning utiliza a sabedoria coletiva de vários modelos para melhorar a precisão e o desempenho geral do sistema."_

## h) "implementar um KNN utilizando somente numpy":
Realizado, não foi utilizado a biblioteca Pandas. Achei que a biblioteca seria útil para plotar o gráfico do tipo bloxpot e verificar os dados outliers de algumas features consideradas importantes para a qualidade do vinho, conforme observado na matriz de correlação.

### Observações:
Os conteúdos utilizados foram:
- KNN (K-Nearest Neighbours)
- Support Vector Machine
- Decision Tree
- Random Forest
- Classificação binária
- Classificação multiclasse
- Métricas de Avaliação (Cross-validation, Confusion Matrix, Precision e Recall)
- Ensemble Learning.
- Limpeza e manipulação de dados

![thinkstockphotos-615269202](https://github.com/ViniciusGN/CIS-2-Trainee/assets/80403948/6cdd6189-8eba-416f-81ba-56f68b9633d6)

### Curiosidade: 
Você sabia que acredita-se que as vinhas mais antigas do mundo estão localizadas na região da Cachemira, no norte da Índia?
