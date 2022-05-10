# Web Crawler para extração de dados da pagina [ComprasNet](https://www.gov.br/compras/pt-br/acesso-a-informacao/noticias)

- Clone o projeto

  ```
  git clone https://github.com/herlandio/forseti-code-challenge
  ```
  
- Acesse a pasta forseti-code-challenge/ e Instale as dependências utilizando o comando abaixo

  ```
  composer install
  ```
  
- No arquivo forseti-code-challenge/src/crawler.php basta definir de quantas paginas serão extraidas as informações

  ```
  $WebCrawler = new WebCrawler();
  $WebCrawler->saveExcel($WebCrawler->getPages(5));
  ```
  
- Para executar o script acesse a pasta forseti-code-challenge/ e execute no terminal

  ```
  php src/crawler.php
  ```
  
- Após a execução do script ira gerar uma planilha excel com todas as informações exportadas 

  - A planilha estará na pasta forseti-code-challenge/

- Para testes acesse a pasta forseti-code-challenge/ e execute

  ```
  ./vendor/bin/phpunit tests
  ```
  
- OBS: a extenção extension=gd2 ou extension=gd deve estar habilitada no php.ini.
