

[![](https://img.shields.io/badge/Home-000000?style=for-the-badge&logo=markdown&logoColor=white)](home)

# Documentação do negócio
[![](https://img.shields.io/badge/Sprints-000000?style=for-the-badge&logo=markdown&logoColor=white)](sprints)
[![](https://img.shields.io/badge/Requisitos-000000?style=for-the-badge&logo=markdown&logoColor=white)](requisitos)
[![](https://img.shields.io/badge/Processos-000000?style=for-the-badge&logo=markdown&logoColor=white)](processos)
[![](https://img.shields.io/badge/Gerência-000000?style=for-the-badge&logo=markdown&logoColor=white)](gerencia)
[![](https://img.shields.io/badge/Horários-000000?style=for-the-badge&logo=markdown&logoColor=white)](horarios)

# Documentação técnica
[![](https://img.shields.io/badge/Arquitetura-FF7518?style=for-the-badge&logo=markdown&logoColor=black)](arquitetura)
[![](https://img.shields.io/badge/Mockups-000000?style=for-the-badge&logo=markdown&logoColor=white)](mockups)
[![](https://img.shields.io/badge/Banco_de_dados-000000?style=for-the-badge&logo=markdown&logoColor=white)](banco_dados)
[![](https://img.shields.io/badge/Instalação-000000?style=for-the-badge&logo=markdown&logoColor=white)](instalacao)
[![](https://img.shields.io/badge/Configuração-000000?style=for-the-badge&logo=markdown&logoColor=white)](configuracao)

---
# $`\mathbb{ARQUITETURA}`$
---

Esta seção é dedicada a apresentar a arquitetura definida para o projeto. Ela está dividida em 3 partes:

- Frontend
- Backend
- Infraestrutura

## Frontend

**Repositório:** https://tools.ages.pucrs.br/veiculos-via-montadora/frontend

Trabalho em andamento...

## Backend

**Repositório:** https://tools.ages.pucrs.br/veiculos-via-montadora/backend

Trabalho em andamento...

## Infraestrutura

**Repositório:** https://tools.ages.pucrs.br/veiculos-via-montadora/infrastructure

Nessa seção, será apresentada uma visão geral da infraestrutura do projeto.

### Diagrama de Deploy

O diagrama a seguir apresenta a arquitetura em alto nível e o processo de deploy da infraestrutura do projeto Veículos Via Montadora:

![Diagram Arquitetura](https://tools.ages.pucrs.br/veiculos-via-montadora/wiki/-/raw/main/pictures/architecture/architecture-deploy-diagram.png)

### Orçamento AWS

Essa seção apresenta o orçamento da infraestrutura na AWS. O orçamento foi feito utilizando a ferramenta [AWS Pricing Calculator](https://calculator.aws/#/) e busca estimar o custo financeiro para manter a infraestrutura do projeto pelo pelo período de 1 semestre, sendo este a duração do projeto e da disciplina da AGES.

O PDF gerado através do AWS Pricing Calculator com o orçamento para a infraestrutura do projeto pode ser encontrado nesse link: https://tools.ages.pucrs.br/veiculos-via-montadora/wiki/-/blob/main/documents/architecture/aws-budget.pdf

A seguir serão apresentados os componentes (serviços da AWS) que irão compor a infraestrutura do projeto Veículos Via Montadora:

<hr />

- **AWS Lambda:** A função Lambda responsável por executar o código do backend da aplicação será invocada a cada requisição HTTP feita ao backend.

<hr />

- **AWS API Gateway:** O AWS API Gateway é um serviço que permite a criação de APIs RESTful. Ele funcionará como um intermédio entre o frontend e o backend da aplicação, fazendo a comunicação entre eles

<hr />

- **AWS S3:** O AWS S3 é um serviço de armazenamento de objetos na nuvem. Ele será utilizado para armazenar o arquivo responsável por guardar o estado do Terraform, o qual será utilizado para provisionar a infraestrutura da aplicação.

<hr />

- **AWS DynamoDB:** O AWS DynamoDB é um serviço de banco de dados NoSQL. Ele será utilizado para armazenar o state lock do Terraform, impedindo com que o Terraform seja executado simultaneamente por mais de uma pessoa. Para isso é criada uma tabela de apenas uma linha, que será utilizada para guardar o lock. O custo para armazenar a tabela será desprezível. A opção `On-Demand` foi escolhida para o DynamoDB ao invés da opção `Provisioned` pois a opção `On-Demand` não possui custo fixo, sendo cobrado apenas pelo uso do serviço. A opção `Provisioned` possui um custo fixo mensal, o que não é interessante para o projeto, visto que o DynamoDB será utilizado apenas para guardar o state lock do Terraform.

<hr />

- **AWS ECR:** O AWS ECR é um serviço de armazenamento de imagens Docker. Ele será utilizado para armazenar as imagens Docker do frontend e do backend da aplicação.

<hr />

- **AWS EC2:** O AWS EC2 é um serviço de computação em nuvem. Ele será utilizado para hospedar o frontend, o banco de dados e os runners do GitLab.

<hr />

**Resumo Geral:** Para manter a infraestrutura do projeto por 1 semestre, esse será o custo financeiro estimado a cada mês e ao final do semestre:

- **Custo Mensal:** ~ 12,56 USD
- **Custo Semestral:** ~ (12,56 USD * 6) = 75,36 USD

### Permissões AWS Terraform

Para que o Terraform possa provisionar a infraestrutura da aplicação na AWS via pipelines, é necessário que ele tenha permissões para executar as ações necessárias. Caso o Terraform fosse assumir uma `role` ou fazer uso das credenciais de uma conta na AWS, foi identificado que **pelo menos** as seguintes permissões teriam de ser concedidas à role ou à conta:

- **AWSLambda_FullAccess**
- **AmazonEC2FullAccess**
- **AmazonDynamoDBFullAccess**
- **AmazonAPIGatewayAdministrator**
- **AmazonS3FullAccess**
- **AmazonElasticContainerRegistryPublicFullAccess**
- **AmazonVPCFullAccess**
