

[![](https://img.shields.io/badge/Home-000000?style=for-the-badge&logo=markdown&logoColor=white)](home)

# Documentação do negócio
[![](https://img.shields.io/badge/Sprints-000000?style=for-the-badge&logo=markdown&logoColor=white)](sprints)
[![](https://img.shields.io/badge/Requisitos-000000?style=for-the-badge&logo=markdown&logoColor=white)](requisitos)
[![](https://img.shields.io/badge/Processos-000000?style=for-the-badge&logo=markdown&logoColor=white)](processos)
[![](https://img.shields.io/badge/Gerência-000000?style=for-the-badge&logo=markdown&logoColor=white)](gerencia)
[![](https://img.shields.io/badge/Horários-000000?style=for-the-badge&logo=markdown&logoColor=white)](horarios)

# Documentação técnica
[![](https://img.shields.io/badge/Arquitetura-000000?style=for-the-badge&logo=markdown&logoColor=white)](arquitetura)
[![](https://img.shields.io/badge/Mockups-000000?style=for-the-badge&logo=markdown&logoColor=white)](mockups)
[![](https://img.shields.io/badge/Banco_de_dados-000000?style=for-the-badge&logo=markdown&logoColor=white)](banco_dados)
[![](https://img.shields.io/badge/Instalação-000000?style=for-the-badge&logo=markdown&logoColor=white)](instalacao)

---
# $`\mathbb{REQUISITOS}`$
---

# User Stories

* Estas User Stories são um bloco de pequenas User Stories que serão separadas em tarefas.

US|NOME|DESCRIÇÃO|CRITÉRIOS DE ACEITAÇÃO
|---|---|---|---|
**US01**|Tela de envio de PDFs|Eu, como usuário, gostaria de acessar a tela de envio de PDF para que eu possa poder enviar os meus PDFs para extração.|- Deve ser possível arrastar e soltar PDFs<br>- Deve ser possível selecionar um arquivo do computador.<br>- Deve ter um botão de "Enviar para Análise” que vai começar o tratamento dos PDFs<br>-  A tela deve ter a mesma estrutura apresentado no figma oficial<br>- Ao enviar um PDF, deve ser possível dizer de qual montadora (GM ou Jeep) ele pertence.
**US02**|Envio de um PDF|Eu, como usuário, gostaria de enviar os PDFs recebidos pela montadora para que possam ser extraídos os dados deles.|- Deve ser possível enviar mais de um PDF ao mesmo tempo.<br>- O sistema deve auto gerenciar a fila de processos dos PDFs.
**US03**|Tela de extração de dados|Eu, como usuário, gostaria de visualizar o status das extrações de cada um dos PDFs para que eu possa saber quando vai finalizar a extração dos arquivos. |- Deve mostrar um tempo aproximado de conclusão das leituras.<br>- Deve mostrar uma barra de status de cada um dos PDFs sendo extraídos.<br>- Deve mostrar que todos os PDFs foram extraídos antes de continuar.
**US04**|Tela de conclusão de extração|Eu, como usuário, gostaria de visualizar que finalizou a extração dos PDFs para que eu possa depois visualizar os dados.|- O sistema deve me informar de forma clara que todos os PDFs foram extraídos.<br>- Deve possuir um botão com o texto “Visualizar Conteúdo” para o cliente poder continuar.
**US05**|Tela de dados|Eu, como usuário, gostaria de visualizar uma tela com as informações para que eu saiba quais dados foram extraídos do PDF.|- A interface deve seguir o mesmo padrão que o atual sistema (SGS) possui.<br>- Deve ser possível ter dois status de sistema: Visualização e Edição (para correção).<br>- A interface deve possuir, além dos itens essenciais do SGS, uma opção de Descrição Completa vinda da Lista de preços.<br>- Deve estar sinalizado qual é o dado atual que a cliente está mexendo.
**US06**|Seleção de veículo|Eu, como usuário, gostaria de poder selecionar qual veículo vou visualizar os dados para que eu possa tratar os dados deste veículo.|- Deve possuir um menu visual para selecionar qual veículo gostaria de visualizar os dados.
**US07**|Botão de copiar|Eu, como usuário, gostaria de poder copiar um único dado da visualização do veículo  para que eu possa colar no projeto SGS.|- Cada campo da tela de dados deve possuir uma opção de Copiar e Colar.<br>- Quando o cliente copiar, deve mostrar em verde o botão para dizer que foi copiado.<br>- O dado deve ser copiado para a área de transferência da cliente.
**US08**|Edição do campo|Eu, como usuário, gostaria de alterar um dado do veículo  para que eu possa corrigir caso tenha sido extraído de forma errada.|- Deve ter um botão para liberar a alteração de todos os dados.<br>- O botão deve ter diferentes estados dependendo da ativação/inativação da edição.
**US09**|Exportação de JSON|Eu, como usuário, gostaria de exportar os dados em formato JSON para que eu possa utilizá-los externamente.|- Deve ser possível extrair todos os carros em formato JSON.
**US10**|Exportação de CSV|Eu, como usuário, gostaria de exportar os dados em formato CSV para que eu possa utilizá-los externamente.|- Deve ser possível extrair todos os carros em formato CSV.
**US11**|Adição de novo PDF|Eu, como usuário, gostaria de adicionar outro PDF para que eu possa extrair os dados e adicionar aos dados já existentes do veículo. |- Deve ser possível após finalizar a visualização/cópia dos dados poder voltar a tela inicial para envio de novos PDFs.
**US12**|Status de envio|Eu, como usuário, gostaria de visualizar o status de envio para o SGS para que eu saiba quais carros já foram enviados.|- Se os dados não tiverem sido todos copiados, deve mostrar que ainda não foi concluído.<br>- Se todos os dados tiverem sido copiados, ele deve mostrar que foi concluído.<br>- Se o PDF foi enviado mas não foi visualizado.
**US13**|Listar os PDFs exportados|Eu, como usuário, gostaria que o sistema liste os PDFs já extraídos para que eu possa continuar trabalhando em outro momento. |- Deve poder apresentar os PDFs já extraídos.<br>- Deve manter o último estado do PDF quando fechado (manter o que foi extraído).

