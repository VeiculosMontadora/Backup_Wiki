

[![](https://img.shields.io/badge/Home-000000?style=for-the-badge&logo=markdown&logoColor=white)](home)

# Documentação do negócio
[![](https://img.shields.io/badge/Sprints-000000?style=for-the-badge&logo=markdown&logoColor=white)](sprints)
[![](https://img.shields.io/badge/Requisitos-000000?style=for-the-badge&logo=markdown&logoColor=white)](requisitos)
[![](https://img.shields.io/badge/Processos-000000?style=for-the-badge&logo=markdown&logoColor=white)](processos)
[![](https://img.shields.io/badge/Gerência-000000?style=for-the-badge&logo=markdown&logoColor=white)](gerencia)
[![](https://img.shields.io/badge/Horários-000000?style=for-the-badge&logo=markdown&logoColor=white)](horarios)
[![](https://img.shields.io/badge/squads-000000?style=for-the-badge&logo=markdown&logoColor=white)](squads)

# Documentação técnica
[![](https://img.shields.io/badge/Arquitetura-FF7518?style=for-the-badge&logo=markdown&logoColor=black)](arquitetura)
[![](https://img.shields.io/badge/Mockups-000000?style=for-the-badge&logo=markdown&logoColor=white)](mockups)
[![](https://img.shields.io/badge/Banco_de_dados-000000?style=for-the-badge&logo=markdown&logoColor=white)](banco_dados)
[![](https://img.shields.io/badge/Instalação-000000?style=for-the-badge&logo=markdown&logoColor=white)](instalacao)

---
# $`\mathbb{ARQUITETURA}`$
---

Esta seção é dedicada a apresentar a arquitetura definida para o projeto. Ela está dividida em 3 partes:

- Frontend
- Backend
- Infraestrutura

## Frontend

**Repositório:** https://tools.ages.pucrs.br/veiculos-via-montadora/frontend

---

## Backend

**Repositório:** https://tools.ages.pucrs.br/veiculos-via-montadora/backend

- Diagrama de caminho do programa

```mermaid
graph 

subgraph Caminho das requisições
    I((Inicio))
    R(Routers/Controllers)
    S(Services)
    Repo[Repository]
    DB[(MongoDB)]
end

I -->|Requisições HTTPS|R
R <--> S
S <--> Repo
Repo <--> DB
```

Neste diagrama, temos os seguintes componentes:

- $`\color{yellow}\sf Routers`$ (Rotas): Responsáveis por definir as rotas HTTP do aplicativo FastAPI.
- $`\color{yellow}\sf Controllers`$ (Controladores): Lidam com a lógica de negócios para cada rota, processando as solicitações e retornando as respostas adequadas.
- $`\color{yellow}\sf Services`$ (Serviços): Realizam a lógica de negócios principal do aplicativo, que pode envolver validações, chamadas a APIs externas, processamento de dados, etc.
- $`\color{yellow}\sf Repository`$ (Repositório): Faz a interação com o banco de dados MongoDB, executando operações de leitura/gravação.
- $`\color{yellow}\sf MongoDB`$: Banco de dados NoSQL utilizado para armazenar e recuperar os dados do aplicativo.

* Diagrama de arquivos

```mermaid
graph

    subgraph Diagrama de Arquivos
        init("#128193; backend/")
        app("#128193; app/")
        apis("#128193; api/")
        databases("#128193; database/")
        pdfs("#128193; pdf/")
        tests("#128193; test/")
        utilss("#128193; utils/")
        configpy("#128196; config.py")
        mainpy("#128196; main.py")

    subgraph api
        mappers("#128193; mappers/")
        models("#128193; models/")
        repositories("#128193; repositories/")
        routers("#128193; routers/")
        services("#128193; services/")
    end

    subgraph database
        mongopy("#128196; mongo.py")
    end

    subgraph pdf
        chevrolet("#128193; chevrolet/")
        jeep("#128193; jeep/")
        exceptionspy("#128196; exceptions.py")
    end

    subgraph test
        mocker("#128193; mockers/")
        pdfsamples("#128193; pdf_samples/")
    end

    subgraph utils
        util("#128196; utils.py")
    end

    subgraph mockers
        pdfmockers("#128196; pdf_mocker.py")
        veiculomocker("#128196; veiculo_mocker.py")
    end
    
    init --> app
    init --> configpy
    init --> mainpy
    app --> apis
    app --> databases
    app --> pdfs
    app --> tests
    app --> utilss
    apis --> api
    pdfs --> pdf
    mocker --> mockers
    databases --> database
    tests --> test
    utilss --> util
end

```

Neste diagrama, temos os seguintes componentes:

- $`\color{yellow}\sf app/api/mappers/`$: diretório onde estão os  componentes ou classes responsáveis por mapear e transformar dados entre diferentes formatos ou estruturas. Em uma API REST, os mappers são comumente usados para converter objetos de domínio em objetos de transferência de dados (DTOs) e vice-versa, facilitando a comunicação entre a camada de serviço e a camada de controle.
- $`\color{yellow}\sf app/api/models/`$: diretório onde estão os arquivos que possuem a estrutura de dados com as informações dos objetos da API REST.
- $`\color{yellow}\sf app/api/repositories/`$: diretório onde estão as classes ou componentes responsáveis por acessar e manipular dados persistentes em uma API REST.
- $`\color{yellow}\sf app/api/routers/`$: diretório com os arquivos responsáveis por definir as rotas e endpoints da API REST, mapeando as requisições HTTP recebidas para as funções ou métodos correspondentes nos controladores.
- $`\color{yellow}\sf app/api/services/`$: diretório com componentes ou classes responsáveis por implementar a lógica de negócios e executar operações complexas em uma API REST, isolando essa lógica dos controladores e dos repositórios.
- $`\color{yellow}\sf app/database/`$: diretório onde estão as configurações em formato JSON do banco de dados mongodb.
- $`\color{yellow}\sf app/pdf/`$: diretório onde estão os algoritmos de tratamento e extração de dados dos PDFs.
- $`\color{yellow}\sf app/test/`$: diretório onde estão os testes do programa.
- $`\color{yellow}\sf app/utils/`$: diretório com bibliotecas auxiliares ao projeto.
- $`\color{orange}\sf app/config.py`$: arquivo de configuração do projeto.
- $`\color{orange}\sf app/main.py`$: arquivo principal para compilar o projeto e rodar todas as dependências escritas.

---

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

- **AWS Lambda:** A função Lambda responsável por executar o código do backend da aplicação será invocada a cada requisição HTTP feita ao backend.

- **AWS API Gateway:** O AWS API Gateway é um serviço que permite a criação de APIs RESTful. Ele funcionará como um intermédio entre o frontend e o backend da aplicação, fazendo a comunicação entre eles

- **AWS S3:** O AWS S3 é um serviço de armazenamento de objetos na nuvem. Ele será utilizado para armazenar o arquivo responsável por guardar o estado do Terraform, o qual será utilizado para provisionar a infraestrutura da aplicação.

- **AWS DynamoDB:** O AWS DynamoDB é um serviço de banco de dados NoSQL. Ele será utilizado para armazenar o state lock do Terraform, impedindo com que o Terraform seja executado simultaneamente por mais de uma pessoa. Para isso é criada uma tabela de apenas uma linha, que será utilizada para guardar o lock. O custo para armazenar a tabela será desprezível. A opção `On-Demand` foi escolhida para o DynamoDB ao invés da opção `Provisioned` pois a opção `On-Demand` não possui custo fixo, sendo cobrado apenas pelo uso do serviço. A opção `Provisioned` possui um custo fixo mensal, o que não é interessante para o projeto, visto que o DynamoDB será utilizado apenas para guardar o state lock do Terraform.

- **AWS ECR:** O AWS ECR é um serviço de armazenamento de imagens Docker. Ele será utilizado para armazenar as imagens Docker do frontend e do backend da aplicação.

- **AWS EC2:** O AWS EC2 é um serviço de computação em nuvem. Ele será utilizado para hospedar o frontend, o banco de dados e os runners do GitLab.

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
