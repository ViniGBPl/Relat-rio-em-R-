# Análise Temporal da Taxa de Desemprego na Califórnia (1976–2025)

**Autor:** Vinícius Lima\
**Data:** `20/06/2025`

## Descrição

Este repositório contém um relatório interativo em R Markdown que analisa a evolução da taxa de desemprego na Califórnia de janeiro de 1976 a fevereiro de 2025. Utilizando dados oficiais do programa Local Area Unemployment Statistics (LAUS) do Bureau of Labor Statistics e do portal data.ca.gov, o projeto explora padrões sazonais, choques econômicos, variações regionais e métricas de emprego ao longo do tempo.

##Relatório Online
Confira o relatório interativo publicado no RPubs: https://rpubs.com/vinigb/1321095

## Conteúdo

- `analise_desemprego_california.Rmd` — Código-fonte em R Markdown que gera o relatório HTML.
- `laborforceandunemployment_monthly.csv` — Conjunto de dados brutos (LAUS) usado na análise.
- `README.md` — Este arquivo de documentação.

## Pré-requisitos

- R (>= 4.0)
- Pacotes R:
  - `readr`
  - `dplyr`
  - `ggplot2`
  - `lubridate`
  - `tidyr`
  - `DT`
  - `plotly`
  - `knitr`
  - `htmltools`

> **Instalação dos pacotes em R:**
>
> ```r
> pacotes <- c("readr","dplyr","ggplot2","lubridate","tidyr","DT","plotly","knitr","htmltools")
> instalados <- pacotes[!pacotes %in% installed.packages()[,"Package"]]
> if(length(instalados)) install.packages(instalados)
> ```
##Relatório Online
Confira o relatório interativo publicado no RPubs: https://rpubs.com/vinigb/1321095
## Como Executar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   cd nome-do-repositorio
   ```
2. Certifique-se de que o arquivo `laborforceandunemployment_monthly.csv` está na raiz do projeto.
3. Abra o arquivo `analise_desemprego_california.Rmd` no RStudio.
4. Rode todos os chunks ou clique em **Knit** para gerar o relatório em HTML.

## Estrutura do Relatório

1. **Introdução**: Contextualização, objetivo e metodologia.
2. **Pacotes Requeridos**: Lista e descrição dos pacotes R.
3. **Preparação dos Dados**: Importação, limpeza e transformação.
4. **Análise Exploratória**:
   - Variação sazonal da taxa de desemprego.
   - Evolução de empregados e desempregados na Califórnia.
   - Comparação entre anos críticos (2019, 2020, 2021, 2024).
   - Análise geográfica por condados.
   - Métrica da Taxa de Emprego.
5. **Conclusão**: Principais insights, limitações e caminhos futuros.
6. **Referências**: Fontes e bibliografia.

## Fonte de Dados

- **LAUS (Local Area Unemployment Statistics)** — Bureau of Labor Statistics: [https://www.bls.gov/lau/](https://www.bls.gov/lau/)
- **Labor Force and Unemployment Data** — California Open Data Portal: [https://data.ca.gov/dataset/local-area-unemployment-statistics-laus](https://data.ca.gov/dataset/local-area-unemployment-statistics-laus)

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

