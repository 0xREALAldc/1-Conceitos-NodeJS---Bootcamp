# 1 Conceitos NodeJS - Bootcamp
Neste projeto foi desenvolvido os conceitos básicos de um projeto em NodeJS. 

Foram desenvolvidas funcionalidades onde foi compreendido como se inicia um projeto backend utilizando o micro framework 
**expres**, quais são os métodos HTTP possíveis de serem utilizados nas rotas e quais as funções de cada um. 

Também foi explorado os tipos de parâmetros que existem para se passar algum valor através das rotas da aplicação. Foi feita a 
utilização de **middlewares** e visto que são três modos que eles podem ser utilizados: 
* Pode ser definida para que toda a aplicação utilize ele, sendo definido no ```app.use(Middleware)```
* Podemos colocá-lo diretamente na rota onde queremos que ele seja executado, logo após a descrição do caminho da rota que será
chamada e antes do **(request, response)**. EG: ```app.get('/projetos', Middleware, (request, response)...```
* Podemos usar o **app.use** mas definindo pelo menos parte da descrição que a rota deve possuir para que o middleware seja
executado. EG: ```app.use('/rotaDesejada', middleware1, middleware2);```. Lembrando que aqui também, podemos passar
quantos middlewares quisermos. 

## Dependências
* **express**  -> micro framework para inicializarmos o projeto do backend e termos acesso ao uso de rotas, middlewares
* **nodemon**  -> utilizado para não haver a necessidade de reiniciar manualmente a aplicação toda vez que alguma alteração é 
realizada, com esta dependência ao salvar o servidor reinicia sozinho
* **uuidv4**   -> utilizada para poder gerar e validar ID's únicos para os registros

## Executar o projeto

Para executar o projeto é necessário que após realizar um ```git clone``` executar o comando ```yarn```para que seja feito
o download da pasta node_modules com as dependências do projeto, e após concluído apenas utilizar o comando ```yarn dev```.
