|[Home](home)|[Sprints](sprints)|[Requisitos](requisitos)|[Arquitetura](arquitetura)|[Processos](processos)|[Configuração](configuracao)|[Mockups](mockups)|[Banco de Dados](banco_dados)|[Instalação](instalacao)|[Gerência de Projeto](Gerenciamento do Projeto)|[Horários Disponiveis](horarios)|
|---|---|---|---|---|---|---|---|---|---|---|

---
# $`\mathbb{REQUISITOS}`$
---

Documento melhorado: [https://github.com/VeiculosMontadora/Management/blob/main/UserStories.md](https://github.com/VeiculosMontadora/Management/blob/main/UserStories.md)

### $`\mathbb{EPICS}`$

<table align="center"><tr><td align="center" width="9999">
<table>
<thead>
<tr>
<th colspan="3">
<p><span style="color: #339966;"><strong>E01</strong></span></p>
</th>
</tr>
<tr>
<th rowspan="2">
<p><strong>T&iacute;tulo</strong></p>
<p><span style="font-weight: 400;">Envio de PDFs</span></p>
</th>
<th rowspan="2">
<p><strong>Prioridade</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</th>
<th rowspan="2">
<p><strong>Estimativa</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="3">
<p><strong>User Stories:</strong></p>
 [E01-US01](#E01-US01), <a href="#E01-US02">E01-US02</a>, <a href="#E01-US03">E01-US03</a>
</td>
</tr>
</tbody>
</table>
</td></tr></table>

---

<table align="center"><tr><td align="center" width="9999">
<table>
<thead>
<tr>
<th colspan="3">
<p><span style="color: #339966;"><strong>E02</strong></span></p>
</th>
</tr>
<tr>
<th rowspan="2">
<p><strong>T&iacute;tulo</strong></p>
<p><span style="font-weight: 400;">Extra&ccedil;&atilde;o de dados do&nbsp; PDF</span></p>
</th>
<th rowspan="2">
<p><strong>Prioridade</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</th>
<th rowspan="2">
<p><strong>Estimativa</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="3">
<p><strong>User Stories:</strong></p>
<a href="#E02-US01">E02-US01</a>, <a href="#E02-US02">E02-US02</a>, <a href="#E02-US03">E02-US03</a>, <a href="#E02-US04">E02-US04</a>, <a href="#E02-US05">E02-US05</a>, <a href="#E02-US06">E02-US06</a>
</td>
</tr>
</tbody>
</table>
</td></tr></table>

---

<table align="center"><tr><td align="center" width="9999">
<table>
<thead>
<tr>
<th colspan="3">
<p><span style="color: #339966;"><strong>E03</strong></span></p>
</th>
</tr>
<tr>
<th rowspan="2">
<p><strong>T&iacute;tulo</strong></p>
<p><span style="font-weight: 400;">Visualizar os dados do PDF</span></p>
</th>
<th rowspan="2">
<p><strong>Prioridade</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</th>
<th rowspan="2">
<p><strong>Estimativa</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="3">
<p><strong>User Stories:</strong></p>
<a href="#E03-US01">E03-US01</a>, <a href="#E03-US02">E03-US02</a>, <a href="#E03-US03">E03-US03</a>, <a href="#E03-US04">E03-US04</a>, <a href="#E03-US05">E03-US05</a>, <a href="#E03-US06">E03-US06</a>
</td>
</tr>
</tbody>
</table>
</td></tr></table>

---

### $`\mathbb{USER \space STORIES}`$

---

<a id="E01-US01"></a>
<table>
<tbody>
<tr>
<td colspan="3">
<p><strong>E01-US01</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Exporta&ccedil;&atilde;o de PDF</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>Gostaria de</strong><span style="font-weight: 400;"> enviar os PDFs recebidos pela montadora&nbsp;</span></p>
<p><strong>Para que</strong><span style="font-weight: 400;"> possam ser extra&iacute;dos os dados deles.</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- Deve ser poss&iacute;vel enviar mais de um PDF ao mesmo tempo.</span></p>
<br />
<p><span style="font-weight: 400;">- Deve ser poss&iacute;vel visualizar e interagir com uma interface de envios de PDF</span></p>
<br />
<p><span style="font-weight: 400;">- Deve ser poss&iacute;vel arrastar e soltar PDFs.</span></p>
<br />
<p><span style="font-weight: 400;">- Deve possuir uma valida&ccedil;&atilde;o de arquivos (se o arquivo em quest&atilde;o &eacute; um PDF ou n&atilde;o).</span></p>
<br />
<p><span style="font-weight: 400;">- Deve ser coletado o nome do PDF.</span></p>
<br />
<p><span style="font-weight: 400;">- A interface de envio de PDF deve ajustar o tamanho conforme os PDFs s&atilde;o enviados.</span></p>
</td>
</tr>
</tbody>
</table>

---

<table>
<tbody>
<tr>
<td colspan="3">
<a id="E01-US02"></a>
<p><strong>E01-US02</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Visualizar os PDFs enviados</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>Gostaria de</strong><span style="font-weight: 400;"> visualizar os PDFs que enviei</span></p>
<p><strong>Para que</strong><span style="font-weight: 400;"> eu possa verificar se enviei certo</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- Deve poss&iacute;vel visualizar a lista de PDFs enviados</span></p>
<br />
<p><span style="font-weight: 400;">- Deve ser poss&iacute;vel visualizar o estado do envio (se o envio deu certo ou n&atilde;o)</span></p>
<br />
<p><span style="font-weight: 400;">- Deve ser poss&iacute;vel excluir o PDF individualmente, caso precise</span></p>
<br />
<p><span style="font-weight: 400;">- Deve ser poss&iacute;vel enviar mais PDFs, caso precise</span></p>
</td>
</tr>
</tbody>
</table>

---

<table>
<tbody>
<tr>
<td colspan="3">
<a id="E01-US03"></a>
<p><strong>E01-US03</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Enviar PDF para an&aacute;lise</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>Gostaria de</strong><span style="font-weight: 400;"> enviar os PDFs selecionados anteriormente</span></p>
<p><strong>Para que</strong><span style="font-weight: 400;"> o sistema possa extrair os seus dados.</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- Deve possuir um bot&atilde;o de envio dos PDFs selecionados para a extra&ccedil;&atilde;o</span></p>
<br />
<p><span style="font-weight: 400;">- Deve ser poss&iacute;vel visualizar, de forma clara, a disponibilidade de enviar para extra&ccedil;&atilde;o (bot&atilde;o deve estar indispon&iacute;vel at&eacute; concluir as importa&ccedil;&otilde;es)</span></p>
<br />
<p><span style="font-weight: 400;">-</span><span style="font-weight: 400;"> Deve ser identificado automaticamente qual a montadora do PDF e exibi-lo de forma clara.</span></p>
<br />
<p><span style="font-weight: 400;">- Caso o t&iacute;tulo do PDF n&atilde;o apresente qual a montadora, deve ser colocado manualmente</span></p>
</td>
</tr>
</tbody>
</table>

---

<table>
<tbody>
<tr>
<td colspan="3">
<a id="E02-US01"></a>
<p><strong>E02-US01</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Gerenciamento de Extra&ccedil;&atilde;o</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>Gostaria de</strong><span style="font-weight: 400;"> ver os PDFs sendo extra&iacute;dos</span></p>
<p><strong>Para que</strong><span style="font-weight: 400;"> eu possa saber quando eles foram finalizados.</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- Deve mostrar um tempo aproximado de conclus&atilde;o das leituras.</span></p>
<p><span style="font-weight: 400;">- Deve mostrar uma barra de status de cada um dos PDFs sendo extra&iacute;dos.</span></p>
<p><span style="font-weight: 400;">- Deve mostrar que todos os PDFs foram extra&iacute;dos antes de continuar.</span></p>
<p><span style="font-weight: 400;">- Deve mostrar de forma visual o atual estado da extra&ccedil;&atilde;o (Erro na extra&ccedil;&atilde;o ou Extra&ccedil;&atilde;o conclu&iacute;da).</span></p>
<p><span style="font-weight: 400;">- Deve possuir um bot&atilde;o para redirecionar para a &aacute;rea de visualiza&ccedil;&atilde;o de dados.</span></p>
</td>
</tr>
</tbody>
</table>

---

<table>
<tbody>
<tr>
<td colspan="3">
<a id="E02-US02"></a>
<p><strong>E02-US02</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Extra&ccedil;&atilde;o MEV Tracker</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>Gostaria de</strong><span style="font-weight: 400;"> extrair os dados do PDF Manual de Especifica&ccedil;&atilde;o do Ve&iacute;culo (MEV) do modelo de PDF da Tracker</span></p>
<p><strong>Para que</strong><span style="font-weight: 400;"> eu possa visualizar os dados necess&aacute;rios.</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- Deve extrair os dados da(s) tabela(s) com o modelo do ve&iacute;culo.</span></p>
<p><span style="font-weight: 400;">- Deve extrair os dados das configura&ccedil;&otilde;es do ve&iacute;culo pelo Modelo/C&oacute;digo de Vendas.</span></p>
<p><span style="font-weight: 400;">- Deve extrair os dados das especifica&ccedil;&otilde;es t&eacute;cnicas pela Descri&ccedil;&atilde;o de Venda.</span></p>
<p><span style="font-weight: 400;">- Deve extrair os dados dos acess&oacute;rios pelo Modelo/C&oacute;digo de Vendas.</span></p>
</td>
</tr>
</tbody>
</table>

---

<table>
<tbody>
<tr>
<td colspan="3">
<a id="E02-US03"></a>
<p><strong>E02-US03</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Extra&ccedil;&atilde;o MEV Onix</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>Gostaria de</strong><span style="font-weight: 400;"> extrair os dados do PDF Manual de Especifica&ccedil;&atilde;o do Ve&iacute;culo (MEV) do modelo de PDF do Onix.</span></p>
<p><strong>Para que</strong><span style="font-weight: 400;"> eu possa visualizar os dados necess&aacute;rios.</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- Deve extrair os dados da(s) tabela(s) com o modelo do ve&iacute;culo.</span></p>
<p><span style="font-weight: 400;">- Deve extrair os dados das configura&ccedil;&otilde;es do ve&iacute;culo pelo Modelo/C&oacute;digo de Vendas.</span></p>
<p><span style="font-weight: 400;">- Deve extrair os dados das especifica&ccedil;&otilde;es t&eacute;cnicas pela Descri&ccedil;&atilde;o de Venda.</span></p>
<p><span style="font-weight: 400;">- Deve extrair os dados dos acess&oacute;rios pelo Modelo/C&oacute;digo de Vendas.</span></p>
</td>
</tr>
</tbody>
</table>

---

<table>
<tbody>
<tr>
<td colspan="3">
<a id="E02-US04"></a>
<p><strong>E02-US04</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Extra&ccedil;&atilde;o MEV Trailblazer</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>Gostaria de</strong><span style="font-weight: 400;"> extrair os dados do PDF Manual de Especifica&ccedil;&atilde;o do Ve&iacute;culo (MEV) do modelo de PDF do Trailblazer.</span></p>
<p><strong>Para que</strong><span style="font-weight: 400;"> eu possa visualizar os dados necess&aacute;rios.</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- Deve extrair os dados da(s) tabela(s) com o modelo do ve&iacute;culo.</span></p>
<p><span style="font-weight: 400;">- Deve extrair os dados das configura&ccedil;&otilde;es do ve&iacute;culo pelo Modelo/C&oacute;digo de Vendas.</span></p>
<p><span style="font-weight: 400;">- Deve extrair os dados das especifica&ccedil;&otilde;es t&eacute;cnicas pela Descri&ccedil;&atilde;o de Venda.</span></p>
<p><span style="font-weight: 400;">- Deve extrair os dados dos acess&oacute;rios pelo Modelo/C&oacute;digo de Vendas.</span></p>
</td>
</tr>
</tbody>
</table>

---

<table>
<tbody>
<tr>
<td colspan="3">
<a id="E02-US05"></a>
<p><strong>E02-US05 </strong><strong>DEPENDENTE (US02, US03 e US04)</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Extra&ccedil;&atilde;o Lista de Pre&ccedil;os</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>Gostaria de</strong><span style="font-weight: 400;"> extrair os dados do PDF Lista de pre&ccedil;os.</span></p>
<p><strong>Para que</strong><span style="font-weight: 400;"> eu possa visualizar os dados necess&aacute;rios.</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- Deve ser acessado o modelo/c&oacute;digo de venda do ve&iacute;culo para encontrar os dados.</span></p>
<p><span style="font-weight: 400;">- Deve ser extra&iacute;do o conte&uacute;do pegando o valor do modelo/c&oacute;digo de venda.</span></p>
</td>
</tr>
</tbody>
</table>

---

<table>
<tbody>
<tr>
<td colspan="3">
<a id="E02-US06"></a>  
<p><strong>E02-US06</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Extra&ccedil;&atilde;o Jeep</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>Gostaria de</strong><span style="font-weight: 400;"> extrair os dados do PDF da Jeep.</span></p>
<p><strong>Para que</strong><span style="font-weight: 400;"> eu possa visualizar os dados necess&aacute;rios.</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- Deve ser extra&iacute;do a tabela com os MVS dos ve&iacute;culos do PDF.</span></p>
<p><span style="font-weight: 400;">- Deve ser extra&iacute;do os dados de cada ve&iacute;culo procurando pela descri&ccedil;&atilde;o.</span></p>
</td>
</tr>
</tbody>
</table>

---

<table>
<tbody>
<tr>
<td colspan="3">
<a id="E03-US01"></a>  
<p><strong>E03-US01</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Visualizar os dados do PDF</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>gostaria de</strong><span style="font-weight: 400;"> visualizar o PDFs extra&iacute;do</span></p>
<p><strong>para que</strong><span style="font-weight: 400;"> eu possa copi&aacute;-lo para o sistema interno (SGS).</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- Deve ser poss&iacute;vel visualizar os dados extra&iacute;dos do PDF.</span></p>
<br />
<p><span style="font-weight: 400;">- Deve ser poss&iacute;vel copiar cada campo individualmente.</span></p>
<br />
<p><span style="font-weight: 400;">- O dado deve ser copiado para a &aacute;rea de transfer&ecirc;ncia do usu&aacute;rio.</span></p>
<br />
<p><span style="font-weight: 400;">- Deve ser poss&iacute;vel visualizar os diferentes modelos do ve&iacute;culo.</span></p>
<br />
<p><span style="font-weight: 400;">- Deve ser poss&iacute;vel visualizar, para cada campo, se ele j&aacute; foi copiado ou n&atilde;o.</span></p>
<br />
<p><span style="font-weight: 400;">- Deve ser poss&iacute;vel visualizar qual foi o &uacute;ltimo campo copiado.</span></p>
<br />
<p><span style="font-weight: 400;">- Deve poder voltar para a p&aacute;gina inicial para enviar outros PDFs.</span></p>
</td>
</tr>
</tbody>
</table>

---

<table>
<tbody>
<tr>
<td colspan="3">
<a id="E03-US02"></a>  
<p><strong>E03-US02</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Lista de PDFs extra&iacute;dos</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>Gostaria de</strong><span style="font-weight: 400;"> visualizar todos os PDFs j&aacute; extra&iacute;dos</span></p>
<p><strong>Para que</strong><span style="font-weight: 400;"> eu possa gerenciar os PDFs que eu j&aacute; extra&iacute;.</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- Visualizar PDF est&aacute; selecionado atualmente.</span></p>
<br />
<p><span style="font-weight: 400;">- Visualizar a lista de PDFs extra&iacute;dos pelas categorias (editores abertos, arquivos incompletos e arquivos completos).</span></p>
<br />
<p><span style="font-weight: 400;">- Visualizar o estado de cada PDF de forma visual (se possui dados faltando, se todos os campos j&aacute; foram copiados ou se ainda faltam campos para copiar).</span></p>
<br />
<p><span style="font-weight: 400;">- Visualizar quando foi feita a &uacute;ltima edi&ccedil;&atilde;o para cada PDF.</span></p>
</td>
</tr>
</tbody>
</table>

---

<table>
<tbody>
<tr>
<td colspan="3">
<a id="E03-US03"></a>  
<p><strong>E03-US03</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Editar os dados de um PDF</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>Gostaria de</strong><span style="font-weight: 400;"> editar os dados de um PDFs j&aacute; extra&iacute;do</span></p>
<p><strong>Para que</strong><span style="font-weight: 400;"> eu possa corrigir dados errados ou antigos.</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- Deve possuir um bot&atilde;o sobre a tela principal para ativar/desativar o modo de edi&ccedil;&atilde;o</span></p>
<br />
<p><span style="font-weight: 400;">- Deve ser poss&iacute;vel editar cada campo individualmente</span></p>
<br />
<p><span style="font-weight: 400;">- Deve ser poss&iacute;vel salvar os campos alterados ao desativar o modo de edi&ccedil;&atilde;o.</span></p>
<br />
<p><span style="font-weight: 400;">- Deve ser alterada a data e hora de quando foi feita a &uacute;ltima edi&ccedil;&atilde;o.</span></p>
</td>
</tr>
</tbody>
</table>

---

<table>
<tbody>
<tr>
<td colspan="3">
<a id="E03-US04"></a>  
<p><strong>E03-US04</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Alterar o status do PDF</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Alta</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>Gostaria de</strong><span style="font-weight: 400;"> ver o status do PDF</span></p>
<p><strong>Para que</strong><span style="font-weight: 400;"> eu possa identificar como est&aacute; indo o envio dos dados para o sistema interno (SGS).</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- Ao copiar um campo novo (que n&atilde;o foi copiado ainda), deve alterar o estado do campo para copiado (campo em azul).</span></p>
<br />
<p><span style="font-weight: 400;">- Ao ir para um pr&oacute;ximo campo, deve atualizar a informa&ccedil;&atilde;o de qual foi o &uacute;ltimo campo copiado.</span></p>
<br />
<p><span style="font-weight: 400;">- Caso todos os campos forem copiados, deve-se atualizar o estado do PDF para &ldquo;completo&rdquo; (&iacute;cone verde) e o PDF deve ser enviado para a categoria de &ldquo;Arquivos completos&rdquo;.</span></p>
<br />
<p><span style="font-weight: 400;">- Por padr&atilde;o, cada PDF extra&iacute;do deve possuir o estado de &ldquo;N&atilde;o aberto&rdquo; at&eacute; ser aberto.</span></p>
<br />
<p><span style="font-weight: 400;">- Ao PDF ser aberto, deve-se atualizar o estado do PDF para "Faltam dados para enviar&rdquo;.</span></p>
</td>
</tr>
</tbody>
</table>

---

<table>
<tbody>
<tr>
<td colspan="3">
<a id="E03-US05"></a>  
<p><strong>E03-US05</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Exportar dados para JSON</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Baixa</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>gostaria de</strong><span style="font-weight: 400;"> extrair os dados dos ve&iacute;culos para o formato JSON</span></p>
<p><strong>para que</strong><span style="font-weight: 400;"> eu possa importar os dados para o sistema SGS.</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- O arquivo JSON deve possuir os mesmos nomes do sistema SGS.</span></p>
<p><span style="font-weight: 400;">- O nome do novo arquivo deve ser o mesmo nome do PDF lido.</span></p>
<p><span style="font-weight: 400;">- A exporta&ccedil;&atilde;o deve ser de todos os ve&iacute;culos do PDF.</span></p>
</td>
</tr>
</tbody>
</table>

---

<table>
<tbody>
<tr>
<td colspan="3">
<a id="E03-US06"></a>  
<p><strong>E03-US06</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>T&iacute;tulo:</strong></p>
<p><span style="font-weight: 400;">Exportar dados para CSV</span></p>
</td>
<td>
<p><strong>Prioridade:</strong></p>
<p><span style="font-weight: 400;">Baixa</span></p>
</td>
<td>
<p><strong>Estimativa:</strong></p>
<p><span style="font-weight: 400;">A definir</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>User Story:</strong></p>
<br />
<p><strong>Eu, como</strong><span style="font-weight: 400;"> usu&aacute;rio,</span><strong>&nbsp;</strong></p>
<p><strong>gostaria de</strong><span style="font-weight: 400;"> extrair os dados dos ve&iacute;culos para o formato CSV</span></p>
<p><strong>para que</strong><span style="font-weight: 400;"> eu possa importar os dados para o sistema SGS.</span></p>
</td>
</tr>
<tr>
<td colspan="3">
<p><strong>Crit&eacute;rios de aceita&ccedil;&atilde;o:</strong></p>
<br />
<p><span style="font-weight: 400;">- O arquivo CSV deve possuir os mesmos nomes do sistema SGS.</span></p>
<p><span style="font-weight: 400;">- O nome do novo arquivo deve ser o mesmo nome do PDF lido.</span></p>
<p><span style="font-weight: 400;">- A exporta&ccedil;&atilde;o deve ser de todos os ve&iacute;culos do PDF.</span></p>
</td>
</tr>
</tbody>
</table>

---



