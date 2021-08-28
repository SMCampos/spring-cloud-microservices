# Spring-Cloud-Microservices
Projeto utilizando Java Spring Cloud com Microsserviços - Bootcamp Santander Fullstack Dev - DIO

O objetivo do projeto é demonstrar a utilização de microsserviços através do Spring Cloud.

Para o desenvolvimento do Projeto foi utilizado o IntelliJ

Também foi utilizado o Docker com a virtualização de imagem do Elasticsearch e do Redis.

Foram criados os projetos através do Spring Initializr:

No IntelliJ os projetos foram importados através do File - New Modules from Existing Sources

#Product-Catalog

#Shopping-Cart

#Config Server
Para gerenciar as configurações foi criado o Config Server através do Spring Cloud ConfigServer.
Foi criado um repositório no GitHub com as configurações dos microsserviços o qual será chamado
pelo Config Server para a execução dos microsserviços.
https://github.com/SMCampos/configs-spring-cloud-microservices.git

Seguindo as boas práticas de microsserviços as configurações foram centralizadas no servidor de
configurações.

#Service Discovery
Para gerenciar as chamadas entre microsserviços foi criado o Service Discovery.
Quando um microsserviço é inicializado ele vai ser registrado no Service Discovery, que verifica
a porta que o microsserviço vai utilizar.
Ele faz a verificação de solicitações de um microsserviço com outro evitando que ocorram chamadas
diretamente ente eles.
O service discovery faz o load balance.

#Gateway
Foi criado o Gateway para interligar o acesso às chamadas dos microsserviços.






