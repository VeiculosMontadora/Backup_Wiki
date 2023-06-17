

[![](https://img.shields.io/badge/Home-000000?style=for-the-badge&logo=markdown&logoColor=white)](home)

# Documentação do negócio
[![](https://img.shields.io/badge/Sprints-000000?style=for-the-badge&logo=markdown&logoColor=white)](sprints)
[![](https://img.shields.io/badge/Requisitos-000000?style=for-the-badge&logo=markdown&logoColor=white)](requisitos)
[![](https://img.shields.io/badge/Processos-FF7518?style=for-the-badge&logo=markdown&logoColor=black)](processos)
[![](https://img.shields.io/badge/Gerência-000000?style=for-the-badge&logo=markdown&logoColor=white)](gerencia)
[![](https://img.shields.io/badge/Horários-000000?style=for-the-badge&logo=markdown&logoColor=white)](horarios)
[![](https://img.shields.io/badge/squads-000000?style=for-the-badge&logo=markdown&logoColor=white)](squads)

# Documentação técnica
[![](https://img.shields.io/badge/Arquitetura-000000?style=for-the-badge&logo=markdown&logoColor=white)](arquitetura)
[![](https://img.shields.io/badge/Mockups-000000?style=for-the-badge&logo=markdown&logoColor=white)](mockups)
[![](https://img.shields.io/badge/Banco_de_dados-000000?style=for-the-badge&logo=markdown&logoColor=white)](banco_dados)
[![](https://img.shields.io/badge/Instalação-000000?style=for-the-badge&logo=markdown&logoColor=white)](instalacao)
[![](https://img.shields.io/badge/Configuração-000000?style=for-the-badge&logo=markdown&logoColor=white)](configuracao)

---
# $`\mathbb{PROCESSO \space DE \space DESENVOLVIMENTO}`$
---

Esta seção é dedicada a apresentar o processo de desenvolvimento do time, junto dela serão apresentados documentos referentes a maneira como o time se organizou e trabalha.

## Sumário

- [Git Workflow](#git-workflow)
- [Code Freezing](#code-freezing)
- [Definition of Ready](#definition-of-ready)
- [Definition of Done](#definition-of-done)

## Git Workflow

Git Workflow é um conjunto de práticas e padrões que as equipes de desenvolvimento usam para colaborar em projetos de software usando o sistema de controle de versão Git.

O Git é uma ferramenta poderosa que permite que os desenvolvedores trabalhem juntos em um mesmo código-fonte sem causar conflitos ou perder trabalho. O Git workflow estabelece uma estrutura para como as alterações no código são gerenciadas, revisadas e implementadas, a fim de garantir que o projeto progrida de maneira organizada e eficiente.

![Imagem](https://tools.ages.pucrs.br/veiculos-via-montadora/wiki/-/raw/8fc13462c45d4d57092f42dc5079c549e71a340a/pictures/processes/gitflow-example.png)

Na imagem acima, é possível observar que um repositório pode ser organizado em galhos, ou ‘branches’. Existe o galho principal ‘master’ e o galho de desenvolvimento ‘develop’, sendo possível criar outros galhos que implementam funcionalidades novas no sistema a partir de ‘develop’. As alterações feitas em outras branches eventualmente são aprovadas e vão para ‘develop’, e, por fim, para ‘master’.

### Fluxo das Branches

Para este projeto, foi-se definido que teremos 2 branches principais, `main` e `develop`.

- `main`: Essa é a branch principal que armazenará o código de cada entrega por Sprint, nessa branch é estritamente necessário que tenhamos o código da aplicação funcionando sem erros, já testado e validado.

- `develop`: Deve-se sempre criar novas branches a partir da develop. Ela será nosso ambiente de desenvolvimento.

### Nomes das Branches

Para padronizar os nomes das branches, deve-se nomeá-las da seguinte forma:

```
<UserStory>-<Descrição>
```

Como por exemplo:
```
US04-add-login
```

### Semântica dos Commits

Para padronizarmos a descrição dos commits, será utilizado um padrão semântico a fim de facilitar o compreendimento de cada commit. Os padrões serão os seguintes:

- **feat:** Tratam adições de novas funcionalidades ou de quaisquer outras novas implantações ao código;
- **fix:** Essencialmente definem o tratamento de correções de bugs;
- **docs:** referem-se a inclusão ou alteração somente de arquivos de documentação;
- **test:** Adicionando testes ausentes ou corrigindo testes existentes nos processos de testes automatizados (TDD);
- **build:** Alterações que afetam o sistema de construção ou dependências externas (escopos de exemplo: gulp, broccoli, npm),
- **ci:** Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs);
- **perf:** Uma alteração de código que melhora o desempenho;
- **refactor:** Tipo utilizado em quaisquer mudanças que sejam executados no código, porém não alterem a funcionalidade final da tarefa impactada;
- **style:** Alterações referentes a formatações na apresentação do código que não afetam o significado do código, como por exemplo: espaço em branco, formatação, ponto e vírgula ausente etc.);
- **chore:** Atualização de tarefas que não ocasionam alteração no código de produção, mas mudanças de ferramentas, mudanças de configuração e bibliotecas que realmente não entram em produção;
- **revert** Reverter mudanças;

Exemplo da descrição commit:
```
fix: login error -> qualquer coisa aqui
```

https://platform.uno/docs/articles/uno-development/git-conventional-commits.html

### Criando uma Branch

Para criar uma branch e começar a trabalhar nela, 3 comandos git serão essenciais, vejamos abaixo quais são eles:

```sh
git checkout develop # Vai para a branch ‘develop’.
git pull # Puxa as modificações remotas.
git checkout -b <NOME_DA_SUA_BRANCH_AQUI> # Cria uma nova branch.
```

Utilizando os comandos acima, você estará indo para a branch ‘develop’, puxando todas as modificações remotas e criando uma nova branch a partir de ‘develop’. Você então passará a trabalhar na nova branch criada.

---

### Code freezing

Code freezing é uma data para congelamento de entrada de código em produção. Após essa data, nenhum merge request será mais aceito. A única coisa que pode passar por esse bloqueio são hotfixes para erros em produção.

---

### Definition of Ready

Para que uma tarefa seja considerada pronta para desenvolvimento, ela deve seguir as seguintes condições:
- Qualquer tarefa da qual ela tenha dependência.
- O ambiente de desenvolvimento local deve estar devidamente setado.

---

### Definition of Done

Para que uma tarefa seja considerada concluída ela deve seguir as seguintes condições:
- O merge request da branch em que a tarefa foi desenvolvida para a develop deve ter sido concluída.
- O código deve ter sido revisado e aprovado.
- O código deve ter testes unitários e ter sido testado manualmente.
- Qualquer documentação necessária deve ter sido escrita (payloads, endpoints, ...).

---
