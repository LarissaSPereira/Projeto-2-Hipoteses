# Projeto-2-Hipoteses

## Contexto
 Num mundo onde a indústria musical é extremamente competitiva e em constante evolução, a capacidade de tomar decisões baseadas em dados tornou-se um ativo inestimável.
 Neste contexto, uma gravadora enfrenta o emocionante desafio de lançar um novo artista no cenário musical global. Felizmente, ela tem uma ferramenta poderosa em seu arsenal: um extenso conjunto de dados do Spotify com informações sobre as músicas mais ouvidas em 2023.
 
 A gravadora levantou uma série de hipóteses sobre o que faz com que uma música seja mais ouvida:

- Músicas com **BPM (Batidas Por Minuto) mais altos** fazem mais sucesso em termos de número de streams no Spotify.

- As músicas mais populares no ranking do Spotify também possuem um **comportamento semelhante em outras plataformas**, como a Deezer.

- A presença de uma música em um **maior número de playlists** está correlacionada com um maior número de streams.

- Artistas com um **maior número de músicas** no Spotify têm mais streams.

- As **características da música** influenciam o sucesso em termos de número de streams no Spotify.

## Objetivo
Validar (refutar ou confirmar) essas hipóteses através da análise de dados e fornecer recomendações estratégicas com base nas descobertas feitas. O objetivo principal desta análise é que a gravadora e o novo artista possam tomar decisões informadas que aumentem suas chances de alcançar o sucesso.

## Equipe 
Larissa Silva Pereira 

## Ferramentas e Tecnologias 
Google Big Query, Power BI, Google Planilhas, Google Slides e Loom.

## Base de Dados 
- [Tabela Track in Spotify](https://github.com/LarissaSPereira/Projeto-2-Hipoteses/blob/main/tabela_track_in_spotify.csv)
- [Tabela Track in Competition](https://github.com/LarissaSPereira/Projeto-2-Hipoteses/blob/main/tabela_track_in_competition.csv)
- [Tabela Track Tecnical Info](https://github.com/LarissaSPereira/Projeto-2-Hipoteses/blob/main/tabela_track_technical_info.csv)

## Processamento e Análises 
**1- Processamento e preparação da base de dados (etapa realizada no BigQuery)**
- Importação dos dados para o BigQuery
- Identificação e tratamento de valores nulos com os comandos COUNT, WHERE e IS NULL
- Identificação e tratamento de valores duplicados com os comandos COUNT, GROUP BY e HAVING
- Identificação e tratamento de dados fora do escopo de análise com os comandos SELECT e EXCEPT
- Identificação e tratamento de dados discrepantes em variáveis ​​categóricas com os comando LIKE e REGEXP
- Identificação e tratamento de dados discrepantes em variáveis ​​numéricas com os comandos MAX, MIN e AVG
- Verificação e alteração do tipo de dados com os comandos SAFE_CAST 
- Criação de novas variáveis com os comandos CONCAT e CAST
- União de tabelas com o comando LEFT JOIN
- Construção de tabelas auxiliares com o comando WITH

**2- Análise exploratória (etapa realizada no Power BI, Google planilhas e BigQuery)**
- Agrupamento dos dados de acordo com variáveis ​​categóricas
- Visualização de variáveis ​​categóricas
- Aplicação de medidas de tendência central (**média e mediana**)
- Visualização da distribuição dos dados através de histograma no Google Planilhas
- Aplicação de medidas de dispersão através do desvio padrão
- Visualização do comportamento dos dados ao longo do tempo através de gráficos de linhas
- Calculo de quartis no BigQuery (criação de categorias para cada variável de característica)
- Calculo de  correlação entre variáveis no BigQuery com o comando CORR

**3- Aplicação de técnica de análise (etapa realizada no Power BI)**
- Aplicação de segmentação
- Validação de hipóteses através de correlação e gráfico de dispersão

**4- Criação de dashboard (etapa realizada no Power BI)**

[**Para visualizar o dashboard completo clique aqui**]()
- Representação dos dados por meio de tabela resumo e scorecards
- Representação dos dados através de gráficos de barras e linhas
- Representação dos dados por meio de gráfico de dispersão
- Aplicação de opções de filtros para gerenciamento e interação (visualização por categoria e data)

**5- Apresentação de resultados**

[**Para ver o vídeo de apresentação clique aqui**](https://docs.google.com/presentation/d/1Viy8BMpuErmIY4jvmM1Hs-YrgVxwkBfXuqVoc1gvI0w/edit?usp=sharing
)
- Seleção de gráficos e informações relevantes
- Criação de uma apresentação de slides 
- Apresentação de resultados com conclusões e recomendações

## Resultado e Conclusões 

## Limitações e Próximos Passos 

## Links de Interesse 
