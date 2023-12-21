# 🤖 Modelos 🤖

## Dataset
De forma geral, utilizou-se 2 possíveis **datasets**: C'<sub>a</sub> [mencionado agora como c1 (dataset.csv)\*], C'<sub>b</sub>[mencionado agora como c3(dataset_pre_processado_stem_2.csv)\*] com níveis crescentes de pré-processamento. Esses _datasets_ foram particionados utilizando-se a técnica um k-fold com k=5.


*_Essa alteração de representação ocorreu para fins de simplificação e compatibilidade de caracteres._


<pre> Deve se ter especial cuidado para não confundir c1, c2 e c3 com C'<sub>1</sub>, C'<sub>2</sub> e C'<sub>3</sub>. 
Os três primeiros se referem a corpus, enquanto os três últimos a partições do k-fold</pre>

## Técnicas de representação vetorial

|	  **Técnica/modelo** | **Biblioteca**  | **Especificação** |
| ------------- | ------------- | ------------- |
| Count Vectorizer | Scikit-learn    | *CountVectorizer*  |
| TF-IDF | Scikit-learn    | *TfidfVectorizer*  |
|BERT  | Hugging Face    | *BERT-base-multilingual-cased*  |
| BERTimbau    | Hugging Face  | *neuralmind/bert-base-portuguese-cased*   |
| GPT-2  | Hugging Face    | *pierreguillou/gpt2-small-portuguese* |


## Algoritmos de Machine Learning 

| **Algoritmo** | **Sigla** | **Biblioteca** | 
| ------------- | ------------- | ------------- |
|Multinomial Naive Bayes |  MNB| Scikit-learn | 
|Complement Naive Bayes Classifier |  CNB | Scikit-learn | 
|K-Nearest Neighbors |  KNN |Scikit-learn | 
|Support Vector Machine |  SVM | Scikit-learn | 
|Random Forest |  RF| Scikit-learn | 
|AdaBoost |  Adb | Scikit-learn | 
|Rede Neural Artificial |  RNA| Scikit-learn/PyTorch| 




## Dos cadernos:
_Obs.:_ As MLP são também um tipo de algoritmo de Machine Learning, mais especificamente um tipo de RNA profunda. Nas descrições a seguir separamos os cadernos com experimento com elas (e/ou adição de camadas aos modleos de linguagem) dos com outros algoritmos de ML.

### 1_countvectorizer_resumo_c3_sem_grid
Esses modelos empregaram a representação vetorial Count Vectorizer combinada com algoritmos de ML (que não RNA), não se utilizou um método de otimização de parâmetros (sem_grid)).

### 1_countvectorizer_mlp_resumo_c3_sem_grid
Esses modelos empregaram a representação vetorial Count Vectorizer combinada com uma MLP, não se utilizou um método de otimização de parâmetros (sem_grid)).


### 2_tf_idf_resumo_c3_sem_grid
Esses modelos empregaram a representação vetorial TF-IDF combinada com algoritmos de ML (que não RNA), não se utilizou um método de otimização de parâmetros (sem_grid)).


### 2_tf_idf_mlp_resumo_c3_sem_grid
Esses modelos empregaram a representação vetorial TF-IDF combinada com uma MLP (que não RNA), não se utilizou um método de otimização de parâmetros (sem_grid)).

### 3_classifica_TRL_bertimbau_neural_pi
Esses modelos empregam o Modelo de Linguagem BERTimbau  acrescido de camadas neurais. O índice _i_ representa a rodada, onde _i_ &#x2208; {1,2,3,4,5}.

Adotou-se a quantidade máxima de _tokens_ como sendo 242.

### 3_classifica_TRL_bertimbau_mod_ML
Esses modelos empregam o Modelo de Linguagem BERTimbau para gerar-se a representação vetorial dos textos, _i.e._, resumos. Essa representação vetorial é apresentada aos algoritmos de ML (que não RNA).

Adotou-se a quantidade máxima de _tokens_ como sendo 242.

### 4_classifica_TRL_bertimbau_neural_512_pi
Esses modelos empregam o Modelo de Linguagem BERTimbau  acrescido de camadas neurais. O índice _i_ representa a rodada, onde _i_ &#x2208; {1,2,3,4,5}.

Adotou-se a quantidade máxima de _tokens_ como sendo 512.

### 4_classifica_TRL_bertimbau_mod_ML_512
Esses modelos empregam o Modelo de Linguagem BERTimbau para gerar-se a representação vetorial dos textos, _i.e._, resumos. Essa representação vetorial é apresentada aos algoritmos de ML (que não RNA).

Adotou-se a quantidade máxima de _tokens_ como sendo 512.

### 5_classifica_TRL_bert_neural_pi

Esses modelos empregam o Modelo de Linguagem BERT (multi) acrescido de camadas neurais. O índice _i_ representa a rodada, onde _i_ &#x2208; {1,2,3,4,5}.

Adotou-se a quantidade máxima de _tokens_ como sendo 242.

### 5_classifica_TRL_bert_mod_ML

Esses modelos empregam o Modelo de Linguagem BERT (multi) para gerar-se a representação vetorial dos textos, _i.e._, resumos. Essa representação vetorial é apresentada aos algoritmos de ML (que não RNA).

Adotou-se a quantidade máxima de _tokens_ como sendo 242.

### 6_classifica_TRL_bert_neural_512_pi

Esses modelos empregam o Modelo de Linguagem BERT (multi) acrescido de camadas neurais. O índice _i_ representa a rodada, onde _i_ &#x2208; {1,2,3,4,5}.

Adotou-se a quantidade máxima de _tokens_ como sendo 512.

### 6_classifica_TRL_bert_mod_ML_512

Esses modelos empregam o Modelo de Linguagem BERT (multi) para gerar-se a representação vetorial dos textos, _i.e._, resumos. Essa representação vetorial é apresentada aos algoritmos de ML (que não RNA).

Adotou-se a quantidade máxima de _tokens_ como sendo 512.

### 7_classifica_TRL_gpt2_neural_pi

Esses modelos empregam o Modelos de Linguagem GPT-2, treinado para o português, em sua variação voltada para a língua portuguesa,  acrescido de camadas neurais. O índice _i_ representa a rodada, onde _i_ &#x2208; {1,2,3,4,5}.

Adotou-se a quantidade máxima de _tokens_ como sendo 242.

### 7_classifica_TRL_gpt2_mod_ML

Esses modelos empregam o Modelo de Linguagem GPT-2, treinado para o português, para gerar-se a representação vetorial dos textos, _i.e._, resumos. Essa representação vetorial é apresentada aos algoritmos de ML (que não RNA).

Adotou-se a quantidade máxima de _tokens_ como sendo 242.

### 8_classifica_TRL_gpt2_neural_512_pi

Esses modelos empregam o Modelos de Linguagem GPT-2, treinado para o português, em sua variação voltada para a língua portuguesa,  acrescido de camadas neurais. O índice _i_ representa a rodada, onde _i_ &#x2208; {1,2,3,4,5}.

Adotou-se a quantidade máxima de _tokens_ como sendo 512.

### 8_classifica_TRL_gpt2_512_mod_ML

Esses modelos empregam o Modelo de Linguagem GPT-2, treinado para o português, para gerar-se a representação vetorial dos textos, _i.e._, resumos. Essa representação vetorial é apresentada aos algoritmos de ML (que não RNA).

Adotou-se a quantidade máxima de _tokens_ como sendo 512.









  ### 📝 Sugestões de referência para estudo envolvendo a utilização de representação vetorial densa contextualizada 📝
- https://medium.com/data-hackers/an%C3%A1lise-de-sentimentos-em-portugu%C3%AAs-utilizando-pytorch-e-python-91a232165ec0
- https://github.com/haocai1992/GPT2-News-Classifier/blob/main/colab-train/gpt2-news-classifier-colab-train.ipynb
