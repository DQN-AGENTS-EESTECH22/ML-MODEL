# Histograma 

O histograma é dos valores de hue da imagem

Os pontos são os valores de hue dos centros do k-means 

Assim podemos tentar perceber como o k-means tenta extrair (agrupar) as cores presentes na imagem

Também notamos que se a cor é pouco densa, apesar de poder ser considerada central para humanos, o k-means tende a ignorá-la

# K-means: avaliação

Usamos o regressor Lasso como avaliador para o desempenho do k-means na geração de paletes

O k-means teve desempenho segundo o Lasso:

Mean:  6.006428585840394
Standard deviation:  0.06439543644108417
Median:  6.0072620111283745


