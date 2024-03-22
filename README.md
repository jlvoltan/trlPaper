# Technology Readiness Level - TRL 

📌  It's a repository for the paper xxxxx focused on the document classification problem using the TRL scale.

📌  Here we find the [_corpus/dataset_](https://github.com/jlvoltan/trlPaper/tree/main/dataset)  constructed and [models](https://github.com/jlvoltan/trlPaper/tree/main/modelos) for this task.
  
✏️  Further explanations about the methodology used can be found in the written article.



### 📝 Abstract 📝

A escala TRL surgiu na década de 70, com o propósito de mensurar a maturidade tecnológica de um produto ou tecnologia. A partir dos anos 2000, ganhou destaque em diversos órgãos e empresas ao redor do mundo, tendo emprego não só no acompanhamento de projetos, como também na gestão e prospecção tecnológica. Apesar desse aumento de importância, a abordagem predominante para avaliar o nível TRL de uma tecnologia ou produto, _i.e._, a Avaliação de Prontidão Tecnológica (_Technology Readiness Assessment_ - TRA), é baseada na avaliação de especialistas. Tal abordagem tem como desvantagens o elevado custo, demora, além de um possível viés. Diante desse cenário, tem-se o problema, de como seria possível realizar uma TRA escalável, com um menor custo e maior padronização de critérios. As propostas de TRA automatizadas são poucas e apresentam espaço para aprimoramento.


An important gap exists in the lack of a methodology for corpus construction. In this work, a methodology was proposed and applied to the Defense domain, gathering 168 scientific articles and news written in Brazilian Portuguese (PT-BR). The study grouped the nine TRL levels into three ranges, labeling all collected documents through expert support with the aid of a form. Finally, quantitative and qualitative analyses were conducted regarding the dataset. The performance of classical ML algorithms combined with the TF-IDF vector representation technique was also evaluated.


### 💬 Brief explanation 💬

- In this work, we built a [_corpus_](https://github.com/jlvoltan/trlPaper/tree/main/dataset) using news and scientific articles. They are located in the folder [_dataset_]((https://github.com/jlvoltan/trl/tree/main/dataset));

- In the [questionnaire,](https://github.com/jlvoltan/trl/tree/main/questionnaire) folder there is a file that synthesizes this _corpus_, in the form of a spreadsheet.

- In the [_manipulates_](https://github.com/jlvoltan/trl/tree/main/manipulates) folder, There are some notebooks related to the analysis of the _corpus_ and preprocessing.

- Finally, in the [_models_](https://github.com/jlvoltan/trl/tree/main/modelos) folder, snotebooks of the experiments are presented, where the vector representation was obtained using the TF-IDF technique, and subsequently, classification models were trained and tested
