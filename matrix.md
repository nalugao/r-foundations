```R
nome_matriz <- matrix(data, nrow, ncol)
```

```R
matriz_numerica <- matrix(c(1, 2, 3, 4, 5, 6, 7, 8, 9), nrow = 3, ncol = 3)
```

```R
matriz_vazia <- matrix(nrow = 2, ncol = 2)
```
```R
matriz <- matrix(c(1, 2, 3, 4, 5, 6), nrow = 2, ncol = 3)

# Acesso a elementos individuais
elemento <- matriz[1, 2]  # Retorna o elemento na primeira linha e segunda coluna

# Acesso a uma linha específica
linha <- matriz[2, ]  # Retorna a segunda linha inteira como um vetor

# Acesso a uma coluna específica
coluna <- matriz[, 3]  # Retorna a terceira coluna inteira como um vetor
```

```R
matriz1 <- matrix(c(1, 2, 3, 4), nrow = 2, ncol = 2)
matriz2 <- matrix(c(5, 6, 7, 8), nrow = 2, ncol = 2)

# Soma de matrizes
soma <- matriz1 + matriz2

# Multiplicação de matrizes
multiplicacao <- matriz1 %*% matriz2

# Transposição de uma matriz
transposta <- t(matriz1)
```

```R
matriz <- matrix(c(1, 2, 3, 4, 5, 6), nrow = 2, ncol = 3)

# Comprimento de uma dimensão da matriz
comprimento_linhas <- nrow(matriz)
comprimento_colunas <- ncol(matriz)

# Valor mínimo e máximo da matriz
minimo <- min(matriz)
maximo <- max(matriz)

# Soma de elementos da matriz
soma <- sum(matriz)
```

```R
matriz <- matrix(c(1, 2, 3, 4), nrow = 2, ncol = 2)

# Adicionar uma nova linha à matriz
nova_linha <- c(5, 6)
matriz <- rbind(matriz, nova_linha)

# Adicionar uma nova coluna à matriz
nova_coluna <- c(7, 8)
matriz <- cbind(matriz, nova_coluna)

# Remover uma linha da matriz
matriz <- matriz[-2, ]

# Remover uma coluna da matriz
matriz <- matriz[, -3]
```