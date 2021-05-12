---
title: "New MD"
author: "Taylor Demetriou"
date: "5/12/2021"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

# Echo shows results, include shows the code, this links analysis.R
```{r, include=FALSE} 
library("knitr")
source("analysis.R")
```

## This is a demo of R Markdown to show what we can do

According to the Hofstede dataset, the country with the highest individualism was `r max_country2`. The country with the highest collectivism was `r min_country2`.

### Summary of individualism values: (kable will display results better, need to run library ("knitr"))
```{r, echo=FALSE}
kable(idv_summary2_df)
```

### Table of countries sorted by individualism scores
```{r, echo=FALSE}
kable(idv_data_df)
```
