# Semana Iniciativa DevOps - KubeDev

- Como resultado da primeira aula (pasta src), foi gerado uma imagem docker e feito upload para o docker hub (https://hub.docker.com/r/davigdc/conversao-temperatura), a aplicação dentro da pasta src é um clone do repositório disponibilizado. Para utilizar a imagem, execute da seguinte forma e acesse em seu navegador na porta 8888 (localhost:8888)

``` bash
docker container run -dp 8888:8080 davigdc/conversao-temperatura
```

- Na segunda aula (pasta kube-news) foi explicado os princípios e finalidades do kubernetes, o objetivo foi criar um cluster local com a ferramenta k3d e subir a aplicação disponibilizada neste cluster, criando o manifesto de deployment e service da aplicação e banco de dados postgres. Foi gerado um novo container e armazenado no docker hub (https://hub.docker.com/r/davigdc/kube-dev). 

- Na terceira aula (pasta terraform) foi criado um cluster k8s na Digital Ocean e "deployado" nossa aplicação para acesso de qualquer lugar.

- Na quarta aula, criamos uma pipeline de CI/CD utilizando o GitHub Actions. A pipeline realiza na parte de CI o build e armazena nosso artefato (container) no DockerHub, na parte de CD ela conecta ao nosso cluster na DigitalOcean e realiza o deploy como magica, sensacional! 