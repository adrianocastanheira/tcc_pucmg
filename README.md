# PONTIFÍCIA UNIVERSIDADE CATÓLICA DE MINAS GERAIS - NÚCLEO DE EDUCAÇÃO A DISTÂNCIA  
## Pós-graduação Lato Sensu em Ciência de Dados e Big Data  
## Trabalho de conclusão do curso - Adriano Diniz Castanheira  

## Título: CLASSIFICAÇÃO DE NCM COM BASE NA DESCRIÇÃO DE MERCADORIAS SUJEITAS A PENA DE PERDIMENTO    

### Este repositório contém uma pasta chamada TCC onde se encontra o Trabalho de Conclusão de Curso em formato .pdf.

### Este repositório contém também uma pasta chamada Códigos uma pasta para os notebooks utilizados na coleta, tratamento de dados e na aplicação do modelo de machine Learning e contém também outra pasta com a versão .pdf desses notebooks.

### Os notebooks foram divididos em notebooks de Análise (um para cada base de dados), Formata dataframes (concatena os dataframes) e Baseline Keras (roda a rede neural).

### Os notebooks de Análise possuem o seguinte conteúdo:
1 - Importa dados do csv  
2 - Analisa e processa coluna 'ncm'  
3 - Cria funções auxiliares para o processamento da coluna descrição  
4 - Analisa e processa coluna 'descricao'  
5 - Cria a coluna 'descricao_limpa'  
6 - Cria a coluna 'descricao_limpa_sem_stopwords'  
7 - Cria a coluna 'descricao_limpa_stemming'  
8 - Cria a coluna 'descricao_limpa_sem_stopwords_stemming'

### O notebook que formata os dataframes possue o seguinte conteúdo:
Trata da criação de um único dataframe com base nos dataframes dos itensTG, da TEC e do Secta
Serão criados três dataframes conforme abaixo:  
1 - Dataframe com descrição limpa (com stopwords e com afixos)  
2 - Dataframe com descrição limpa, sem stopwords (com afixos)  
3 - Dataframe com descrição limpa, sem stopwords e radicais das palavras (stemming)¶

### Os notebooks que rodam a rede neural possuem o seguinte conteúdo:
1 - Carrega informações do dataframe  
2 - Criação do encoder e da matriz binária para cada coluna que iremos usar para classificação  
3 - gera o corpus (bag of words) e vetoriza  
4 - Faz a transformação TFIDF  
5 - Cria bases de treinamento e validação  
6 - Cria modelo  
7 - Analisa a acurária e a perda de cada modelo  
8 - Cria predições para cada modelo treinado  
9 - Aplica o modelo na base completa e analisa resultados 
