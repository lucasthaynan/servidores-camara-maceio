## Salários dos servidores da Câmara Municipal de Maceió
Script que raspa os dados da [página de pagamentos e subsídios](https://www.maceio.al.leg.br/transparencia/portal/salarios-subsidios) dos servidores e vereadores da Câmara Municipal de Maceió e exporta as informações para uma planilha do Google Sheets.

## Metodologia 
O programa navega pela lista com todos os pagamentos dos servidores e vereadores e coleta as informações de cada um. É possível definir como parâmetro a quantidade de páginas que o scrip vai rodar.

## Bibliotecas

* **requests** 
* **re** 
* **pandas**

Necessário instalar:
* **tqdm** `pip install tqdm`- Adiciona uma barra de progresso ao executar um for
* **gspread** `pip install gspread` - Conecta com planilhas do Google Sheets
* **google.oauth2** `pip install google.auth` - Permite acessar APIs do Google

