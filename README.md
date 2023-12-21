# Technology Readiness Level - TRL 

📌  Trata-se de repositório para a dissertação de mestrado voltada para o problema de classificação de documentos utilizando a escala TRL.

📌  Aqui encontramos o [_corpus/dataset_](https://github.com/jlvoltan/trl/tree/main/dataset)  construído e [modelos treinados](https://github.com/jlvoltan/trl/tree/main/modelos) para essa tarefa.

✏️  Maiores explicações sobre a metodologia utilizada pode ser encontrada nos artigos e dissertação.


### 📝 Resumo do trabalho 📝

A escala TRL surgiu na década de 70, com o propósito de mensurar a maturidade tecnológica de um produto ou tecnologia. A partir dos anos 2000, ganhou destaque em diversos órgãos e empresas ao redor do mundo, tendo emprego não só no acompanhamento de projetos, como também na gestão e prospecção tecnológica. Apesar desse aumento de importância, a abordagem predominante para avaliar o nível TRL de uma tecnologia ou produto, _i.e._, a Avaliação de Prontidão Tecnológica (_Technology Readiness Assessment_ - TRA), é baseada na avaliação de especialistas. Tal abordagem tem como desvantagens o elevado custo, demora, além de um possível viés. Diante desse cenário, tem-se o problema, de como seria possível realizar uma TRA escalável, com um menor custo e maior padronização de critérios. As propostas de TRA automatizadas são poucas e apresentam espaço para aprimoramento. O estado da arte ainda é baseado na combinação de técnicas de representação vetorial esparsa e algoritmos de classificação. Essas técnicas de representação, derivadas do _Bag-of-Words_, não utilizam o contexto em que as palavras ocorrem (_e.g._ a palavra manga, parte da vestimenta, possui a mesma representação vetorial que a fruta manga), além de gerarem vetores de alta dimensionalidade com muitos valores nulos. Essas limitações podem impactar negativamente no desempenho dos algoritmos de classificação. Diante desta perspectiva, inspirado por resultados bem sucedidos em diversas aplicações de classificação textual em outras áreas, o presente trabalho levantou como hipótese que o emprego de técnicas de representação vetorial densa contextualizada (_i.e._ que considerem o contexto onde as palavras ocorrem) pode trazer melhora no desempenho de algoritmos de classificação também no escopo da TRA. Para verificar essa hipótese, foi construído um corpus voltado para o domínio da Defesa, reunindo artigos científicos e notícias escritos em língua portuguesa (PT-BR). Também foi proposta uma metodologia para aplicação da mineração de texto na TRA. Através dela, foram avaliadas as combi nações de cinco técnicas de representação vetorial (Count Vectorizer, TF-IDF, BERT, BERTimbau e GPorTuguese-2 - variação do GPT-2) e sete algoritmos de aprendizado de máquina voltados para a tarefa de classificação. Ao final, os melhores resultados foram obtidos pelo modelo de linguagem BERTimbau combinado com Redes Neurais Artificias, chegando-se a uma acurácia de 72%, superando o estado da arte. Os resultados mostraram que as representações densas contextualizadas contribuíram para uma pequena melhora de desempenho na maioria dos algoritmos avaliados.

### 💬 Breve explicação 💬

- Neste trabalho, construímos um [_corpus_](https://github.com/jlvoltan/trl/tree/main/dataset) utilizando notícias e artigos científicos. Eles se encontram na pasta [_dataset_]((https://github.com/jlvoltan/trl/tree/main/dataset));

- Na pasta [questionário](https://github.com/jlvoltan/trl/tree/main/questionario) há um arquivo que sintetiza esse _corpus_, na forma de planilha.

- Na pasta [_manipula-dataset_](https://github.com/jlvoltan/trl/tree/main/manipula-dataset), existem alguns cadernos relacionados com a análise do _corpus_, pré-processamento e divisão dos _folders_.

- Por fim, na pasta [_modelos_](https://github.com/jlvoltan/trl/tree/main/modelos), são apresentados os cadernos dos experimentos, em que se obteve a representação vetorial, através de técnicas baseadas no BoW ou através de Modelos de Linguagem, e posteriormente se treinou e testou modelos de classificação. 
