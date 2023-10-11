# ExampleGateway-Api

## O que é este projeto?

Este projeto é um exemplo simples que demonstra o uso de um Gateway.

## O que é um Gateway?

Um Gateway é como uma porta de entrada única que simplifica o acesso a diferentes serviços ou APIs. Ele facilita o gerenciamento de solicitações,
direcionando-as para os serviços corretos com base em critérios como URLs, métodos HTTP ou cabeçalhos.

## Por que é importante?

- **Centralização:** Um Gateway centraliza o acesso a serviços diversos, reduzindo a complexidade para os usuários e desenvolvedores.
- **Gerenciamento de Tráfego:** Ele ajuda a direcionar e balancear o tráfego entre vários serviços, melhorando a escalabilidade e o desempenho.
- **Segurança:** Pode fornecer recursos de segurança, como autenticação e autorização, protegendo os serviços subjacentes.
- **Monitoramento:** Facilita o monitoramento de solicitações e respostas, permitindo uma melhor análise e solução de problemas.

## Como funciona:

No Visual Studio, temos a nossa estrutura do projeto, com o nosso Gateway e acima os nossos serviços (APIs).

![image](https://github.com/rafaandradde/ExampleGateway-Api/assets/147434748/93398ec0-3aa5-4447-a9ba-a3c04bb10e20)


Nossos serviços simplesmente retornam informações meteorológicas padrão, representando serviços diferentes. Cada serviço é identificado pelo nome da API, que pode ser 'API One'[porta: 44307] ou 'API Two' [porta: 44393] no caso da Service2.

![image](https://github.com/rafaandradde/ExampleGateway-Api/assets/147434748/b59e9073-18b0-4a6c-8306-d653b9aa682a)

![image](https://github.com/rafaandradde/ExampleGateway-Api/assets/147434748/0b0cabed-450f-45b2-acb7-c98caa429b4e)


No nosso Gateway, utilizamos uma classe de configuração chamada 'configuration.development.json'. Nessa classe, definimos as URLs para cada serviço, permitindo que o Gateway saiba como rotear as solicitações para os serviços corretos.

![image](https://github.com/rafaandradde/ExampleGateway-Api/assets/147434748/1543fa97-1aa0-4d40-a58e-5183b31ade63)

![image](https://github.com/rafaandradde/ExampleGateway-Api/assets/147434748/e90650bd-5a4a-4f4c-bbe1-1ddee30129af)



 Agora que exploramos algumas das configurações essenciais, é hora de iniciar os três serviços em janelas separadas. 
Cada serviço representa uma parte fundamental do nosso sistema e precisa estar em execução para que o Gateway funcione corretamente.
(será necessario abrir 3 janelas do Vs, cada uma startando um serviço diferente: Service1, Service2 e Gateway)


No Postman, basta fornecer a URL do nosso Gateway, no caso localhost:44373, e em seguida, especificar qual serviço você deseja acessar, como 'api1'(o nome que você deu ao seu serviço no configuration.development.json). O Gateway cuidará do restante,
direcionando automaticamente sua solicitação para o serviço correto e retornando a resposta apropriada.

![image](https://github.com/rafaandradde/ExampleGateway-Api/assets/147434748/76ecdbdf-39b0-4dfc-85b9-dc1dba22f3f7)

Ao especificar 'api2', observe que a resposta mudará, trazendo dados da 'Api Two'

![image](https://github.com/rafaandradde/ExampleGateway-Api/assets/147434748/2c6543be-2f07-4ffe-b004-9b5416cc1a47)

## Conclusão:
Espero que este exemplo tenha sido útil para compreender o poder e a praticidade de um Gateway na simplificação do acesso a serviços diversos. Sinta-se à vontade para explorar e adaptar este projeto para suas próprias necessidades.







