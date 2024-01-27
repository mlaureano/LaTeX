# LaTeX

```{r setup, include=FALSE}
opts_chunk$set(echo = FALSE,
               comment = NA,
               results = "asis",
               error = FALSE,
               warning = FALSE,
               message = FALSE)
a <- "```tex"
b <- "```"
```
```{r, include=FALSE}
file.remove("child.Rmd")
tmp <- readLines("template.Rmd")

pdf <- sub(x = list.files(path = "./", pattern = "*.pdf"),
           pattern = "\\.pdf$",
           replacement = "")

```

teste de texto

```{r, child = "child.Rmd"}
```
