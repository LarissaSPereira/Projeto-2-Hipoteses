# Projeto-2-Hipoteses

## Contexto
 Num mundo onde a indústria musical é extremamente competitiva e em constante evolução, a capacidade de tomar decisões baseadas em dados tornou-se um ativo inestimável.
 Neste contexto, uma gravadora enfrenta o emocionante desafio de lançar um novo artista no cenário musical global. Felizmente, ela tem uma ferramenta poderosa em seu arsenal: um extenso conjunto de dados do Spotify com informações sobre as músicas mais ouvidas em 2023.
 
 A gravadora levantou uma série de hipóteses sobre o que faz com que uma música seja mais ouvida:

**1-** Músicas com **BPM (Batidas Por Minuto) mais altos** fazem mais sucesso em termos de número de streams no Spotify.

**2-** As músicas mais populares no ranking do Spotify também possuem um **comportamento semelhante em outras plataformas**, como a Deezer.

**3-** A presença de uma música em um **maior número de playlists** está correlacionada com um maior número de streams.

**4-** Artistas com um **maior número de músicas** no Spotify têm mais streams.

**5-** As **características da música** influenciam o sucesso em termos de número de streams no Spotify.

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

[**Para ver a ficha técnica completa do projeto clique aqui**](https://github.com/LarissaSPereira/Projeto-2-Hipoteses/blob/main/Ficha%20T%C3%A9cnica-%20Projeto%202%20(Hip%C3%B3teses).docx)

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

[**Para acessar o arquivo do Power BI clique aqui**](https://github.com/LarissaSPereira/Projeto-2-Hipoteses/blob/main/An%C3%A1lises%20e%20Dashboard%20PBI-%20Projeto%202%20(Hip%C3%B3teses).pbix)

[**Para ver os histogramas clique aqui**](https://github.com/LarissaSPereira/Projeto-2-Hipoteses/blob/main/Histogramas-%20Projeto%202%20(Hip%C3%B3teses)%20.xlsx)

- Agrupamento dos dados de acordo com variáveis ​​categóricas
- Visualização de variáveis ​​categóricas
- Aplicação de medidas de tendência central (**média e mediana**)
- Visualização da distribuição dos dados através de histograma no Google Planilhas
- Aplicação de medidas de dispersão através do desvio padrão
- Visualização do comportamento dos dados ao longo do tempo através de gráficos de linhas
- Calculo de quartis no BigQuery (criação de categorias para cada variável de característica)
- Calculo de  correlação entre variáveis no BigQuery com o comando CORR

**3- Aplicação de técnica de análise (etapa realizada no Power BI)**

[**Para acessar o arquivo do Power BI clique aqui**](https://github.com/LarissaSPereira/Projeto-2-Hipoteses/blob/main/An%C3%A1lises%20e%20Dashboard%20PBI-%20Projeto%202%20(Hip%C3%B3teses).pbix)

- Aplicação de segmentação
- Validação de hipóteses através de correlação e gráfico de dispersão

**4- Criação de dashboard (etapa realizada no Power BI)**

[**Para acessar o dashboard clique aqui**](https://github.com/LarissaSPereira/Projeto-2-Hipoteses/blob/main/An%C3%A1lises%20e%20Dashboard%20PBI-%20Projeto%202%20(Hip%C3%B3teses).pbix)

- Representação dos dados por meio de tabela resumo e scorecards
- Representação dos dados através de gráficos de barras e linhas
- Representação dos dados por meio de gráfico de dispersão
- Aplicação de opções de filtros para gerenciamento e interação (visualização por categoria e data)

  ![Números gerais](IMAGENS/Números%20gerais.png)

  ![Hipótese 1](IMAGENS/Hipótese%201.png)

  ![Hipótese 2](IMAGENS/Hipótese%202.png)

  ![Hipótese 3](IMAGENS/Hipótese%203.png)

  ![Hipótese 4](IMAGENS/Hipótese%204.png)

  ![Hipótese 5 A](IMAGENS/Hipótese%205%20A.png)

  ![Hipótese 5 B](IMAGENS/Hipótese%205%20B.png)


**5- Apresentação de resultados**

[**Para ver o vídeo de apresentação clique aqui**](https://www.loom.com/share/e5f2883626654cfd82507b3267e0d92b)

- Seleção de gráficos e informações relevantes
- Criação de uma apresentação de slides 
- Apresentação de resultados com conclusões e recomendações

## Resultado e Conclusões 
:x:**Hipótese 1: Músicas com maior número de BPM tendem a ter mais streams?**

Hipótese refutada, pois não foi identificada uma correlação forte entre essas variáveis, músicas com valor alto de BPM não necessariamente tem mais streams.

:white_check_mark:**Hipótese 2: As músicas mais populares no ranking do Spotify também possuem um comportamento semelhante em outras plataformas como Deezer?**

Foi identificada uma correlação moderada entre todas as variáveis testadas. As músicas que são populares no Spotify tendem a ter um comportamento semelhante em termos de popularidade nessas outras plataformas, mas essa associação não é tão forte.

:white_check_mark:**Hipótese 3: A presença de uma música em um maior número de playlists está correlacionada com um maior número de streams?**

Hipótese confirmada, a análise constatou que músicas presentes em muitas playlists tendem a ter um número maior de streams, tendência que pode ser resultado de uma maior exposição da música aos usuários.

:white_check_mark:**Hipótese 4: Artistas com um maior número de músicas no Spotify têm mais streams?**

Hipótese confirmada, há uma alta correlação entre as variáveis, artistas que lançam mais músicas tendem a ser mais ouvidos.

:x:**Hipótese 5: As características de uma música influenciam no sucesso em termos de número de streams no Spotify?**

Hipótese refutada, não há uma correlação significativa entre as características das músicas e sua popularidade.


## Limitações e Próximos Passos 
- A base de dados contém informações mais completas somente do Spotify, faltando informações das outras plataformas
- A amostra de dados é pequena (somente 948 músicas)
- Restrição dos dados apenas às músicas mais ouvidas em um único ano pode limitar a generalização dos resultados
- Um próximo passo interessante seria avaliar a influência de fatores externos como a popularidade da música em redes sociais e Youtube, por exemplo.

