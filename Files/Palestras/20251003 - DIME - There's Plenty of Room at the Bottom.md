# Nicola Ferro - Universitá Degli Studi di Padova

## Joint Work With

- Guglielmo Faggioli
- Raffaele Perego
- Nicola Tonellotto

## Neural INformation Retrieval

### Information Retrieval: The Y

- Matching Queries to Documents
- Then retrieve results
- Usually vectores of features trying to describe a document.
- The document is evaluated offline

---

- Três espaços. O das queries, o dos documentos e o dos resultados.
- BM25 mais usado e boa baseline

### Bag-of-Words (BoW) and Traitional IR Models

- The matching is the smaller angle between the two vectors

DÚVIDA: Mas e se ele estiver com baixo ângulo mas estiver longe?

- Dot Product
- Problema: o vocabulário tá limitado aos documentos, usar termo de fora do vocabulário pode dar problema.

Dúvida: even if I use not previously seen words, wouldn't it be mapped in some way to the existing vocabulary? Like understanding which other words would be used in this context.

## Neural IR Models

- Interaction-focused models
- Representation-focused models

### Interaction-Focused Models: monoBERT/Vanilla BERT

- Uses the probability of being relevant as a score to rank
- Problema: para calcular isso, teríamos que fazer on-the-fly e isso seria online.

### Re-ranking with INteraction-Focused Models

- Solução: ranquear primeiro com BM25 e depois re-ranquear com BERT

### Representation-focused models: Single Representations

- We can store the encoding the vectores of the documents offline
- These embeddings are dense so the calculation are slower
- We could reorder the documents by categories to reuse some calculations

#### Single Representation: Intuition

- Sine similarity is slower than dot product

## DIMEs for Neural IR

- Consideramos que os embedding são pré-computados
- Há o sentimento de que o embedding maior é melhor, mas não necessariamente. Provavelmente, muitas dessas features não são tão relevantes.

### The Clustering and the Manifold Hypotheses

- CLustering Hypothesis (van Rijsbergen, 1979)
- Manifold Hypothesis (Bengio, 2013)
  - Data represented in high-dimensional space lie (approximately) near on the similar based on low-dimensional manifolds

### The Manifold Clustering Hypotheses (Us)

- É esperado que um espaço que relacione queries e documentos tem um resultado melhor do que só o dos documentos.

#### Simplifying the Search of the Manifold

- Problem 1: Manifolds are infinite and possibly "Complex"
- Solution: we limit ourselves to looking for linear subspaces

---

- Problem 2: Linear subspaces are a lot
- Solution: we assume independence between dimensions
- Simplificação, mas que considerar dependente pode trazer resultados melhores.

### Dimension IMportance Estimators (DIMEs)

- Generating a real number related to their importance.
- Usamos o número da dimensão e alguma informação extra como os top relevantes documentos e/ou as variações da Query.

### DIMEs in Practice

...

---

Depois da análise de caixa preta sobre a qualidade de cada feature do embedding. Mas ainda não tá claro como definir quais são os importantes e quais não são e nem como computá-los.

O "remover embedding" é basicamente substituir todos eles por zeros.

### Are DIME True or Just MAgic? The Random DIME

- Imagem: cada coluna é uma query, randomly sample the dimensions
  1. Contriever
     - É o que tem mais melhoria ao fazer o sampling das features.
  2. Dragons
  3. ANCE

### Are DIME True or Just Magic? The Oracle DIME

- Hadamard Product between query and documents
- In the interaction Matrix calculates the pearson correlation to the final baseline ranking

### The Oracle DIME: Performance

- 2x4 images
  - No geral todas elas, ao pegar uns 30% das features já aumenta em muito a performance.
  - Obs.: o aumento da performance não é em rapidez/velocidade, mas sim em precisão e recall por exemplo. Ou seja, efetividade.
  - That's basically reducing noise

Optimistically we could categorize queries and then map them to a masking list of each of the features are relevant. But this would solve Explainable AI

### JV: Aplicações diversas

#### ???

#### the Magnitude DIME: Performance

This perfomance upgrading could be like just like dropping the lowest ranked 20% features.

#### The active feedback of DIME

#### The active feedback of DIME: Performance

#### The Pseudo-Relevance Feedback DIME

Centroid something

#### The PRF DIME: Perfomance

Nota: para tabela de valores usar um mapa de calor para analisar os melhores valores.

#### The LLM DIME

Ask the LLM to generate a pseudo-relevant document

#### The LLM DIME: Performance

Mixed results. We don't have a very clear visualization

#### The LLM as a Judge DIME

Use LLM as a scorer.

Dúvida do Marcos: mas e como verificar a eficiência? Ainda não foi mostrado. Como não estamos removendo colunas, apenas zeroing them, não há necessariamente melhoria de eficiência. Porém, é possível que usando uma estrutura de dados dinâmica possa vir a gerar menos computações, resultando em mais eficiência.

#### Query Variants DIME

- Redução dimensional para encontrar queries variantes próximas.

"Magnitude do centroide"

Dúvida: como gerar as query variants.

### Advanced DIMEs

- Counterfactual DIMEs (CoDIMEs)
  - Existe influência em alguns viéses como sempre clicar no primeiro.
- Eclipse
  - Calcula o centroide dos documentos irrelevantes

## Summing Up

- Framework de subsample das dimensões de representações densas para IR
- Não é necessário retreinamento ou reindexação

We train LLM to maximally separate documents. But when we want to match queries it does something not wanted (unclear).

- Later work:
  - Query-Independent DIMEs: indexes that exclude dimensions, reducing storage and computational cost
  - New indexing pipelines: optimisations to bypass operations
  - how many dimensions to be dropped?
  - Going beyond linear independence

## Perguntas

- Wagner Meira: fazer meio que uma combinação linear entre dimensões.
- Por que não analisar as que são redundantes? Oversimplification and simplest way
- Marcos: Maybe removing the top features it also remove core concepts of the documents itself.
- Marcos: its still missing semantic meaning
