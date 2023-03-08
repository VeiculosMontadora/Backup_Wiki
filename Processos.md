|[Home](home)|[Sprints](sprints)|[Requisitos](requisitos)|[Arquitetura](arquitetura)|[Processos](processos)|[Configuração](configuracao)|[Mockups](mockups)|[Banco de Dados](banco_dados)|[Instalação](instalacao)|[Gerência de Projeto](Gerenciamento do Projeto)|[Horários Disponiveis](horarios)|
|---|---|---|---|---|---|---|---|---|---|---|

# Processo de Desenvolvimento

Esta seção é dedicada a apresentar o processo de desenvolvimento do time, junto dela serão apresentados documentos referentes a maneira como o time se organizou e trabalha.

## Sumário

- [Git Workflow](#git-workflow)
- [Template Pull Request](#template-pull-request)

## Git Workflow

### Nomes das Branches

Para padronizarmos os nomes das branches, deve-se nomeá-las da seguinte forma:

```
<UserStory>-<Descrição>
```

Como por exemplo:
```
US04-DesenvolverLogin
```

### Semântica dos Commits

Para padronizarmos a descrição dos commits, será utilizado um padrão semântico a fim de facilitar o compreendimento de cada commit. Os padrões serão os seguintes:


- **feature:** Tratam adições de novas funcionalidades ou de quaisquer outras novas implantações ao código;
- **fix:** Essencialmente definem o tratamento de correções de bugs;
- **docs:** referem-se a inclusão ou alteração somente de arquivos de documentação;
- **test:** Adicionando testes ausentes ou corrigindo testes existentes nos processos de testes automatizados (TDD);
- **build:** Alterações que afetam o sistema de construção ou dependências externas (escopos de exemplo: gulp, broccoli, npm),
- **ci:** Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs);
- **perf:** Uma alteração de código que melhora o desempenho;
- **refactor:** Tipo utilizado em quaisquer mudanças que sejam executados no código, porém não alterem a funcionalidade final da tarefa impactada;
- **style:** Alterações referentes a formatações na apresentação do código que não afetam o significado do código, como por exemplo: espaço em branco, formatação, ponto e vírgula ausente etc.);
- **chore:** Atualização de tarefas que não ocasionam alteração no código de produção, mas mudanças de ferramentas, mudanças de configuração e bibliotecas que realmente não entram em produção;
- **env:** basicamente utilizado na descrição de modificações ou adições em arquivos de configuração em processos e métodos de integração contínua (CI), como parâmetros em arquivos de configuração de containers.

Exemplo da descrição commit:
```
fix-loginError
```

### Criando uma Branch

Para criar uma branch e começar a trabalhar nela, 3 comandos git serão essenciais, vejamos abaixo quais são eles:

```sh
git checkout develop # Vai para a branch ‘development’.
git pull # Puxa as modificações remotas.
git checkout -b <NOME_DA_SUA_BRANCH_AQUI> # Cria uma nova branch.
```

Utilizando os comandos acima, você estará indo para a branch ‘develop’, puxando todas as modificações remotas e criando uma nova branch a partir de ‘develop’. Você então passará a trabalhar na nova branch criada.

## Template Pull Request 

