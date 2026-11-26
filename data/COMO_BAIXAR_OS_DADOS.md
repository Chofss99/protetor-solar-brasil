# Como baixar os dados

Todos os arquivos ficam nesta pasta (`data/`), com estes nomes exatos.

## 1. Levantamento de preços → `coleta_protetores.xlsx`

O arquivo `coleta_protetores.xlsx` já está nesta pasta, com os 40 produtos coletados em 24 e 25/11/2026. Se você corrigir algo na planilha online, baixe de novo e substitua:

1. A planilha de coleta (aba **Coleta**) segue as regras da aba **Como preencher**: preço cheio = "De" da Drogaria São Paulo; ativos pela lista de ingredientes do site oficial da marca (use Ctrl+F com os nomes em inglês indicados na aba).
2. Na página da planilha, baixe como **.xlsx**.
3. Renomeie para `coleta_protetores.xlsx` e coloque nesta pasta.

## 2. Google Trends: ao longo do tempo → `trends_tempo.csv`

1. Acesse trends.google.com.br e clique em **Explorar**.
2. Digite `protetor solar facial`. Depois clique em **+ Comparar** e adicione `protetor solar pele oleosa`.
3. Ajuste os filtros: **Brasil**, **Últimos 5 anos**, **Todas as categorias**, **Pesquisa na Web**.
4. No quadro **Interesse ao longo do tempo**, clique no ícone de download (seta para baixo) e escolha CSV.
5. Renomeie para `trends_tempo.csv` e coloque nesta pasta.

## 3. Google Trends: por estado → `trends_estados.csv`

1. Faça uma pesquisa nova com **só** `protetor solar facial`. Com mais de um termo, o arquivo por estado sai em outro formato.
2. Filtros: **Brasil**, **Últimos 12 meses**, **Todas as categorias**, **Pesquisa na Web**.
3. No quadro **Interesse por sub-região**, confira se está em **Sub-região** (estados), clique no ícone de download e escolha CSV.
4. Renomeie para `trends_estados.csv` e coloque nesta pasta.

Anote no README a data em que baixou: o Google Trends recalcula o índice a cada consulta.

## 4. IPCA (IBGE)

Não precisa fazer nada. Na primeira vez que o notebook rodar, ele baixa os dados da API do SIDRA e salva `ipca_tabela_1419.csv` e `ipca_tabela_7060.csv` nesta pasta. Para atualizar, apague esses dois arquivos e rode de novo.
