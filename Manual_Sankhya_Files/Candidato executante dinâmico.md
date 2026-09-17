# Candidato executante dinâmico

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/4405488432663-Candidato-executante-din%C3%A2mico](https://ajuda.sankhya.com.br/hc/pt-br/articles/4405488432663-Candidato-executante-din%C3%A2mico)

---

# Candidato executante dinâmico

A definição de usuários candidatos dinâmicos é determinada através de expressões (scripts) na linguagem JavaScript ou Groovy, de acordo com o contexto do processo, sendo possível utilizar todas as funções de consulta para definir o candidato executante dinâmico, como por exemplo, **"getUsuarioInclusao"**, que irá retornar o usuário solicitante do processo.

 **![dica FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16092145499415)**Todas as funções de consulta estão disponíveis o botão de **"Ajuda"** do campo onde é digitado o script.

Ao definir uma expressão em uma determinada tarefa, no momento em que a instância dela for criada, será executada a expressão, definindo assim a lista de seus usuários candidatos.

Esse recurso deve ser utilizado em processo que os candidatos executantes de uma tarefa são desconhecidos, até o momento em que um determinado fluxo de trabalho ou tarefas anteriores sejam executadas.

![Marcador](https://ajuda.sankhya.com.br/hc/article_attachments/15977988071063) Existe uma rotina no SankhyaFlow que mantém a lista de usuários candidatos sempre atualizada, ou seja, caso uma tarefa esteja sem um responsável (dono) e ocorra uma alteração, como exemplo, a inserção de um novo usuário em um grupo de usuário, ou a alteração do usuário responsável por um determinado Centro de Resultado, no dia seguinte os usuários candidatos dessa tarefa estarão atualizados.

Para demonstrar essa funcionalidade, iremos utilizar como caso de uso o processo de **"Adiantamento de viagens"**, o qual os candidatos de algumas tarefas irão variar em função de um dado preenchimento em um campo do processo e em relação ao usuário que realizou a solicitação:

![floww1.png](https://ajuda.sankhya.com.br/hc/article_attachments/15499504149527)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Processo de Adiantamento de viagens</strong></span></p></td></tr></tbody></table>

Esse processo permite que qualquer colaborador solicite um adiantamento de viagem para seu líder imediato (responsável pelo Centro de Resultado) ou gerente, sendo que o líder aprova valores de até R$1000,00 e acima desse valor, apenas um determinado grupo de gerentes poderá aprovar. Sendo assim, os usuários candidatos da tarefa **"Aprovar adiantamento de viagem"** irão variar em função do valor informado em um determinado campo de um formulário formatado do processo.

Após aprovação do líder/gerente, a solicitação é direcionada ao solicitante (colaborador), para que ele detalhe todos os gastos ocasionados durante a viagem; dessa forma, o candidato da tarefa **"Apontar despesa de viagem"** estará sempre em função do usuário solicitante.

Enfim, a solicitação é direcionada ao departamento financeiro para realizar a análise das despesas e execução da compensação financeira.

---

Abaixo, demonstraremos as configurações necessárias para atender o processo descrito acima, em relação aos usuários candidatos das tarefas mencionadas.

---

Na tela Processos de Negócio, na tarefa **"Aprovar adiantamento de viagem"**, aba **"Usuários Candidatos"**, sub-aba **"Expressão"**, vamos configurar os candidatos dinâmicos dessa tarefa:

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405489619095)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configuração de usuários candidatos dinâmicos</strong></span></p></td></tr></tbody></table>

Conforme o cenário descrito, os usuários candidatos dessa tarefa irão variar conforme o contexto abaixo:

1.  Se o valor do adiantamento solicitado for menor ou igual à R$1.000,00, deve ser encaminhado para o responsável do Centro de Resultado do solicitante realizar a aprovação do adiantamento;
2.  Caso o valor do adiantamento solicitado for maior do que R$1.000,00, deve ser encaminhado para o grupo de usuário Gerência realizar essa aprovação.

As informações serão obtidas através do campo de um formulário formatado que permite único registro:

**Campo:** VALORADIANTAMENTO  
**Formulário:** AD\_SOLICITACAOADIANTAMENTO

Portanto, para que esse cenário ocorra, é necessário escrever o script abaixo contemplando as seguintes informações:

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-justify" style="width: 100%;"><pre><span class="wysiwyg-font-size-small wysiwyg-color-black50"><em><span style="font-weight: 400;">// Obter dados do formulários</span></em></span><br><span class="wysiwyg-font-size-small"><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">formulario</span> <span style="font-weight: 400;">=</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">getLinhasFormulario</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"AD_SOLICITACAOADIANTAMENTO"</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small wysiwyg-color-black50"><em><span style="font-weight: 400;">// Validar existência de conteúdo </span></em></span><br><span class="wysiwyg-font-size-small"><span class="wysiwyg-color-yellow120" style="font-weight: 400;">if</span><span style="font-weight: 400;"> (</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">formulario</span><span style="font-weight: 400;">.length </span><span class="wysiwyg-color-yellow120" style="font-weight: 400;">&gt;</span> <span class="wysiwyg-color-pink110" style="font-weight: 400;">0</span><span style="font-weight: 400;">) {</span></span><br><span class="wysiwyg-font-size-small"><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">valorAdiantamento</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">=</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">formulario</span><span style="font-weight: 400;">[</span><span class="wysiwyg-color-pink110" style="font-weight: 400;">0</span><span style="font-weight: 400;">].</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">getCampo</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"VALORADIANTAMENTO"</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small"><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">usuario</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">=</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">getUsuarioInclusao</span><span style="font-weight: 400;">();</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="wysiwyg-color-black40">&nbsp;</span></span><span class="wysiwyg-color-black50"><em><span style="font-weight: 400;">// Valor do adiantamento menor ou igual a R$1000,00</span></em></span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;"> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span class="wysiwyg-color-yellow120" style="font-weight: 400;">if</span></span><span style="font-weight: 400;"> (</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">valorAdiantamento</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">&lt;= </span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"1000"</span><span style="font-weight: 400;">){</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="wysiwyg-color-black50"><em><span style="font-weight: 400;">// Identificação do usuário responsável pelo centro de resultado do solicitante</span></em></span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">query</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">=</span><span style="font-weight: 400;"> [];</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">params</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">=</span><span style="font-weight: 400;"> [</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">usuario</span><span style="font-weight: 400;">];</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="wysiwyg-color-blue80"><span style="font-weight: 400;">query</span><span style="font-weight: 400;">.</span><span style="font-weight: 400;">push</span></span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">" SELECT "</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="wysiwyg-color-blue80"><span style="font-weight: 400;">query</span><span style="font-weight: 400;">.</span><span style="font-weight: 400;">push</span></span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"&nbsp; &nbsp; CODUSURESP AS COLUNA, "</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="wysiwyg-color-blue80">&nbsp;</span></span><span class="wysiwyg-color-blue80"><span style="font-weight: 400;">query</span><span style="font-weight: 400;">.</span><span style="font-weight: 400;">push</span></span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"&nbsp; &nbsp; 'U' AS TIPO "</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;"> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span class="wysiwyg-color-blue80">query.push</span></span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">" FROM "</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;"> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span class="wysiwyg-color-blue80">query.push</span></span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"&nbsp; &nbsp; TSICUS "</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;"> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span class="wysiwyg-color-blue80">query.push</span></span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">" WHERE CODCENCUS = (SELECT CODCENCUSPAD FROM TSIUSU WHERE CODUSU = :usuario)"</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="wysiwyg-color-yellow120" style="font-weight: 400;">return</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">getLista</span><span style="font-weight: 400;">(<span class="wysiwyg-color-blue80">query</span></span><span style="font-weight: 400;">.</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">join</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">''</span><span style="font-weight: 400;">), </span><span class="wysiwyg-color-blue80" style="font-weight: 400;">params</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small" style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;}</span><br><span class="wysiwyg-font-size-small" style="font-weight: 400;">}</span><br><span class="wysiwyg-font-size-small wysiwyg-color-black50"><em><span style="font-weight: 400;">// Caso a condição acima não for verdadeira, os usuário candidatos será o grupo de usuário = 9</span></em></span><br><span class="wysiwyg-font-size-small"><span class="wysiwyg-color-yellow120" style="font-weight: 400;">return</span> <span class="wysiwyg-color-cyan110" style="font-weight: 400;">"G = 9"</span><span style="font-weight: 400;">;</span></span></pre></td></tr></tbody></table>

**Observação:** existem várias formas de concatenar uma string. Nesse exemplo, estamos utilizando um arranjo de dados. Para identificar o usuário responsável pelo centro de resultado do solicitante, a função **getLista** transforma em uma lista de usuários baseados na query escrita e o **query.join** junta todos os elementos da **query.push** retornando em uma linha.

Será possível retornar mais de um grupo, usuário ou equipe, informando sempre o **"Tipo"** (G, U, E) e **"Valor"** em sequência, conforme o exemplo: return 'G=9,U=10,E=11,U=7'

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405499562135)Na imagem abaixo apresentamos o script configurado na tarefa:

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Script usuários candidatos dinâmicos na tarefa</strong></span></p></td></tr></tbody></table>

Após descrever o script, devemos clicar em **"OK"** e salvar as informações.

Agora iremos configurar o usuário candidato dinâmico na tarefa **"Apontar despesas de viagem"**:

![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405499757335)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configuração de usuários candidatos dinâmicos</strong></span></p></td></tr></tbody></table>

Conforme o contexto do processo, essa tarefa deve ser direcionada sempre ao usuário solicitante; para isso, utilizaremos no script o método abaixo:

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td style="width: 100%;"><pre><span class="wysiwyg-color-yellow120" style="font-weight: 400;">return </span><span class="wysiwyg-color-blue80">getUsuarioInclusao</span><span class="wysiwyg-color-yellow110">()</span></pre></td></tr></tbody></table>

O método acima sempre irá retornar o usuário que realizou a solicitação:

![mceclip3.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405499859863)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Script usuários candidatos dinâmicos na tarefa</strong></span></p></td></tr></tbody></table>

Abaixo, no primeiro exemplo, a colaboradora Juliane realizou uma solicitação de adiantamento no valor de R$2.000,00 (tela [Lista de Tarefas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044595434-Lista-de-Tarefas)):

![floww21.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4405501732375)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Solicitação de Adiantamento de viagem</strong></span></p></td></tr></tbody></table>

Como o valor do adiantamento foi maior do que R$1.000,00, os usuários candidatos da tarefa **"Aprovar adiantamento de viagem"** será o grupo de usuários com o código 9. Alice é uma das candidatas desse grupo para realizar a tarefa; sendo assim, ela é quem realizará a aprovação desse adiantamento:

![mceclip4.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405491090711)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Usuário candidato da tarefa de Aprovar adiantamento de viagem</strong></span></p></td></tr></tbody></table>

Após a aprovação do adiantamento e a baixa do título, a tarefa **"Apontar despesas de viagem"** irá para a colaboradora Juliane realizar as prestações de contas.

Agora, no segundo exemplo o colaborador Luiz realizou uma solicitação de adiantamento de viagem no valor de R$950,00:

![floww22.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4405491245335)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Solicitação de Adiantamento de viagem</strong></span></p></td></tr></tbody></table>

Como o valor do adiantamento foi menor do que R$1.000,00, o usuário candidato da tarefa de **"Aprovar adiantamento de viagem"** é o responsável pelo Centro de Resultado do solicitante. Nesse caso, o colaborador Luiz faz parte do CR do Comercial, o qual o usuário responsável é a Laura.

Sendo assim, Laura realizará a aprovação desse adiantamento:

![mceclip5.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405502380311)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Usuário candidato da tarefa de Aprovar adiantamento de viagem</strong></span></p></td></tr></tbody></table>

Após a aprovação do adiantamento e a baixa do título, a tarefa **"Apontar despesas de viagem"** irá para o colaborador Luiz realizar as prestações de contas.

[\[Voltar ao topo\]](#top)