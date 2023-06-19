

[![](https://img.shields.io/badge/Home-000000?style=for-the-badge&logo=markdown&logoColor=white)](home)

# Documentação do negócio
[![](https://img.shields.io/badge/Sprints-000000?style=for-the-badge&logo=markdown&logoColor=white)](sprints)
[![](https://img.shields.io/badge/Requisitos-000000?style=for-the-badge&logo=markdown&logoColor=white)](requisitos)
[![](https://img.shields.io/badge/Processos-000000?style=for-the-badge&logo=markdown&logoColor=white)](processos)
[![](https://img.shields.io/badge/Gerência-000000?style=for-the-badge&logo=markdown&logoColor=white)](gerencia)
[![](https://img.shields.io/badge/Horários-000000?style=for-the-badge&logo=markdown&logoColor=white)](horarios)
[![](https://img.shields.io/badge/squads-000000?style=for-the-badge&logo=markdown&logoColor=white)](squads)

# Documentação técnica
[![](https://img.shields.io/badge/Arquitetura-000000?style=for-the-badge&logo=markdown&logoColor=white)](arquitetura)
[![](https://img.shields.io/badge/Mockups-000000?style=for-the-badge&logo=markdown&logoColor=white)](mockups)[![](https://img.shields.io/badge/Banco_de_dados-000000?style=for-the-badge&logo=markdown&logoColor=white)](banco_dados)
[![](https://img.shields.io/badge/Instalação-FF7518?style=for-the-badge&logo=markdown&logoColor=black)](instalacao)

---
# $`\mathbb{INSTALAÇÕES \space NECESSÁRIAS}`$
---

### $`\mathbb{FRONTEND}`$
<br>

![Static Badge](https://img.shields.io/badge/Linguagem%3A--gray)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?&logo=typescript&logoColor=blue&color=black)

![Static Badge](https://img.shields.io/badge/Tecnologias%3A--gray)
![HTML5](https://img.shields.io/badge/HTML5-%23E34F26.svg?&logo=html5&logoColor=orange&color=black)
![HTML5](https://img.shields.io/badge/CSS3-%23E34F26.svg?&logo=css3&logoColor=lightblue&color=black)

![Static Badge](https://img.shields.io/badge/Biblioteca_Javascript-React-blue)
![Static Badge](https://img.shields.io/badge/Enviroment-Node.js-green)
![Static Badge](https://img.shields.io/badge/Interface-MaterialUI-orange)


## Como executar para ambiente de desenvolvimento

1. Instale o Node.js, versão >= 18.
2. Instale o Yarn com o comando `npm install -g yarn`.
3. Instale as dependências do projeto com o comando `yarn install`.
    3.1. Para isso, é necessário estar com um terminal aberto na pasta raiz do projeto.
4. Execute o comando `yarn dev` para iniciar o servidor de desenvolvimento.
    4.1. Depois, acesse o endereço `http://localhost:3000` no seu navegador.
5. Para mais comandos, veja o arquivo `package.json` em 'scripts'.

---

### $`\mathbb{BACKEND}`$
<br>

![Static Badge](https://img.shields.io/badge/Linguagem%3A--gray)
![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&color=black)

![Static Badge](https://img.shields.io/badge/Framework-FastAPI-lightblue)
![Static Badge](https://img.shields.io/badge/Arquitetura-REST-green)
![Static Badge](https://img.shields.io/badge/Testes-PyTest-orange)

- Passos:

1. Instale o Python, versão >= 3.9
2. Instale o Docker, em sua versão mais recente
3. Instale o gerenciador de dependências Poetry na versão 1.4.1:
```
$ pip install poetry==1.4.1
```
1. Configure o virtualenv:
```
$ poetry config virtualenvs.in-project true
```
1. Instale as dependências:
```
$ poetry install
```
1. Agora o backend pode ser executado:
```
poetry run uvicorn app.main:app --reload
```
---

### $`\mathbb{DATABASE}`$
<br>

![Static Badge](https://img.shields.io/badge/Tecnologia_de_Conteineriza%C3%A7%C3%A3o%3A-gray)
![Static Badge](https://img.shields.io/badge/Docker-black?logo=docker)

![Static Badge](https://img.shields.io/badge/Banco%20de%20dados-N%C3%A3o_Relacional-red)

![Static Badge](https://img.shields.io/badge/Tecnologia%3A-gray)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?&logo=mongodb&logoColor=white)



1. Instale o Docker, em sua versão mais recente
2. O banco de dados pode ser executado com o comando:
```
docker compose up mongodb
```