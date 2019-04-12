# miningAbandonment

Projeto da disciplina de mineração de dados. 
Análise do abandono de disciplina por alunos da Ciência da Computação

## Tema do projeto

Este projeto tem como objetivo avançar as capacidades analíticas e facilitar a gestão da Universidade Federal do ABC sobre o abandono de disciplinas pelos alunos de graduação do Bacharelado em Ciência da Computação. Este tema além de ter impacto sobre o tempo de formação do discente e planejamento de demanda por cursos, prejudica a eficiência operacional da organização.

Ao final do projeto, a expectativa do grupo é entregar:

* Análise exploratória dos dados com diagnóstico do problema tema do trabalho. 
* Pelo menos um modelo campeão e um desafiante, comparando a performance de ambos na resolução do desafio. 
* Os resultados e a interpretação do modelo campeão. 
* Sugestões de próximos passos para modelagem do problema, incluindo possivelmente ideias de associação com outros dados.

### Procedimentos de Análise de Dados

Iniciamos efetuando uma análise exploratória para identificação das relações, conhecimentos latentes, proporções e estrutura dos dados. Não há técnicas estabelecidas nessa etapa. Nessa fase não inferencial, buscamos através da visualização levantar hipóteses sobre os dados e durante o desenvolvimento aprofundar os indícios-relações encontrados.

Seguindo, iremos incrementar os atributos com dados de outros conjuntos de dados. Da listagem de disciplinas do curso iremos verificar qual o seu vínculo nos projetos pedagógicos, além disso, propomos a criação de atributos derivados. Um exemplo de atributo pode ser o coeficiente de afinidade do aluno e sua turma, considerando como afins alunos que cursaram até o momento do curso mais disciplinas em comum.
Posteriormente faremos ajuste de pelo menos dois modelos de classificadores para prever a ocorrência de conceitos O. Um primeiro forte candidato é Random Forest, pela adaptabilidade a cenários particulares dentro do contexto do problema. Outro que poderá ser avaliado é Bayes pela natureza do problema (probabilidade de abandono dado um contexto do aluno). Poderá ser necessário utilizar aumentação de Dados para melhora da performance em validação.

### Descrição da fonte de dados

O conjunto de dados contém os históricos dos alunos matriculados no curso de Ciência da Computação da Universidade Federal do ABC. Os dados preservam anonimidade e foram obtidos através da lei de acesso à informação. Inteiramos que dado a natureza da solicitação esses dados são livres para qualquer cidadão. Os atributos da base são ID_ALUNO, ANO, QUADRIMESTRE, NOME_DISCIPLINA, COD_DISCIPLINA e o CONCEITO. O recorte temporal é do final do ano de 2017, ou seja, até o terceiro quadrimestre. A primeira disciplina por aluno varia, dado a heterogeneidade na formação dos alunos, o início do histórico abrange de 2006 a 2016.