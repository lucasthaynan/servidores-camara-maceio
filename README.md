## Salários dos servidores da Câmara Municipal de Maceió
Script que raspa os dados da [página de pagamentos e subsídios](https://www.maceio.al.leg.br/transparencia/portal/salarios-subsidios) dos servidores e vereadores da Câmara Municipal de Maceió e exporta as informações para uma planilha do Google Sheets.

## Metodologia 
O programa [`web_scraping_servidores_camara_maceio.ipynb`](https://github.com/lucasthaynan/servidores-camara-maceio/blob/main/web_scraping_servidores_camara_maceio.ipynb) navega pela lista de páginas do site de transparência com as informações dos pagamentos e extrai os dados de cada um dos servidores da Câmara Municipal. 
Como exemplo, para coletar os dados de janeiro a setembro de 2021 foi necessário passar **283** como parâmetro da função `pega_links_servidores()`. Assim, serão percorridas as páginas de 1 a 283 e extraídos os todos os dados deste período.

## Bibliotecas

* **requests** 
* **re** 
* **pandas**

Necessário instalar:
* **tqdm** `pip install tqdm`- Adiciona uma barra de progresso ao executar um `for`.útil para saber a estimativa do tempo total para execução do código;
* **gspread** `pip install gspread` - Conecta com o Google Sheets, o que permite importar, atualizar e deletar dados de planilhas;
* **google.oauth2** `pip install google.auth` - Permite acessar APIs do Google.

## Obter credenciais de API Google

Siga as etapas [deste tutorial](https://medium.com/pyladiesbh/gspread-trabalhando-com-o-google-sheets-f12e53ed1346) (ou [deste outro](https://www.youtube.com/watch?v=ddf5Z0aQPzY&t=17)) para autorização de acesso à API do Google Sheets. Esta etapa é necessária para a biblioteca `gspread` funcionar.

## Sobre
Trabalho final do Master em Jornalismo de Dados, Automação e Data Storytelling, do Insper das disciplinas:
* **Pensamento Computacional** - elaboração do programa -, professor Álvaro Justen (Turicas);
* **Transparência, reprodutibilidade e uso éticos dos dados** - documentação do projeto, professoras Natália Mazotte e Carla Vieira.

