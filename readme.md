# Modelos de Linguagem Neurais: fundamentos, tendências e aplicações

Materiais utilizados e desenvolvidos durante o curso de capacitação em Modelos de Linguagens Neurais, fornecido pelo projeto Tomorrow, uma parceria do instituto de computação da Universidade Federal da Bahia (UFBA) e a Positivo. Curso ministrado pela professora [Aline Paes](http://lattes.cnpq.br/0506389215528790).

## Objetivos do Curso
Capacitar os alunos a compreender, desenvolver e aplicar modelos de linguagem baseados em redes neurais, proporcionando uma base em conceitos fundamentais, técnicas de modelagem, treinamento e avaliação, além de explorar aplicações práticas em processamento de linguagem natural (PLN) e inteligência artificial. O curso visa preparar os alunos para utilizar essas tecnologias de maneira eficaz em diversos contextos, desde pesquisa acadêmica até soluções industriais.

## Objetivos Específicos
- Compreender os fundamentos teóricos: ensinar os princípios subjacentes às redes neurais e como elas são aplicadas para o aprendizado de representações de palavras e textos, incluindo conceitos como embeddings, redes neurais recorrentes (RNNs), transformers, entre outros. 

- Desenvolver habilidades práticas: Capacitar os alunos a treinar e ajustar modelos de linguagem utilizando ferramentas e frameworks populares como Hugging Face. 

- Explorar técnicas avançadas: Introduzir os alunos às técnicas avançadas em modelos de linguagem, como pré-treinamento e fine-tuning de modelos como BERT. Explorar modelos de linguagem de larga escala como llama e GPT, bem como seus agentes de conversação e técnicas de prompt e RAG. Apresentar brevemente modelos de linguagem utilizados para vocabulários não textuais. 

- Avaliar modelos de linguagem: Ensinar métodos de avaliação de desempenho de modelos de linguagem, incluindo métricas de qualidade, eficiência computacional e ética em IA. 

- Aplicar em contextos reais: Incentivar os alunos a aplicar os modelos de linguagem em problemas reais, como tradução automática, análise de sentimentos, geração de texto, e outras tarefas de processamento de linguagem natural. 

- Desenvolver pensamento crítico sobre IA: Estimular a reflexão crítica sobre as implicações sociais, éticas e técnicas do uso de modelos de linguagem neurais, incluindo questões de viés, privacidade e impacto no mercado de trabalho.

## Trabalhos
Para a conclusão do curso, foram propostos dois trabalhos, sendo eles (com suas respectivas especificações):

### Manipulação de vetores de palavras;
A partir do código disponibilizado em 2-word-embeddings.ipynb:
* Fazer uma cópia do notebook para o seu drive.
* Plotar as palavras usando o modelo pre-treinado (esse: model = KeyedVectors.load_word2vec_format(hf_hub_download(repo_id="Word2vec/wikipedia2vec_ptwiki_20180420_100d", filename="ptwiki_20180420_100d.txt"))
), ao invés do modelo que treinamos (no livro do Machado de Assis, que chamamos de our_model). Enviar apenas o plot do gráfico com vetores em 2D na tarefa.
* Gerar embeddings de frases. Escolher 10 frases do livro e fazer o plot das frases. Enviar o plot com os vetores em 2D.

Considerando o conjunto de dados utilizado em 2-sentiment.ipynb,
* Fazer uma cópia do notebook para o seu drive.
* Aproveitar o código de 2-word-embeddings.ipynb que for necessário.
* Plotar as palavras após tokenização usando o modelo pre-treinado utilizado no notebook 2-word-embeddings.ipynb, ao invés do modelo que treinamos,  e usando o modelo que treinamento em 2-sentiment. Enviar o plot de ambos como imagem na tarefa.

### Comparando as representações de emojis isoladamente entre dois modelos
Nesta tarefa, você deve comparar as representações extraídas dos embeddings do modelo BERTweet.BR (treinado com tweets em português) e dos embeddings do modelo BERTimbau.
A extração completa para o BERTweet.BR está pronta no Notebook. Você deve reproduzir o código nos locais indicados para o BERTimbau.

Ao final, você deve escolher 3 representações que os modelos concordaram e dizer se concorda ou não; e escolher 3 que os modelos discordaram e dizer com quem você concorda mais. Você não precisa postar o notebook, mas pode apenas colocar essas 6 saídas da função que retorna os mais similares, juntamente com a sua avaliação.