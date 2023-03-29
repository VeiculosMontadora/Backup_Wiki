| [Home](home) | [Sprints](sprints) | [Requisitos](requisitos) | [Arquitetura](arquitetura) | [Processos](processos) | [Configuração](configuracao) | [Mockups](mockups) | [Banco de Dados](banco_dados) | [Instalação](instalacao) | [Gerência de Projeto](Gerenciamento do Projeto) | [Horários Disponiveis](horarios) |
| ------------ | ------------------ | ------------------------ | -------------------------- | ---------------------- | ---------------------------- | ------------------ | ----------------------------- | ------------------------ | ----------------------------------------------- | -------------------------------- |

# Arquitetura

Esta seção é dedicada a apresentar a arquitetura definida para o projeto. Ela está dividida em 3 partes:

- Frontend
- Backend
- Infraestrutura

## Frontend

Trabalho em andamento...

## Backend

Trabalho em andamento...

## Infraestrutura

A seguir é apresentada uma visão geral e em alto nível da infraestrutura do projeto:

![Diagrama Infraestrutura](https://tools.ages.pucrs.br/veiculos-via-montadora/wiki/-/raw/main/pictures/architecture/architecture-diagram.png)

### Diagrama de Deploy

O diagrama a seguir apresenta o processo de deploy da aplicação e

![Diagrama de Deploy](https://tools.ages.pucrs.br/veiculos-via-montadora/wiki/-/raw/main/pictures/architecture/deploy-diagram.png)

### Orçamento AWS

Essa seção apresenta o orçamento da infraestrutura na AWS. O orçamento foi feito utilizando a ferramenta [AWS Pricing Calculator](https://calculator.aws/#/) e busca estimar o custo financeiro para manter a infraestrutura do projeto pelo pelo período de 1 semestre, sendo este a duração do projeto e da disciplina da AGES.

<hr />

- **AWS Lambda:** A função Lambda responsável por executar o código do backend da aplicação será invocada a cada requisição HTTP feita ao backend. Tratando-se de uma API, a função Lambda é cobrada por quantidade de requisições HTTP feitas, mas para gerar um custo realmente significativo, seria necessário um volume de requisições muito grande, na faixa dos milhões de requests. Por esse motivo, considerando que no máximo algumas milhares de requisições serão feitas ao backend, o custo da função Lambda será desprezível.

  **Custo Mensal:** ~ R$ 0,00 -
  **Custo Semestral:** ~ R$ 0,00

<hr />

- **AWS API Gateway:** O AWS API Gateway é um serviço que permite a criação de APIs RESTful. Ele funcionará como um intermédio entre o frontend e o backend da aplicação, fazendo a comunicação entre eles. O AWS API Gateway é também cobrado pela quantidade de requisições HTTP feitas, e, pelo mesmo motivo do função Lambda, o custo será desprezível.

  **Custo Mensal:** ~ R$ 0,00 -
  **Custo Semestral:** ~ R$ 0,00

<hr />

- **AWS S3:** O AWS S3 é um serviço de armazenamento de objetos na nuvem. Ele será utilizado para armazenar o arquivo responsável por guardar o estado do Terraform, o qual será utilizado para provisionar a infraestrutura da aplicação. O custo para armazenar o arquivo será desprezível, visto que o arquivo possui apenas alguns bytes. No entanto, existe a possibilidade de usarmos o AWS S3 para armazenar os PDFs manipulados pelo sistema, os quais são arquivos maiores. Considerando que precisaremos de 10Gb de armazenamento para os arquivos e que a quantidade de dados trafegados será de 100Gb mensais, o custo será de US$ 0.50 por mês, o que representa R$ 2,58.

  **Custo Mensal:** ~ R$ 2,58 -
  **Custo Semestral:** ~ R$ 15,48

<hr />

- **AWS DynamoDB:** O AWS DynamoDB é um serviço de banco de dados NoSQL. Ele será utilizado para armazenar o state lock do Terraform, impedindo com que o Terraform seja executado simultaneamente por mais de uma pessoa. Para isso é criada uma tabela de apenas uma linha, que será utilizada para guardar o lock. O custo para armazenar a tabela será desprezível. A opção `On-Demand` foi escolhida para o DynamoDB ao invés da opção `Provisioned` pois a opção `On-Demand` não possui custo fixo, sendo cobrado apenas pelo uso do serviço. A opção `Provisioned` possui um custo fixo mensal, o que não é interessante para o projeto, visto que o DynamoDB será utilizado apenas para guardar o state lock do Terraform.

  **Custo Mensal:** ~ R$ 0,00 -
  **Custo Semestral:** ~ R$ 0,00

<hr />

- **AWS ECR:** O AWS ECR é um serviço de armazenamento de imagens Docker. Ele será utilizado para armazenar as imagens Docker do frontend e do backend da aplicação. Se considerarmos que precisaremos de 5Gb de armazenamento para as imagens, o custo mensal será de US$ 0.50, o que representa R$ 2,58.

  **Custo Mensal:** ~ R$ 2,58 -
  **Custo Semestral:** ~ R$ 15,48

<hr />

- **AWS EC2:** O AWS EC2 é um serviço de computação em nuvem. Ele será utilizado para hospedar o frontend, o banco de dados e os runners do GitLab. Utilizando um tamanho de instância `t3.small` e ativando a opção de instância sob demanda, a qual gera custos por horas de uso, o custo mensal total será de US$ 15.18, ou R$ 78,48, levando em consideração que a instância ficará ativa 24 horas por dia, 7 dias por semana.

  **Custo Mensal:** ~ R$ 78,48 -
  **Custo Semestral:** ~ R$ 470,88

<hr />

**Resumo Geral:** Para manter a infraestrutura do projeto por 1 semestre, esse será o custo financeiro estimado a cada mês e ao final do semestre:

- **Custo Mensal:** ~ R$ 83,56
- **Custo Semestral:** ~ R$ 501,36

### Permissões AWS Terraform

Para que o Terraform possa provisionar a infraestrutura da aplicação na AWS via pipelines, é necessário que ele tenha permissões para executar as ações necessárias. Caso o Terraform fosse assumir uma `role` na AWS, foi identificado que **pelo menos** as seguintes permissões seriam necessárias:

- **AWSLambda_FullAccess**
- **AmazonEC2FullAccess**
- **AmazonDynamoDBFullAccess**
- **AmazonAPIGatewayAdministrator**
- **AmazonS3FullAccess**
- **AmazonElasticContainerRegistryPublicFullAccess**
- **AmazonVPCFullAccess**
