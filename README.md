# A Caracterização de Mulheres na Música Brasileira: Identificando Padrões com Processamento de Linguagem Natural

## Descrição

Este trabalho explora a caracterização de mulheres nas músicas brasileiras, identificando padrões linguísticos, especialmente aqueles que revelam elementos de sexualização e sexismo. Utilizamos técnicas de Processamento de Linguagem Natural (PLN) para responder às seguintes perguntas de pesquisa:

### Perguntas de Pesquisa
1. Como é a distribuição dos adjetivos utilizados para caracterizar as mulheres?
2. Os adjetivos empregados para caracterizar mulheres são utilizados de forma positiva ou negativa?
3. Quais são as ocupações mais citadas para cada gênero?
4. Os estereótipos de gênero mudam de acordo com o estilo musical?
5. Qual proporção das músicas analisadas apresenta sexismo?

Após a seleção do corpus, seguimos um fluxo metodológico estruturado, com cada etapa voltada para uma análise específica. O diagrama ilustrado na *Figura* apresenta o fluxo de etapas seguido.

![mapa1](https://github.com/user-attachments/assets/78fd5b5e-1c67-4226-b607-97aa051377d4)

## Estrutura de Pastas

### 1. Corpus
Você pode fazer o download de todos os corpus utilizados, incluindo o corpus unificado com um total de **146.612 músicas**.

[Link Google Drive](https://drive.google.com/drive/folders/1BdBsE5gqEVaQ7ANuiuOilYMmjX320Okv?usp=sharing)

### 2. Pasta Análise de Frases Predicativas
- **analise-frases-predicativas.ipynb**: Código para capturar frases predicativas usando expressões regulares.
- **Resultados**: [Subpasta com os resultados das análises.](https://drive.google.com/drive/folders/1z9uPvH2deVN4XYr1UUd300cnhiqM522b?usp=sharing)

### 3. Pasta Profissões
Contém códigos para a análise de profissões e resultados com listas de profissões específicas, incluindo o ranking.

#### Arquivos e Pastas
- **Códigos**:
  - `Feminino Árvore de Dependência.ipynb`: Análise de dependência de profissões no gênero feminino.
  - `Feminino Expressão Regular.ipynb`: Análise de profissões no gênero feminino usando expressões regulares.
  - `Masculino Árvore de Dependência.ipynb`: Análise de dependência de profissões no gênero masculino.
  - `Masculino Expressão Regular.ipynb`: Análise de profissões no gênero masculino usando expressões regulares.
  - `ranking_Buscando_profissões`: Script para gerar ranking de profissões com base nos critérios do projeto.

- **Lista de Profissões**:
  - `profissoes_casos_especiais.txt`: Lista de profissões que requerem análise diferenciada.
  - `profissoes_fem.txt`: Lista de profissões no gênero feminino.
  - `profissoes_masc.txt`: Lista de profissões no gênero masculino.

- **Resultados**:
  - `resultados_rank_fem.csv`: Ranking de profissões no feminino.
  - `resultados_rank_masc.csv`: Ranking de profissões no masculino.

### 4. Pasta Agrupamento
Contém a análise de 1.000 predicativos femininos e masculinos categorizados.
- `categ_adjetivo_fem.csv`: CSV com os predicativos femininos categorizados.
- `categ_adjetivo_masc.csv`: CSV com os predicativos masculinos categorizados.
- `agrupamento_dados.ipynb`: Notebook para gerar gráficos com base nos dados de predicativos.

### 5. Pasta Anotação Sentenças
Contém 1.999 sentenças anotadas manualmente quanto ao sentimento, classificadas como positivo, negativo ou neutro para os gêneros feminino e masculino.
- `Positivo_Feminino.csv`, `Negativo_Feminino.csv`, `Neutro_Feminino.csv`
- `Positivo_Masculino.csv`, `Negativo_Masculino.csv`, `Neutro_Masculino.csv`

### 6. Pasta Modelo de Classificação de Sentimentos
- **Resultados**: [Subpasta com resultados](https://drive.google.com/drive/folders/1p57lDAngnc0piW9rs3OTJuIUkYMqZDCI?usp=sharing) das sentenças anotadas em termos de sentimento (positivo, neutro ou negativo).
- **Dados de Treinamento**: [Subpasta com o subcorpus anotado manualmente.](https://drive.google.com/drive/folders/1VFOnKBQlXfCtykBJqX7txTnaTu7-UNy3?usp=sharing)
- **bertimbau-analise.ipynb**: Código para o fine-tuning do modelo BERTimbau, aplicando-o na análise de sentimento em frases predicativas.
