# Eventos de Campos

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/4403799538199-Eventos-de-Campos](https://ajuda.sankhya.com.br/hc/pt-br/articles/4403799538199-Eventos-de-Campos)

---

# Eventos de Campos

![Versão - 32x32 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313314694935) **Versão:** a partir da 4.2

---

Os Eventos de Campos são ações personalizadas que permite manipular dados nos campos de um formulário (embarcado, formatado e nativo) na inicialização e/ou nas tarefas, com o objetivo de nos instruir durante o preenchimento do mesmo. Essas ações podem ser definidas em 3 momentos, sendo eles:

*   **Evento de entrada:** No momento que o campo receber o "foco" (clicar no campo), a ação será executada.
*   **Evento de saída:** No momento que o campo perder o "foco" (ao sair do campo), a ação será realizada.
*   **Evento de alteração:** No momento que o campo tiver seu conteúdo alterado, a ação será feita.

Com eventos de campos é possível executar ações como: validação do conteúdo informado ao sair do campo, preenchimento de um conteúdo automaticamente quando o campo receber foco, ou então, a partir de dados de outros campos do formulário, ter histórico de campo, etc.

Nesse artigo, você terá acesso sobre:

---

1.  [Caso de Uso](#casodeuso)                                                                       
2.  [Configurações e Resultados](#configura%C3%A7%C3%B5eseresultados)
3.  [Demais informações sobre os Eventos de Campos](#demaisinforma%C3%A7%C3%B5esobreoseventosdecampos)

---

#### **Caso de Uso**

Na imagem abaixo, temos a representação do processo de [Adiantamento de Viagem](https://drive.google.com/drive/folders/1w6yYzFz0WlgMFDWqZlipUEZLVG6z-UiE) de uma Empresa, o qual utiliza eventos de campos na inicialização do processo.

![flow6.png](https://ajuda.sankhya.com.br/hc/article_attachments/4403852668055)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Processo de Adiantamento de Viagem</strong></span></p></td></tr></tbody></table>

Esse processo permite que qualquer colaborador solicite um adiantamento de viagem acima de R$20,00 para o seu líder imediato. Caso seja inserido um valor menor, o campo apresentará um erro contendo uma mensagem e somente será possível prosseguir quando for informado um valor acima do permitido.

Quando o valor solicitado for menor ou igual à R$100,00, a forma de pagamento será realizada em dinheiro e, acima desse valor, a empresa realiza uma transferência bancária; para isso, ao informar o valor do adiantamento, um determinado campo do formulário (embarcado) é preenchido com essa informação.

Na solicitação, existe o campo **"Observações"**, para que o colaborador informe o tipo de despesa. Assim, ao clicar no campo, será apresentado um template para guiá-lo a preencher as informações.

Após solicitar o adiantamento, o processo seguirá para aprovação/reprovação.

[\[voltar ao topo\]](#top)

#### **Configurações e Resultados**

---

**Validação do valor de adiantamento menor que R$20,00**

Para atender essa regra, utilizamos o evento de alteração de campo, que dará um erro no campo contendo uma mensagem, para o caso em que informamos o valor do adiantamento menor do que R$20,00.

Para isso, acessamos as configurações avançadas do formulário formatado **"AD\_SOLICITACAOADIANTAMENTO"** e, sem seguida, selecionamos o campo do formulário **"VALORADIANTAMENTO"**, clicamos nas configurações avançadas do campo e abrimos a aba **"Eventos de Alteração"**, conforme demonstramos abaixo:

![flow7.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4403857702039)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configurações avançadas de campo do Evento de Alteração</strong></span></p></td></tr></tbody></table>

**Observação:** para que o cenário acima ocorra, é necessário escrever o script abaixo, contemplando as seguintes informações:

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre class="wysiwyg-text-align-justify wysiwyg-indent2"><span class="wysiwyg-font-size-medium"><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">valor</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">=</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">getCampo</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"VALORADIANTAMENTO"</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-medium"><span class="wysiwyg-color-yellow120" style="font-weight: 400;">if</span><span style="font-weight: 400;"> (<span class="wysiwyg-color-blue80" style="font-weight: 400;">valor</span></span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">&lt;</span><span class="wysiwyg-color-pink110" style="font-weight: 400;">20</span><span style="font-weight: 400;">){</span></span><br><span class="wysiwyg-font-size-medium"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="wysiwyg-color-black50"><em><span style="font-weight: 400;">//Sinaliza visualmente o erro no campo contendo uma mensagem </span></em></span></span><br><span class="wysiwyg-font-size-medium"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">erroCampo</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"O valor solicitado deve ser maior que R$20,00."</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-medium" style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;}</span></pre></td></tr></tbody></table>

No nosso exemplo, a colaboradora Juliane informou um valor de adiantamento de R$18,00. Então, conforme a regra, foi apresentado um erro no campo:

![flow8.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4403903233047)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Solicitação de adiantamento com valor menor do que R$20,00.</strong></span></p></td></tr></tbody></table>

Então, a função **erroCampo** utilizada nesse exemplo sinaliza um erro no campo contendo uma mensagem. Para esse mesmo caso, poderíamos utilizar a função **mensagemErroCampo**, a qual apresentaria um pop-up contendo uma mensagem de erro, ambas funções e somente conseguiríamos seguir com a solicitação no momento em que fosse informado um valor acima do permitido.

---

**Definição de conteúdo no campo "FORMAPAGAMENTO" (campo do formulário embarcado) a partir do valor solicitado (campo do formulário formatado)**

Para atender essa regra, iremos utilizar o evento de saída. Quando o valor do adiantamento for menor ou igual à R$100,00, a forma de pagamento será em dinheiro e, maior que esse valor, será realizada uma transferência bancária.

**Nota:** essa informação será inserida no campo FORMAPAGAMENTO do formulário embarcado.

Inicialmente, acessamos as configurações avançadas do formulário formatado **"AD\_SOLICITACAOADIANTAMENTO"**. Em seguida, selecionamos o campo do formulário **"VALORADIANTAMENTO"**, acessamos as configurações avançadas desse campo e clicamos na aba **"Eventos de Saída"**. Observe abaixo: 

![flow9.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4403897565335)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configurações avançadas de campo do Evento de Saída</strong></span></p></td></tr></tbody></table>

Assim, para que esse cenário ocorra, devemos escrever o script abaixo com as seguintes informações:

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre class="wysiwyg-text-align-justify wysiwyg-indent1"><span class="wysiwyg-font-size-small" style="font-weight: 400;"><span class="wysiwyg-color-black" style="font-weight: 400;"><strong>var </strong></span><span class="wysiwyg-color-yellow120" style="font-weight: 400;"><span class="wysiwyg-color-blue80" style="font-weight: 400;">valor</span>=<span class="wysiwyg-color-blue80" style="font-weight: 400;">getCampo</span>(<span class="wysiwyg-color-cyan110" style="font-weight: 400;">"VALORADIANTAMENTO"</span>);</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;"><span class="wysiwyg-color-yellow120" style="font-weight: 400;">if</span></span><span style="font-weight: 400;">(<span class="wysiwyg-font-size-small" style="font-weight: 400;"><span class="wysiwyg-color-yellow120" style="font-weight: 400;"><span class="wysiwyg-color-blue80" style="font-weight: 400;">valor</span></span></span></span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">&lt;=</span> <span class="wysiwyg-color-pink110" style="font-weight: 400;">100</span><span style="font-weight: 400;">){</span></span><span class="wysiwyg-font-size-small"><span style="font-weight: 400;"><span class="wysiwyg-color-black50"><br> </span></span><span class="wysiwyg-color-black50" style="font-weight: 400;">//Define valor a um campo. Para manipular um campo do formulário embarcado, o campo deve estar precedido da palavra 'embarcado'</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;<span class="wysiwyg-color-blue80">&nbsp;</span></span><span class="wysiwyg-color-blue80" style="font-weight: 400;">setCampo</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"embarcado.FORMAPAGAMENTO"</span><span style="font-weight: 400;">, </span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"Dinheiro"</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;}</span><span class="wysiwyg-color-yellow120" style="font-weight: 400;">else</span><span style="font-weight: 400;">{</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;"> &nbsp;&nbsp;&nbsp;  <span class="wysiwyg-color-blue80" style="font-weight: 400;">setCampo</span>(<span class="wysiwyg-color-cyan110" style="font-weight: 400;">"embarcado.FORMAPAGAMENTO"</span>,</span> <span class="wysiwyg-color-cyan110" style="font-weight: 400;">"Transferência bancária"</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small" style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;}</span></pre></td></tr></tbody></table>

Em nosso exemplo acima, a colaboradora Juliane informou um valor de adiantamento de R$1000,00. Dessa maneira, conforme a regra, a forma de pagamento será através de transferência bancária e essa informação constará no campo **"Forma de pagamento"** do formulário embarcado, como podemos observar logo abaixo:

![flow10.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4403897584279)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Solicitação de adiantamento com forma de pagamento via transferência bancária</strong></span></p></td></tr></tbody></table>

---

**Definição de conteúdo no campo "Observações"**

Para essa regra, utilizaremos o evento de entrada, onde o colaborador deve informar o tipo de despesa no campo **"Observações"**. Para isso, ao clicar no campo, será apresentado um template para guiá-lo no preenchimento dessas informações. 

Então, acessamos as configurações avançadas do formulário formatado **"AD\_SOLICITACAOADIANTAMENTO"**, selecionamos o campo do formulário **"OBSERVACOES"**, clicamos no botão de configurações avançadas desse campo e abrimos a aba **"Eventos de Entrada"**, conforme demonstramos abaixo:

![flow11.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4403903438231)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configurações avançadas de campo do Evento de Entrada</strong></span></p></td></tr></tbody></table>

Para termos o cenário acima, devemos escrever o script abaixo:

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre class="wysiwyg-text-align-justify wysiwyg-indent2"><span class="wysiwyg-color-black50 wysiwyg-font-size-small"><em><span style="font-weight: 400;">//Verifica se o campo está vazio</span></em></span><br><span class="wysiwyg-font-size-small"><span class="wysiwyg-color-yellow120" style="font-weight: 400;">if</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">getCampo</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"OBSERVACOES"</span><span style="font-weight: 400;">) </span><span class="wysiwyg-color-yellow120" style="font-weight: 400;">==</span> <span class="wysiwyg-color-yellow110" style="font-weight: 400;">undefined</span><span style="font-weight: 400;">){</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="wysiwyg-color-black50"><em><span style="font-weight: 400;">//Define um conteúdo para o campo</span></em></span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">setCampo</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"OBSERVACOES"</span><span style="font-weight: 400;">, </span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"Informe o(s) tipos(s) de despesa(s) (passagem, alimentação, curso, etc):"</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">}</span></span></pre></td></tr></tbody></table>

**Observação:** utilizamos o **"if"** para que, quando for inserida uma informação e ela for salva, ao clicar novamente no campo, não sejam perdidas as informações já inseridas, ou seja, é para manter as informações.

Na solicitação do adiantamento de viagem, ao clicar no campo Observações, será apresentado um template para preenchimento:

![flow12.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4403897665815)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Solicitação de adiantamento com conteúdo no campo "Observações"</strong></span></p></td></tr></tbody></table>

[\[voltar ao topo\]](#top)

#### **Demais informações sobre os Eventos de Campos**

As funções **erroCampo**, **mensagemErroCampo**, **getCampo**, **setCampo** estão todas disponíveis para o uso em eventos de campos, o qual estão detalhadas no help do script.

É importante ressaltar que, nesse contexto, é possível utilizar apenas a linguagem **JavaScript**.

Ao utilizar uma dessas funções, caso o nome do campo esteja precedido da palavra Embarcado, será possível referenciar um campo do formulário embarcado, ou seja, pode-se manipular campos do formulário embarcado a partir de formulários formatado/nativo.

No contexto **"Evento de Alteração"** também estão disponíveis as variáveis oldValue (valor do campo antes da alteração) e newValue (valor do campo após alteração).

[\[voltar ao topo\]](#top)