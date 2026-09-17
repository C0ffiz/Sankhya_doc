# Direcionadores de fluxo (Gateway)

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/4405298798103-Direcionadores-de-fluxo-Gateway](https://ajuda.sankhya.com.br/hc/pt-br/articles/4405298798103-Direcionadores-de-fluxo-Gateway)

---

# Direcionadores de fluxo (Gateway)

Os Gateways são elementos que determinam o caminho que o processo seguirá, definindo ramificações, bifurcações e união de caminhos, por meio dos Gateways Paralelo, Exclusivo e Inclusivo.

Nessa documentação, trataremos sobre os seguintes tópicos:

---

1.  [Gateways](#gateways)
2.  [Casos de Uso](#casosdeuso)                                                                       
3.  [Configurando Gateways no Processo](#Configurandogatewaysnoprocesso)

---

#### **Gateways**

Nesse tópico falaremos sobre cada um dos Gateways: [Paralelo](#paralelo), [Exclusivo](#exclusivo) e [Inclusivo](#inclusivo).

**Paralelo**

Esse gateway representa a divisão de um fluxo em 2 ou mais caminhos que serão executados paralelamente, ou seja, todos os caminhos de saída são executados simultaneamente.

Ele é utilizado também como junção; nesse caso, o fluxo de execução será percorrido apenas quando todos os seus fluxos de entrada forem percorridos.

![floww4.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405304270615)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 42.285%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Ícone Gateway Paralelo</strong></span></p></td></tr></tbody></table>

[\[voltar ao subtítulo\]](#gateways) [\[voltar ao topo\]](#top)

---

**Exclusivo**

O gateway exclusivo é utilizado em um processo onde vários caminhos são possíveis porém, de acordo com as condições, apenas um deles será percorrido. Assim, deverá existir sempre 2 ou mais fluxos de saídas, sendo que um desses fluxos pode ser um caminho padrão, que será executado apenas se todos os outros fluxos não forem verdadeiros no tempo de execução. Ele é representado por um fluxo sequencial com uma barra diagonal:

![floww5.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405299425943)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 42.285%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Fluxo de sequência padrão</strong></span></p></td></tr></tbody></table>

Ou seja, a primeira condição (script) que for avaliada como verdadeira (true) irá determinar o fluxo a ser seguido, e se por acaso todas as condições dos fluxos retornarem falso (false), o fluxo padrão terá sequência.

Esse gateway também pode unificar fluxos distintos em uma única sequência de atividades, sendo que a primeira sequência que chegar dará continuidade no fluxo do processo.

![floww6.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405299484183)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 42.285%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Ícone Gateway Exclusivo</strong></span></p></td></tr></tbody></table>

[\[voltar ao subtítulo\]](#gateways) [\[voltar ao topo\]](#top)

---

**Inclusivo**

Esse gateway será utilizado em pontos do processo onde vários caminhos de continuidade são possíveis, desde que sua condição seja verdadeira. Sendo assim, sempre deverá ter 2 ou mais fluxos de saídas.

A execução do processo pode ser dividida em inúmeros fluxos paralelos e todos os fluxos que retornarem com a condição (script) verdadeira serão executados. Também pode ser definido um caminho padrão que será percorrido caso nenhuma das condições forem verdadeiras.

O gateway inclusivo permite também unificar o fluxo de execução, ou seja, a continuidade do processo acontecerá apenas quando todos os fluxos de saída de um gateway inclusivo tiver sido percorrido.

![floww7.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405299585175)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 42.285%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Ícone Gateway Inclusivo</strong></span></p></td></tr></tbody></table>

[\[voltar ao subtítulo\]](#gateways) [\[voltar ao topo\]](#top)

#### **Casos de Uso**

Nesse tópico, trouxemos um caso de uso para cada tipo de Gateway. Para verificar sobre, clique nos link's abaixo:

[Gateway Paralelo](#gatewayparalelo)                              [Gateway Exclusivo](#gatewayexclusivo)                              [Gateway Inclusivo](#gatewayinclusivo)

---

**Gateway Paralelo**

![floww8.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405304951063)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Processo utilizando Gateway Paralelo</strong></span></p></td></tr></tbody></table>

Nesse exemplo, serão executados paralelamente 2 fluxos (representado pelo primeiro gateway). Enquanto a **"Tarefa 2"** é realizada, a **"Tarefa 3"** também poderá ser executada. O segundo gateway faz a junção dos fluxos, garantindo que a **"Tarefa 4"** só seja realizada depois que as Tarefas 2 e 3 tiverem sido finalizadas.

**Observação:** os gateways são utilizados de maneira independente, ou seja, não precisa utilizar um gateway de junção ou os dois juntos.

[\[voltar ao subtítulo\]](#casosdeuso) [\[voltar ao topo\]](#top)

---

**Gateway Exclusivo**

O processo abaixo permite que um colaborador realize uma solicitação de Adiantamento de viagens para seu líder:

![floww9.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405305033239)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Processo utilizando Gateway Exclusivo</strong></span></p></td></tr></tbody></table>

No exemplo acima, o primeiro gateway verifica o resultado da tarefa **"Aprovar adiantamento de viagem"**; se na execução dessa tarefa o líder aprovar o adiantamento, o fluxo seguirá pela sequência de saída padrão **"Registrar títulos de adiantamento"** e se o adiantamento for reprovado, o fluxo seguirá pelo caminho **"Notificar o solicitante"**.

![Marcador 2 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16092447985559) Uma boa prática no SankhyaFlow é utilizar o Gateway Exclusivo também quando uma determinada tarefa tiver várias entradas, pois na tarefa é possível ter apenas um evento de entrada.

Nesse mesmo exemplo, utilizamos o Gateway Exclusivo para dar sequência nos 2 fluxos criados, onde ambos serão direcionados para a mesma tarefa Notificar solicitante, conforme a execução do fluxo.

[\[voltar ao subtítulo\]](#casosdeuso) [\[voltar ao topo\]](#top)

---

**Gateway Inclusivo**

No caso abaixo, o primeiro gateway verifica o resultado da atividade **"Avaliar documentação"**; se na execução dessa atividade for identificada a necessidade de ter que digitalizar a documentação e/ou validar a autenticidade desses documentos, cada fluxo será executado. Caso esteja tudo certo com a documentação, o fluxo seguirá o caminho padrão.

![floww10.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405305272343)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Processo utilizando Gateway Inclusivo</strong></span></p></td></tr></tbody></table>

Aqui, o Gateway Inclusivo foi utilizado para unir os fluxos criados. Isso garante que a atividade **"Notificar partes envolvidas"** só seja iniciada depois que todos os fluxos que forem iniciados pelo gateway anterior sejam executados.

![Marcador 2 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16092447985559) Os gateways são utilizados de maneira independente, ou seja, não precisa utilizar um gateway de junção ou então os dois juntos.

[\[voltar ao subtítulo\]](#casosdeuso) [\[voltar ao topo\]](#top)

#### **Configurando Gateways no Processo**

Ao selecionar uma tarefa do processo na tela Processos de Negócio, será exibida uma caixa com várias opções. Dentre elas, selecione o ícone **"Adicionar Gateway"** ![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405311975959) ou busque esse elemento dentro da paleta localizada ao lado esquerdo:

![floww11.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4405312002711)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Adicionando Gateways</strong></span></p></td></tr></tbody></table>

Por padrão, é apresentado o Gateway Exclusivo; para alterar o tipo, basta clicar no ícone **"Alterar tipo"** ![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405306267543) e selecionar o que você desejar:

![floww12.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4405306343959)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Alteração do tipo de Gateways</strong></span></p></td></tr></tbody></table>

Para configurar um Gateway Paralelo, basta inseri-lo no processo e dar sequência na modelagem de cada caminho que deverá ser percorrido. Para configurar esse elemento como junção, o gateway deve receber as entradas dos caminhos do Gateway Paralelo anterior:

![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405312065175)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Modelagem do Processo com Gateway Paralelo</strong></span></p></td></tr></tbody></table>

Na configuração do Gateway Exclusivo, é necessário inserir uma condição no fluxo sequencial para que o caminho seja executado conforme os dados inseridos na tarefa anterior. Quando o caminho for definido como fluxo padrão, não é necessário inserir um script.

Você pode realizar a configuração de um gateway exclusivo, de duas formas: Modo assistente e Modo avançado.

---

**Modo assistente**

Essa opção é viável para auxiliar o usuário que está realizando a modelagem do processo e não possui conhecimento em criação de script (Groovy ou JavaScript).

Para definir uma condição, utilizando o Modo Assistente, no caminho que não é padrão, é necessário clicar sobre o fluxo sequencial, onde será apresentado na aba Geral o botão **"Abrir configurador de condições"**. 

![unnamed.png](https://ajuda.sankhya.com.br/hc/article_attachments/5567336333207)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configurador de condições<br></strong></span></p></td></tr></tbody></table>

Ao abrir o configurador de condições, o usuário deverá selecionar no **"****Modo de construção"** a opção **"Assistente"**. 

![unnamed\_\_1\_\_\_1\_.png](https://ajuda.sankhya.com.br/hc/article_attachments/5575163794967)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Modo de construção - Assistente</strong></span></p></td></tr></tbody></table>

Nesse exemplo, iremos realizar uma configuração utilizando o Modo assistente para buscar os dados de um campo do formulário formatado, na situação em que a solicitação do adiantamento seja reprovada. Para que este cenário ocorra é necessário seguir os passos abaixo:

 ![Marcador 2 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16092447985559) O exemplo abaixo é referente ao processo de Adiantamento de viagens, no gateway Aprovação de adiantamento. Para realizar um teste, procure na base utilizada um processo correspondente.

**Campo**: SITUACAO

**Formulário**: AD\_SOLICITACAOADIANTAMENTO

Com o campo Modo de construção indicado com a opção Assistente, clique em **"Formulário****s"**, opção **"****Formatado"** e selecione o formulário formatado **"****AD\_SOLICITACAOADIANTAMENTO"**. Feito isso, selecione a opção **"****SITUACAO"**, em seguida escolha o operador lógico **"****Igual(=)"** e indique a opção **"****Reprovado"** . Para finalizar clique em **"OK"**.

![condi\_ao\_gateway.gif](https://ajuda.sankhya.com.br/hc/article_attachments/5576907772055)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configurando uma condição no modo assistente<br></strong></span></p></td></tr></tbody></table>

---

**Modo avançado**

Essa opção é viável para o usuário que está realizando a modelagem do processo e possui conhecimento em criação de script (Groovy ou JavaScript).

Para definir uma condição script - Modo Avançado no caminho que não é padrão, é necessário clicar sobre o fluxo sequencial, onde será apresentado na aba Geral o botão **"****Abrir configurador de condições"**.

![unnamed.png](https://ajuda.sankhya.com.br/hc/article_attachments/5567336333207)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configurador de condições</strong></span></p></td></tr></tbody></table>

Ao abrir o configurador de condições, o usuário deverá selecionar no **"Modo de construção"** a opção **"Avançado"**.

![unnamed\_\_2\_.png](https://ajuda.sankhya.com.br/hc/article_attachments/5569988416023)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Modo de construção - Avançado</strong></span></p></td></tr></tbody></table>

Neste exemplo, iremos configurar um script para buscar os dados de um campo do formulário formatado, para o caso onde a solicitação de adiantamento for reprovada. Então para que este cenário ocorra é necessário definir o script abaixo:

 ![Marcador 2 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16092447985559) O exemplo abaixo é referente ao processo de Adiantamento de viagens, no gateway Aprovação de adiantamento. Para realizar um teste, utilizando esse script, procure na base utilizada um processo correspondente.

**Campo**: SITUACAO

**Formulário**: AD\_SOLICITACAOADIANTAMENTO

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre class="wysiwyg-text-align-justify"><span class="wysiwyg-color-black50"><em><span style="font-weight: 400;">//Obter dados do formulário</span></em></span><br><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">formulario</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">=</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">getLinhasFormulario</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"AD_SOLICITACAOADIANTAMENTO"</span><span style="font-weight: 400;">);</span><br><span class="wysiwyg-color-black50"><em><span style="font-weight: 400;">//Se o campo SITUACAO for igual a RP (REPROVADO) a condição será verdadeira</span></em></span><br><span class="wysiwyg-color-yellow120" style="font-weight: 400;">if</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">formulario</span><span style="font-weight: 400;">[</span><span class="wysiwyg-color-pink110" style="font-weight: 400;">0</span><span style="font-weight: 400;">].</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">getCampo</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"SITUACAO"</span><span style="font-weight: 400;">) </span><span class="wysiwyg-color-yellow120" style="font-weight: 400;">==</span> <span class="wysiwyg-color-cyan110" style="font-weight: 400;">'RP'</span><span style="font-weight: 400;">){</span><br><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="wysiwyg-color-yellow120" style="font-weight: 400;">return</span> <span class="wysiwyg-color-yellow110" style="font-weight: 400;">true</span><span style="font-weight: 400;">;</span><br><span style="font-weight: 400;">}</span><span class="wysiwyg-color-yellow120" style="font-weight: 400;">else</span><span style="font-weight: 400;">{</span><br><span style="font-weight: 400;"> &nbsp;  <span class="wysiwyg-color-yellow120" style="font-weight: 400;">return</span></span> <span class="wysiwyg-color-yellow110" style="font-weight: 400;">false</span><span style="font-weight: 400;">;</span><br><span style="font-weight: 400;">}</span></pre></td></tr></tbody></table>

No script deve ser informada sempre a chave que resulta na opção de um determinado campo; por exemplo a lista de opções para o campo SITUACAO são:

**RP=REPROVADO**  
**AP=APROVADO**

Ou seja, a chave corresponde à **"RP"** e **"AP"**.

Para buscar os dados de um campo do formulário formatado para um único registro, utilizamos a função **getLinhasFormulario**, conforme demonstrado no exemplo acima. Quando usado o formulário nativo, utilizamos a função **getLinhasFormularioNativo**, e para buscar um campo de um formulário embarcado, é utilizada a função **getCampo**, de acordo com o exemplo abaixo:

**Linguagem Groovy:** getCampo("DOCUMENTACAO") _\==_ "S"

**Linguagem JavaScript:** return getCampo("DOCUMENTACAO") \== "S"

 **![dica FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16092447987991)**É possível utilizar apenas as funções de consulta para os scripts de gateways. Elas estão disponíveis no botão **"Ajuda"** ![mceclip6.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405306768535) do script.

---

Por fim, a configuração do Gateway Inclusivo segue conforme apresentado no exemplo anterior do Gateway Exclusivo, ou seja, é necessário inserir uma condição para que o caminho seja executado conforme os dados inseridos na tarefa anterior. Quando o caminho for definido como fluxo padrão, não é necessário inserir uma condição.

[\[voltar ao topo\]](#top)