# Eventos de Processo e Eventos de Tarefa

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/4406903288855-Eventos-de-Processo-e-Eventos-de-Tarefa](https://ajuda.sankhya.com.br/hc/pt-br/articles/4406903288855-Eventos-de-Processo-e-Eventos-de-Tarefa)

---

# Eventos de Processo e Eventos de Tarefa

![Versão - 32x32 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313294125463) **Versão:** a partir da 4.6

---

O Evento tem o poder de definir um script associado a um determinado cenário, ou seja, quando algo acontecer em uma Tarefa de Usuário ou no Processo, podemos definir que um script seja executado. Diferentemente da Tarefa de Serviço que é possível modelar de forma independente e em qualquer ponto do fluxo de processo, os Eventos são obrigatoriamente relacionados a acontecimentos na utilização do processo. 

Quando os Eventos são configurados, poderão auxiliar desde automação até integrações com outros módulos Sankhya e outros sistemas ao longo do processo. Ele permite scripts em várias linguagens, definidos para executar em vários pontos ou contextos de Processo e de Tarefa de Usuário, como por exemplo, quando for inserido um apontamento em uma tarefa, um Evento poderá disparar uma notificação a um determinado grupo de usuários.

Um outro exemplo é o processo de **"Manutenção de Equipamentos"**, onde o modelador poderá definir que na finalização da tarefa **"Realizar Manutenção"**, um script execute e faça a baixa do produto utilizado na manutenção, sem a necessidade do usuário ter que sair do processo e acessar uma outra tela para fazer essa baixa manualmente. 

Nessa documentação, trataremos sobre os seguintes tópicos:

---

1.  [Caso de Uso](#casodeuso)                                                                       
2.  [Configurando os Eventos](#configurandooseventos)
3.  [Resultados](#resultados)
4.  [Demais Eventos disponíveis no contexto de Processo](#demaiseventosdispon%C3%ADveisnocontextodeprocesso)
5.  [Demais Eventos disponíveis no contexto de Tarefas](#demaiseventosdispon%C3%ADveisnocontextodetarefas)

---

#### **Caso de Uso**

O processo **"Solicitação de Compras"** exibido na imagem abaixo, foi modelado a fim de atender a proposta de simplificar uma solicitação de compra, tanto para o usuário quanto para automatização do lançamento da solicitação.

![flow.png](https://ajuda.sankhya.com.br/hc/article_attachments/4406994313239)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Solicitação de Compras</strong></span></p></td></tr></tbody></table>

O processo possui 3 Tarefas de Usuário: **"Analisar a Solicitação"**, **"Realizar cotação"** e **"Refazer Solicitação"**, possui 1 Tarefa de Serviço, que é a **"Geração de pedido de compras"** e por fim, possui também 2 Tarefas de E-mail para notificação dos cenários de reprovação ou status do pedido.

Na Tarefa de Usuário Realizar Cotação existe a necessidade de enviar um e-mail no exato momento em que o responsável por essa tarefa começa a trabalhar nela. O intuito é de avisar em tempo real o andamento da compra para o solicitante do processo.

A Tarefa de Serviço Geração de pedido de compras é responsável por gerar o pedido na Central de Compras; para isso, são obrigatórias algumas informações da empresa que está emitindo o pedido, como por exemplo: Tipo de Operação, Tipo de Negociação, Natureza e etc. A fim de facilitar o ajuste dessas informações para se adequar a qualquer empresa que queira utilizar o processo, esses parâmetros não são contemplados na implementação da Tarefa de Serviço pois, como são informações relacionadas a cada pedido de venda gerado, elas precisam constar no contexto de processo.

[\[voltar ao topo\]](#top)

#### **Configurando os Eventos**

Para a necessidade de definição dos parâmetros para gerar o pedido de compras, utilizamos o recurso de Evento na inicialização do Processo.

Para acessar a aba Eventos no contexto de Processo, basta dar um duplo clique em qualquer área branca do fluxograma; com isso, o painel lateral à direita se abrirá na tela.

Nesse painel, temos a aba **"Eventos"**. Posicionada nela, clique no botão ![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4407022203671) para abrir o pop-up **"Configuração de Evento"** para adicionar um novo Evento:

![flow3.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4407022480279)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configuração de Evento</strong></span></p></td></tr></tbody></table>

Com o pop-up aberto, podemos adicionar um novo Evento e também podemos editar os que já estiverem cadastrados no processo. Primeiramente, iremos inserir o **"Nome do Evento"** que será Parâmetros da Empresa.

O campo **"Onde"** é de multisseleção e indica o momento em que o Evento vai acontecer. Nesse ponto, temos as opções de Processo, Formulário Embarcado e Formulário Formatado. Conforme as regras de negócio descritas no [Caso de Uso](#casodeuso), utilizaremos a opção Processo.

Ao selecionar que o campo Onde será no contexto de Processo, precisamos definir a **"Ação"**. Nesse campo, temos as opções **"Iniciar"** e **"Finalização"**, ambas relacionadas ao Processo. Em nosso caso, iremos utilizar a opção Iniciar. Assim, com esses dois campos definimos o exato momento em que o script será executado.

Os scripts podem ser escritos em **"Java"**, **"JavaScript"** ou **"Procedure"**, bastando que você sinalize qual desses será o script dentro da Configuração de Evento. Para o nosso caso de uso iremos utilizar um script em JavaScript. Abaixo demonstramos como definir a linguagem a ser utilizada no script e, logo em seguida, o script do Evento:

![flow2.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4407022349079)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Definindo a linguagem do Script</strong></span></p></td></tr></tbody></table>

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre class="wysiwyg-text-align-justify"><span class="wysiwyg-color-black50" style="font-weight: 400;"><em>//Dados a serem alterados para adequar a realidade da empresa que utilizará </em><br><em>o processo de Solicitação de Compras no SankhyaFlow</em> </span><br><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">data</span> <span class="wysiwyg-color-yellow120"><span style="font-weight: 400;">=</span> <span style="font-weight: 400;">new</span> <span style="font-weight: 400;">Date</span></span><span style="font-weight: 400;">();&nbsp; </span><br><span class="wysiwyg-color-blue80" style="font-weight: 400;">setCampo</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"CODEMP"</span><span style="font-weight: 400;">, </span><span class="wysiwyg-color-pink110" style="font-weight: 400;">1</span><span style="font-weight: 400;">); </span><span style="font-weight: 400;">//Código da empresa </span><br><span style="font-weight: 400;"><span class="wysiwyg-color-blue80" style="font-weight: 400;">setCampo</span>(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"CODTIPOPER"</span><span style="font-weight: 400;">, </span><span class="wysiwyg-color-pink110" style="font-weight: 400;">7</span><span style="font-weight: 400;">); </span><span style="font-weight: 400;">//Tipo de Operação </span><br><span style="font-weight: 400;"><span class="wysiwyg-color-blue80" style="font-weight: 400;">setCampo</span>(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"CODTIPVENDA"</span><span style="font-weight: 400;">, </span><span class="wysiwyg-color-pink110" style="font-weight: 400;">5</span><span style="font-weight: 400;">);&nbsp; </span><span style="font-weight: 400;">//Tipo de Negociação </span><br><span style="font-weight: 400;"><span class="wysiwyg-color-blue80" style="font-weight: 400;">setCampo</span>(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"CODNAT"</span><span style="font-weight: 400;">, </span><span class="wysiwyg-color-pink110" style="font-weight: 400;">3020600</span><span style="font-weight: 400;">); </span><span style="font-weight: 400;">//Natureza </span><br><span style="font-weight: 400;"><span class="wysiwyg-color-blue80" style="font-weight: 400;">setCampo</span>(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"CODCENCUS"</span><span style="font-weight: 400;">, </span><span class="wysiwyg-color-pink110" style="font-weight: 400;">10300</span><span style="font-weight: 400;">);&nbsp; </span><span style="font-weight: 400;">//Centro de Resultado </span><br><span style="font-weight: 400;"><span class="wysiwyg-color-blue80" style="font-weight: 400;">setCampo</span>(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"DTNEG"</span><span style="font-weight: 400;">,</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">''</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">+</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">data</span><span style="font-weight: 400;">.</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">getDate</span><span style="font-weight: 400;">() <span class="wysiwyg-color-yellow120" style="font-weight: 400;">+</span></span> <span class="wysiwyg-color-cyan110" style="font-weight: 400;">'/'</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">+</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">data</span><span style="font-weight: 400;">.</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">getMonth</span><span style="font-weight: 400;">() <span class="wysiwyg-color-yellow120" style="font-weight: 400;">+</span></span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">'/'</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">+</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">data</span><span style="font-weight: 400;">.</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">getFullYear</span><span style="font-weight: 400;">());&nbsp;</span></pre></td></tr></tbody></table>

Após a inserção do script, basta salvar; assim, o Evento já estará definido e contendo o script necessário para poder gerar o pedido de compras. Note que, depois de adicionado o Evento, é possível ler as definições dele, bastando abrir o painel lateral do Processo na aba Eventos:

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4407013725463)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Painel de controle dos Eventos</strong></span></p></td></tr></tbody></table>

Para a necessidade de enviar um e-mail no instante em que for atribuída a tarefa de **"Realizar Cotação"**, utilizamos o recurso de Evento na Atribuição/Desatribuição da Tarefa. No campo Ação, temos as opções **"Atribuição/Desatribuição"**, **"Criação"** e **"Finalização"**, todas relacionadas à Tarefa em que o Evento está sendo definido.

Para acessar a aba Eventos no contexto de Tarefa, dê um duplo clique na atividade Realizar Cotação para que seja aberto o painel lateral. Clicando no botão , teremos acesso ao pop-up Configuração de Evento para adicionar um novo Evento.

Primeiramente, devemos inserir o Nome do Evento que será Envio de E-mail. O campo Onde indica onde o Evento vai acontecer; portanto, em nosso cenário, queremos que o Evento aconteça na Tarefa e a Ação seja de Atribuição/Desatribuição.

Com esses dois campos temos então definido o exato momento em que o script será executado. O Onde na tarefa Realizar Cotação em junção da Ação que será no ato de atribuir a tarefa.

Novamente, escrevemos o script do Evento em JavaScript:

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre class="wysiwyg-text-align-justify"><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">emailSolicitante</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">=</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">getEmailSolicitante</span><span style="font-weight: 400;">;</span><br><span class="wysiwyg-color-blue80" style="font-weight: 400;">eMail</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"Cotação foi iniciada"</span><span style="font-weight: 400;">, </span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"Sua cotação esta sendo realizada e logo mais teremos um resultado"</span><span style="font-weight: 400;">, <br></span><span style="font-weight: 400;"><span class="wysiwyg-color-blue80" style="font-weight: 400;">emailSolicitante</span>);</span></pre></td></tr></tbody></table>

Após a inserção do script, basta salvar. Dessa forma, o Evento já está definido e contendo o script necessário para poder enviar o e-mail ao solicitante. Note que, depois de adicionado o Evento, será possível ler as definições acessando a tarefa a qual foi definido o Evento:

![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/4407023032215)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Painel de controle dos Eventos</strong></span></p></td></tr></tbody></table>

[\[voltar ao topo\]](#top)

#### **Resultados**

O processo **"Pedido de Compras"** foi iniciado e para isso é necessário o preenchimento de 3 campos: **"Produto"**, **"Quantidade"** e **"Observação"**:

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4407006592279)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Lançamento do Pedido</strong></span></p></td></tr></tbody></table>

Após o pedido lançado, o processo passa pela atividade **"Realizar Cotação"** e quando a cotação é finalizada, o pedido então é gerado na Central de Compras, contendo todas as informações necessárias para gerar o pedido e que foi escrito no script contido no Evento que descrevemos no tópico [Configurando os Eventos](#configurandooseventos).

Quando o processo chega na tarefa Realizar Cotação e ela é atribuída, o Evento descrito no tópico [Configurando os Eventos](#configurandooseventos) entra em ação e envia um e-mail ao solicitante que fez a abertura do processo. Podemos conferir na imagem abaixo o e-mail recebido:

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4407000131991)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>E-mail do evento da tarefa "Realizar Cotação"</strong></span></p></td></tr></tbody></table>

[\[voltar ao topo\]](#top)

#### **Demais Eventos disponíveis no contexto de Processo**

Os conceitos que definem um Evento são as junções de momentos e ações que indicam ou não a execução de um script escrito pelo modelador. O modelador pode definir vários Eventos, editar, excluir e incluir no contexto de Processo.

Para todo Evento adicionado, é necessário escrever o **"Nome do Evento"**. Além dele, existem de 3 a 5 campos obrigatórios e que, sequencialmente, devem ser preenchidos de acordo com a regra de negócio do Evento, são eles:

**1- Onde:**

*   **Formulário Embarcado:** O momento será relacionado a qualquer campo do Formulário Formatado contido no processo e, para esse apontamento, existe a ação **"Salvar"** a ser definida; ao salvar um campo de qualquer Formulário Formatado, o Evento é disparado.
*   **Formulário Formatado:** O momento será relacionado diretamente a um Formulário Formatado contido na Tarefa onde o Evento está sendo definido. Para o Formulário Formatado existem as seguintes ações:

**Excluir:** Na exclusão de um Formulário Formatado o Evento é disparado.

**Incluir:** Na inclusão de um Formulário Formatado o Evento é disparado.

**Alterar:** Na alteração de um Formulário Formatado o Evento é disparado.

**Observação:** é necessário definir o **"Quando"**, sendo **"Antes"** ou **"Depois"** da ação e por fim, selecionar qual Formulário Formatado está relacionado à essa configuração de Evento no campo **"Formulário"**.

**2- Tipo de Rotina:**

*   **Java:** Para essa rotina é necessário vincular um arquivo _.jar_ na tela [Módulo Java](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110573-M%C3%B3dulo-Java) e, posteriormente, associar o módulo java ao Evento. Assim, o modelador pode escrever scripts simples e até mais completos, como por exemplo, um que utiliza WebService, chamando um serviço externo qualquer.
    
*   **Banco de Dados:** Também é possível criar uma rotina de banco de dados no padrão procedure do Sankhya Om. Então, dentro da rotina do banco de dados, teremos que retornar um resultado **'N'** caso a condição testada seja falsa, ou **'S'** se a condição for verdadeira.
    

[\[voltar ao topo\]](#top)

#### **Demais Eventos disponíveis no contexto de Tarefas**

Os conceitos que definem um Evento são as junções de momentos e ações que indicam ou não a execução de um script escrito pelo modelador. O modelador pode definir vários Eventos, editar, excluir e incluir no contexto de Tarefa.

Para todo Evento adicionado, é necessário escrever o **"Nome do Evento"**. Além dele, existem de 3 a 5 campos obrigatórios e que, sequencialmente, devem ser preenchidos, são eles:

**1- Onde:**

*   **Apontamento:** O momento será relacionado aos apontamentos na Tarefa onde o Evento está sendo definido e, para esse apontamento existem as seguintes ações a serem definidas:

**Excluir:** Na exclusão de um apontamento o Evento é disparado.

**Incluir:** Na inclusão de um apontamento o Evento é disparado.

**Pausar:** Na pausa de um apontamento o Evento é disparado.

**Iniciar:** Na inicialização de um apontamento o Evento é disparado.

**Alterar:** Na alteração de um apontamento o Evento é disparado.

**Nota:** é necessário definir também o **"Quando"**, sendo **"Antes"** ou **"Depois"** da ação.

*   **Formulário Embarcado:** O momento será relacionado a qualquer campo do Formulário Embarcado contido no processo e, para esse apontamento, existe a ação **"Salvar"** a ser definida; assim, ao salvar um campo de qualquer Formulário Formatado o Evento é disparado.
*   **Formulário Formatado:** O momento será relacionado diretamente a um Formulário Formatado contido na Tarefa onde o Evento está sendo definido. Para o Formulário Formatado existem as seguintes ações:

**Excluir:** Na exclusão de um Formulário Formatado o Evento é disparado.

**Incluir:** Na inclusão de um Formulário Formatado o Evento é disparado.

**Alterar:** Na alteração de um Formulário Formatado o Evento é disparado.

**Observação:** é necessário definir o **"Quando"**, sendo **"Antes"** ou **"Depois"** da ação e por fim, selecionar qual Formulário Formatado está relacionado à essa configuração de Evento no campo **"Formulário"**.

**2- Tipo de Rotina:**

*   **Java:** Para essa rotina é necessário vincular um arquivo _.jar_ na tela [Módulo Java](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110573-M%C3%B3dulo-Java) e, posteriormente, associar o módulo java ao Evento. Assim, o modelador pode escrever scripts simples e até mais completos, como por exemplo, um que utiliza WebService, chamando um serviço externo qualquer.
    
*   **Banco de Dados:** Também é possível criar uma rotina de banco de dados no padrão procedure do Sankhya Om. Então, dentro da rotina do banco de dados, teremos que retornar um resultado **'N'** caso a condição testada seja falsa, ou **'S'** se a condição for verdadeira.
    

[\[voltar ao topo\]](#top)