**Dataframes**: correspondem a uma das estruturas de dados mais comuns em R por serem semelhantes a matrizes, mas com a capacidade de armazenar colunas com tipos de dados diferentes. Cada coluna de um dataframe pode ser de um tipo diferente, como numérico, caractere, lógico, fator, entre outros. Para criar um dataframe em R, você pode usar a função `data.frame()`. A sintaxe básica é a seguinte:
```R
# Criando um dataframe
df <- data.frame(
  nome = c("João", "Maria", "Pedro"),
  idade = c(25, 30, 28),
  casado = c(TRUE, FALSE, TRUE)
)
  ```

```R
# Acesso a elementos individuais
elemento_df <- df[1, 2]  # Retorna o elemento da primeira linha e segunda coluna do dataframe
elemento_tib <- tib[2, 3]  # Retorna o elemento da segunda linha e terceira coluna do tibble

# Acesso a uma coluna específica
coluna_df <- df$idade  # Retorna a coluna "idade" do dataframe
coluna_tib <- tib$casado  # Retorna a coluna "casado" do tibble
```

```R
# Adicionar uma nova coluna
df$nova_coluna <- c(1, 2, 3)  # Adiciona a coluna "nova_coluna" ao dataframe

# Remover uma coluna
df <- subset(df, select = -nome)  # Remove a coluna "nome" do dataframe

# Filtrar linhas com base em critérios
df_filtrado <- subset(df, idade > 25)  # Filtra as linhas do dataframe onde a idade é maior que 25
```