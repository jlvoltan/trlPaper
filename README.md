# Technology Readiness Level - TRL 

📌  It's a repository for the paper xxxxx focused on the document classification problem using the TRL scale.

📌  Here we find the [_corpus/dataset_](https://github.com/jlvoltan/trlPaper/tree/main/dataset)  constructed and [models](https://github.com/jlvoltan/trlPaper/tree/main/modelos) for this task.
  
✏️  Further explanations about the methodology used can be found in the written article.



### 📝 Abstract 📝

The TRL scale emerged in the 1970s with the purpose of measuring the technological maturity of a product or technology. From the 2000s onwards, it gained prominence in various organizations and companies around the world, being employed not only in project monitoring but also in technology management and foresight. Despite this increased importance, the predominant approach to assessing the TRL level of a technology or product, _i.e._, the Technology Readiness Assessment (TRA), is based on expert evaluation. This approach has disadvantages such as high cost, delay, and possible bias. Given this scenario, the problem arises: how could a scalable TRA be conducted with lower cost and greater standardization of criteria? Automated TRA proposals are few and have room for improvement.

An important gap exists in the lack of a methodology for corpus construction. In this work, a methodology was proposed and applied to the Defense domain, gathering 168 scientific articles and news written in Brazilian Portuguese (PT-BR). The study grouped the nine TRL levels into three ranges, labeling all collected documents through expert support with the aid of a form. Finally, quantitative and qualitative analyses were conducted regarding the dataset. The performance of classical ML algorithms combined with the TF-IDF vector representation technique was also evaluated.


### 💬 Brief explanation 💬

- In this work, we built a [_corpus_](https://github.com/jlvoltan/trlPaper/tree/main/dataset) using news and scientific articles. They are located in the folder [_dataset_]((https://github.com/jlvoltan/trl/tree/main/dataset));

- In the [questionnaire,](https://github.com/jlvoltan/trl/tree/main/questionnaire) folder there is a file that synthesizes this _corpus_, in the form of a spreadsheet.

- In the [_manipulates_](https://github.com/jlvoltan/trl/tree/main/manipulates) folder, There are some notebooks related to the analysis of the _corpus_ and preprocessing.

- Finally, in the [_models_](https://github.com/jlvoltan/trl/tree/main/modelos) folder, snotebooks of the experiments are presented, where the vector representation was obtained using the TF-IDF technique, and subsequently, classification models were trained and tested
