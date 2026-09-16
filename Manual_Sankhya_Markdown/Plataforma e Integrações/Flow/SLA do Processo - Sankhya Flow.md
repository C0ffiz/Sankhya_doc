# SLA do Processo - Sankhya Flow

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/4409135122583-SLA-do-Processo-Sankhya-Flow](https://ajuda.sankhya.com.br/hc/pt-br/articles/4409135122583-SLA-do-Processo-Sankhya-Flow)

---

# SLA do Processo - Sankhya Flow

Um contrato estabelecido entre duas partes pode envolver uma série de itens, acordos e também prazos de atendimento. Com os prazos estabelecidos no processo, temos então a necessidade de acompanhar em dias ou horas se os prazos estão sendo cumpridos. 

Para esse acompanhamento, baseado nas regras estabelecidas em contrato, existe o recurso do SLA (Acordo de Nível de Serviço) do processo.

O SLA do Processo possibilita estabelecer regras para contagem do prazo. Em uma determinada ação no processo iniciará uma contagem de tempo, como também será possível estabelecer regras para a suspensão da contagem. Assim, uma vez tendo regras acordadas entre fornecedor e cliente, o SLA do Processo fará esse acompanhamento.

Além das regras de contagem e suspensão de prazo, será possível criar alertas de notificações e e-mails em função dos prazos decorridos portanto, se determinado prazo for atingido, os usuários do sistema podem ser alertados.

Nessa documentação trataremos sobre os seguintes temas:

1.  [Caso de Uso](#casodeuso),
2.  [Configurações do SLA do Processo](#configura%C3%A7%C3%B5esdosladoprocesso),
3.  [Demais informações do SLA do Processo](#demaisinforma%C3%A7%C3%B5esdosladoprocesso),
4.  [Inicialização/Continuação e Suspensão - Configurações de Script e Rotina de Banco de Dados](#inicializa%C3%A7%C3%A3o/continua%C3%A7%C3%A3oesuspens%C3%A3o-configura%C3%A7%C3%B5esdescripterotinadebancodedados), e
5.  seus [Status](#status).

---

#### **Caso de Uso**

O processo **"Solicitação de compras"**, exibido na imagem abaixo, foi modelado a fim de atender a proposta de simplificar uma solicitação de compra, tanto para o usuário quanto para automatização do lançamento da solicitação.

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409140270359)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Solicitação de Compras</strong></span></p></td></tr></tbody></table>

O processo possui 3 Tarefas de Usuário: **"Analisar solicitação de compra"**, **"Realizar cotação"** ou **"Refazer Solicitação"**, possui também 2 Tarefas de Serviço para Atualizar e Gerar o pedido e por fim, 2 Tarefas de E-mail para notificação nos cenários de reprovação ou status do pedido.

A partir do momento em que a solicitação é lançada, ou seja, um processo é aberto, o SLA começa a contar. A primeira Tarefa de Usuário é a de Analisar solicitação de compra; nela o gestor responsável analisa a solicitação feita e decide se ela é válida para prosseguir ou se é inválida para ser diretamente cancelada ou refeita na atividade de Refazer Solicitação, na qual o solicitante edita e refaz a solicitação de compra.

**Observação:** quando o processo é direcionado para essa atividade, o SLA é suspenso e somente volta a ser contado quando retorna a atividade de Analisar solicitação de compra.

A Souza Empreendimentos executa uma série de solicitações de compras dos mais variados produtos e para alguns produtos existem fornecedores acordados com prazos de atendimento estabelecidos. Hoje, existem 2 SLA's configurados, sendo um para grupo de produtos de consumo alimentício e o outro produtos de consumo de escritório.

Os itens do grupo alimentício são comprados em eventos para o coffee break e como são perecíveis, o prazo de SLA é mais curto.

Já itens do grupo de escritório são itens de consumo do dia a dia da Empresa, como canetas, borrachas, cadernos, etc. Como são itens comprados em volumes maiores e não possuem data de validade, têm um SLA mais longo.

[\[voltar ao topo\]](#top)

#### **Configurações do SLA do Processo**

Podemos adicionar vários SLA's no mesmo processo (conforme demonstramos abaixo), sendo que, cada um deve seguir regras e alertas diferentes. Para acessar o painel lateral de configurações do processo, basta dar um duplo clique fora do mapeamento do processo e clicar na aba **"SLA"**. Nessa aba podemos adicionar um novo SLA e configurá-lo, editá-lo e também excluí-lo do processo:

![flow13.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4409190621847)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Acessando a configuração do SLA</strong></span></p></td></tr></tbody></table>

Para todo SLA adicionado no processo, será necessário dar um **"Nome"** a ele, informar se seu **"Prazo de solução"** será em **"Dias"** ou **"Horas"** e informar a quantidade de **"Dias ou Horas"**. Também podemos informar qual **"Carga horária"** poderá ser levada em consideração na contagem desse SLA:

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409190682647)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configurando SLA detalhes</strong></span></p></td></tr></tbody></table>

Se o solicitante lançar um produto que esteja no grupo de produtos alimentícios, isso indica que será vigente um SLA de 3 dias para o processo. O modelador do processo deve selecionar o **"Contexto de Processo"**, conforme demonstramos no gif acima, e na configuração do contexto, selecionar a opção por campo de formulário. Nesse caso de uso existem 2 formulários; no caso, o modelador pode selecionar o formulário que contém o campo relacionado ao grupo de produto.

Assim, quando o processo for iniciado com um produto selecionado do grupo alimentício, a contagem de um SLA de 3 dias para o processo passará a contar.

![4.2.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4409195741975)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configurando SLA Contexto de Processo</strong></span></p></td></tr></tbody></table>

Na Tarefa de Usuário Analisar solicitação de compra, o gestor poderá devolver a demanda para o solicitante refazer o pedido, devolvendo os pedidos que forem lançados com algum erro, por exemplo. Então, para esse cenário, o SLA é suspenso já que a solicitação será refeita.

A configuração da Suspensão é semelhante à configuração da Inicialização/Continuação. O modelador acessa a configuração Contexto de Tarefa (conforme abaixo) e seleciona a tarefa onde será analisada a solicitação, e o **"Quando"** será na finalização da tarefa.

![flow14.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4409190864663)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto; height: 22px;"><tbody><tr style="height: 22px;"><td style="width: 100%; height: 22px;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configurando Suspensão SLA Contexto de Tarefa</strong></span></p></td></tr></tbody></table>

**Nota:** a informação de suspensão está contida em um campo de formulário; dessa forma, o modelador terá que fazer essa relação. Assim, quando a atividade Analisar solicitação de compra for finalizada e o campo **"Refazer Solicitação"** for igual a **"Sim"**, será suspensa a contagem do SLA.

---

**Alertas no SLA do Processo**

Para o acompanhamento do SLA, existe a configuração dos **"Alertas"**; nesse caso, os alertas **"No Prazo"** e **"A Vencer"**.

Configurando o status No Prazo, o tipo de **"Contagem"** será mantido em **"Dias"**, a marcação **"Status"** será habilitada pois assim será possível acompanhar a contagem do SLA no card do processo na Lista de Tarefas. Para cada alerta existe um tempo **"Decorrido"** padrão e, nesse caso, manteremos o valor padrão para o alerta No Prazo que é de 50 (relacionado à dias).

Quanto às notificações, elas serão do **"Tipo"** de **"Notificações do Sistema"**, não sendo necessário relacionar uma **"Conta SMTP"**. O **"Destinatário"** deve ter a marcação **"Notificar o dono/candidatos da tarefas"** selecionada, sendo possível também colocar mais destinatários de **"Scripts SQL"**.

Para o status A Vencer, o tipo de Contagem será mantido em Dias e a marcação Status também será mantida ligada para que seja possível acompanhar a contagem do SLA no card da tarefa. No caso do tempo Decorrido, manteremos o valor padrão para o alerta A Vencer que é de 75 (relacionado à dias).

As notificações serão do Tipo **"Ambas"**, sendo necessário relacionar uma Conta SMTP. A marcação Notificar o dono/candidatos de tarefa também deverá ser habilitada e você poderá inserir mais destinatários através de Scripts SQL.

---

**Cards na Lista de Tarefas**

Quando configurados os Alertas, na Lista de Tarefas será apresentado um novo campo, trazendo o **"Prazo do SLA"** no card e também no cabeçalho do formulário da tarefa. As cores que constam na configuração dos Alertas também serão representadas no card.

A imagem abaixo representa um card com o SLA **"Muito Vencido"**:

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409195902871)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto; height: 22px;"><tbody><tr style="height: 22px;"><td style="width: 100%; height: 22px;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Lista de Tarefas</strong></span></p></td></tr></tbody></table>

Outra funcionalidade com o SLA no card é utilizar ele como critério na ordenação na Lista de Tarefas de acordo com o seu **"Vencimento"**, que poderá ser **"Mais próximos primeiro"** ou **"Mais distantes primeiro"**:

![flow15.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4409196090263)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto; height: 22px;"><tbody><tr style="height: 22px;"><td style="width: 100%; height: 22px;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configurando ordenação dos cards</strong></span></p></td></tr></tbody></table>

---

**Notificações dos Alertas**

Podemos configurar o Alerta de SLA para enviar tanto uma notificação quanto um e-mail para o dono da atividade. As notificações aparecem no ícone de notificação geral do sistema conforme imagem abaixo:

![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409196195095)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto; height: 22px;"><tbody><tr style="height: 22px;"><td style="width: 100%; height: 22px;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Notificação no sistema</strong></span></p></td></tr></tbody></table>

E também no texto do e-mail:

![mceclip3.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409191633047)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto; height: 22px;"><tbody><tr style="height: 22px;"><td style="width: 100%; height: 22px;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Notificação por e-mail</strong></span></p></td></tr></tbody></table>

[\[voltar ao topo\]](#top)

#### **Demais informações do SLA do Processo**

**Inicialização / Continuação - Alteração de Formulário**

Nessa configuração, você pode estabelecer que uma alteração em um campo qualquer de um formulário qualquer que esteja no processo (independente do ponto em que ele esteja), seja iniciada ou continuada uma contagem do SLA.

---

**Inicialização / Continuação - Contexto de Tarefa**

Aqui você pode estabelecer que uma Tarefa de Usuário inicie ou continue a contagem do SLA. Os momentos disponíveis para esse contexto são: **"Ao atribuir dono"**, **"Ao desatribuir dono"**, **"Ao criar tarefa"** e **"Ao finalizar tarefa"**.

---

**Suspensão - Alteração de Formulário**

Por fim, nessa configuração você estabelece que uma alteração em um campo qualquer de um formulário que esteja no processo (independente do ponto em que ele esteja) possa ser suspensa uma contagem do SLA que está sendo executada.

[\[voltar ao topo\]](#top)

#### **Inicialização/Continuação e Suspensão - Configurações de Script e Rotina de Banco de Dados**

No [Caso de Uso](#casodeuso) vimos a configuração do SLA do Processo através de campos do formulário, mas existem outras 2 possibilidades de configuração para Inicialização/Continuação do SLA do Processo e Suspensão.

Também é possível combinar scripts, rotinas de banco e campos de formulários com os operadores lógicos **"E"** e/ou **"OU"**, para que essa combinação retorne ao final um valor verdadeiro para iniciar/continuar o SLA do Processo ou realizar sua suspensão.

Através de scripts na linguagem JavaScript ou Groovy estabelecemos regras para a Inicialização/Continuação ou Suspensão; o script deverá retornar verdadeiro ou falso. As funções disponíveis para uso podem ser consultadas no help.

No gif abaixo temos a demonstração de utilização de script na configuração de um SLA do Contexto de Processo:

![flow12.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4409190577303)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto; height: 22px;"><tbody><tr style="height: 22px;"><td style="width: 100%; height: 22px;"><p class="wysiwyg-text-align-center"><strong><span class="wysiwyg-font-size-small wysiwyg-color-black30">Configurando SLA do Contexto de Processo por Script</span></strong></p></td></tr></tbody></table>

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre class="wysiwyg-text-align-justify"><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">var </span></span><span class="wysiwyg-font-size-medium wysiwyg-color-blue70">grupo</span><span class="wysiwyg-font-size-medium wysiwyg-color-yellow110"> = </span><span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium">getLinhasFormulario</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">(</span></span><span class="wysiwyg-color-cyan110"><span class="wysiwyg-font-size-medium">"AD_SOLICITACAOCOMPRA"</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">);<br></span></span><span class="wysiwyg-color-yellow120"><span class="wysiwyg-font-size-medium">if</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black"> (<span class="wysiwyg-font-size-medium wysiwyg-color-blue70">grupo</span>.</span></span><span class="wysiwyg-color-yellow110"><span class="wysiwyg-font-size-medium">length</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black"> &gt; <span class="wysiwyg-color-pink110"><span class="wysiwyg-font-size-medium">0</span></span>){<br>var </span></span><span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium">Codgrupo </span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black"><span class="wysiwyg-font-size-medium wysiwyg-color-yellow110">=</span> <span class="wysiwyg-font-size-medium wysiwyg-color-blue70">grupo</span>[</span></span><span class="wysiwyg-color-pink110"><span class="wysiwyg-font-size-medium">0</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">].</span></span><span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium">getCampo</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">(</span></span><span class="wysiwyg-color-cyan110"><span class="wysiwyg-font-size-medium">"CODGRUPOPROD"</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">);<br><span class="wysiwyg-color-yellow120"><span class="wysiwyg-font-size-medium">if</span></span> (<span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium">Codgrupo</span></span> <span class="wysiwyg-font-size-medium wysiwyg-color-yellow110">==</span> </span></span><span class="wysiwyg-color-pink110"><span class="wysiwyg-font-size-medium">1000000</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">) {<br></span></span><span class="wysiwyg-color-yellow110"><span class="wysiwyg-font-size-medium">return true</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">;<br>}<br>} <br></span></span><span class="wysiwyg-color-yellow110"><span class="wysiwyg-font-size-medium">return false</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">;<br></span></span></pre></td></tr></tbody></table>

**Observação:** também é possível criar uma rotina de banco de dados no padrão procedure do Sankhya Om. Então, dentro da rotina do banco de dados, você deve retornar um resultado **"N"**, caso a condição testada seja falsa ou **"S"** se a condição for verdadeira.

[\[voltar ao topo\]](#top)

#### **Status**

Para todo SLA do Processo é possível estabelecer Alertas diferentes, em diferentes níveis te tempo. Eles estão segmentados da seguinte forma:

*   **Início do Prazo:** Tempo decorrido 0, cor **azul**;
*   **No Prazo:** Tempo decorrido 50, cor **verde**;
*   **A Vencer:** Tempo decorrido 75, cor **amarela**;
*   **Vencido:** Tempo decorrido 100, cor **vermelha**;
*   **Muito Vencido:** Tempo decorrido 110, cor **preta**.

O tempo Decorrido pode ser ajustado para outros valores caso o modelador queira. Os Alertas possuem os seguintes campos:

No campo **"Contagem"** é informado se a contagem será em **"Percentual"**, **"Dias"** ou **"Horas"**.

Se a marcação **"Status"** estiver ligada, as informações de tempo consumido do SLA estarão no card do processo na Lista de Tarefas e no cabeçalho do formulário.

O campo **"Tipo"** refere-se aos tipos de notificações que o sistema irá emitir, sendo eles: **"E-mail"**, **"Notificações do Sistema"**, **"Ambas"** ou **"Nenhuma"**.

Caso seja selecionado o Tipo de Notificação de E-mail ou Ambas, será necessário informar a **"Conta SMTP"** para o disparo do e-mail.

Se a marcação **"Notificar o dono/candidato da tarefa"** estiver selecionada, fará com que os usuários candidatos/dono da tarefa sejam notificados.

Por fim, será possível escrever uma consulta no campo **"Script SQL"** que retorne o e-mail do usuário para ele receber a notificação de alerta do SLA.

[\[voltar ao topo\]](#top)