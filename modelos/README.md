# 🤖 Modelos 🤖

## Dataset
De forma geral, utilizou-se 3 possíveis **datasets**: c1 (dataset.csv), c2(dataset_pre_processado_1.csv) e c3(dataset_pre_processado_stem_2.csv) com níveis crescentes de pré-processamento. Esses _datasets_ foram particionados utilizando-se a técnica um k-fold com k=5.

## Técnicas de representação vetorial

|	  **Técnica/modelo** | **Biblioteca**  | **Especificação** |
| ------------- | ------------- | ------------- |
| TF-IDF | Scikit-learn    | *TfidfVectorizer*  |
|BERT  | Hugging Face    | *BERT-base-multilingual-cased*  |
| BERTimbau    | Hugging Face  | *neuralmind/bert-base-portuguese-cased*   |
| GPT-2  | Hugging Face    | *pierreguillou/gpt2-small-portuguese* |







## Dos cadernos:

### 2_tf_idf_resumo_XX_sem_grid.ipynb
Esses modelos empregaram a representação vetorial TF-IDF combinada com algoritmos de ML, não se utilizou um método de otimização de parâmetros (sem_grid)).
xx representa o _dataset_ utilizado, i.e., C1, C2 ou C3



### 4_classifica_TRL_bertimbau_neural_pi.ipynb

Esses modelos empregam o Modelos de Linguagem BERTImbau  acrescido de camadas neurais. O índice _i_ representa a rodada, onde _i_ &#x2208; {1,2,3,4,5}.

Adotou-se a quantidade máxima de _tokens_ como sendo 242.






  ### 📝 Sugestões de referência para estudo envolvendo a utilização de representação vetorial densa contextualizada 📝
- https://medium.com/data-hackers/an%C3%A1lise-de-sentimentos-em-portugu%C3%AAs-utilizando-pytorch-e-python-91a232165ec0
- https://github.com/haocai1992/GPT2-News-Classifier/blob/main/colab-train/gpt2-news-classifier-colab-train.ipynb
