**Tibbles:**

Os tibbles são uma versão moderna e aprimorada dos dataframes em R, introduzidos pelo pacote `tibble`. Os tibbles têm muitas características semelhantes aos dataframes, mas com algumas diferenças sutis. Os tibbles são projetados para serem mais intuitivos e amigáveis, fornecendo uma experiência de programação mais consistente. Para criar um tibble em R, você pode usar a função `tibble()`, disponível no pacote `tibble`. A sintaxe básica é a seguinte:

```R
# Criando um tibble
library(tibble)

tib <- tibble(
  nome = c("João", "Maria", "Pedro"),
  idade = c(25, 30, 28),
  casado = c(TRUE, FALSE, TRUE)
)
  ```
  
  ```R
# Adicionar uma nova coluna
tib$nova_coluna <- c(1, 2, 3)  # Adiciona a coluna "nova_coluna" ao tibble

# Remover uma coluna
tib <- tib[, -2]  # Remove a segunda coluna do tibble

# Filtrar linhas com base em critérios
tib_filtrado <- filter(tib, idade > 25)  # Filtra as linhas do tibble onde a idade é maior que 25
```