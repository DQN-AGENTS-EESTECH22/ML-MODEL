# DNQ Agents

- Cauã
- Guilherme
- Felipe

# Proposta

- Gerar paletas de cores para design de websites

    - Extração de paleta de imagens

    - Construir paleta a partir de palavras-chave

    - Emprego automático e funcional da paleta no layout do website

# Fase exploratória

- Sandbox próprio com 3 ambientes distintos

- Gerada a paleta, como aplicar da maneira mais eficiente ao website?

    - Como utilizar o contraste entre cores para ter um website funcional?

    - Como quantificar a qualidade da paleta?

    - Como escolher uma paleta que corresponde ao gosto do usuário?

# Datasets

- "Color Compatibility From Large Datasets, Peter O'Donovan"

- Avaliações dos usuários do site https://www.colourlovers.com/ para as paletas lá disponibilizadas

- Algoritmo de regressão para avaliar o quão agradável uma paleta é

# Regressão

- Dada uma paleta, retornar um *score*

- Algoritmo Lasso

- *Feature engineering*
    - Diferentes espaços de cor: RGB, HSV
    - Cor média, desvio padrão
    - Pontuações normalizadas
    - Etc.

# K-Means Clustering

- Dada uma imagem, agrupar 5 principais cores -> Paleta

- Avaliar desempenho com o regressor

# K-Means Clustering

![china](.\kmeans_presentation\china\china.png)
![china_palette](.\kmeans_presentation\china\palette.png)

# K-Means Clustering

![china_dv](.\kmeans_presentation\china\histogram.png)

# K-Means Clustering

![flower](.\kmeans_presentation\flower\flower.png)
![flower_palette](.\kmeans_presentation\flower\palette.png)

# K-Means Clustering

![flower_dv](.\kmeans_presentation\flower\histogram.png)

# K-Means Clustering

## Avaliado num *dataset* de posters de filmes

![reg_eval](.\kmeans_presentation\evaluation\lasso_eval.png)


# K-Means Clustering

Escala 0-10

$$
\textrm{score} = 6.0 \pm 0.1
$$

Grande margem para aperfeiçoar (regressão & K-Means)

# Gerar paleta a partir de palavras

