# Semana Iniciativa DevOps - KubeDev

- Como resultado da primeira aula, foi gerado uma imagem docker e feito upload para meu docker hub (https://hub.docker.com/r/davigdc/conversao-temperatura), a aplicação dentro da pasta src, é um clone do repositório disponibilizado (https://github.com/KubeDev/conversao-temperatura). Para utilizar a imagem, execute da seguinte forma e acesse em seu navegador na porta 8888 (localhost:888)

``` bash
docker container run -dp 8888:8080 davigdc/conversao-temperatura
```