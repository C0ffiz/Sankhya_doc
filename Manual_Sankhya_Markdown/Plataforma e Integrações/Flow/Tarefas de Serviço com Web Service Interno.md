# Tarefas de Serviço com Web Service Interno

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/4403903691799-Tarefas-de-Servi%C3%A7o-com-Web-Service-Interno](https://ajuda.sankhya.com.br/hc/pt-br/articles/4403903691799-Tarefas-de-Servi%C3%A7o-com-Web-Service-Interno)

---

# Tarefas de Serviço com Web Service Interno

![Versão - 32x32 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313315342103) **Versão disponível:** a partir da 4.4

---

Esse é um recurso existente em tarefas de serviço do SankhyaFlow, que permite integrar processos de negócios em execução na ferramenta com os demais serviços nativos do Sankhya Om, possibilitando enviar e receber dados.

A utilização de uma tarefa de serviço com Web Service Interno no Flow realiza a integração com recursos nativos de nosso ERP sem a necessidade de desenvolvimento utilizando módulos Java, o que o torna mais simples e rápido, possibilitando aproveitar as rotinas já existentes no Sankhya Om e acrescentar novas funcionalidades no Flow, sem que seja necessário desenvolver rotinas do ERP a partir do zero.

Nesse artigo, você terá acesso aos seguintes tópicos:

---

1.  [Caso de Uso](#casodeuso)                                                                       
2.  [Configurando tarefa de serviço com Web Service Interno](#configurandotarefadeservi%C3%A7ocomwebserviceinterno)
3.  [Resultados](#resultados)

---

#### **Caso de Uso**

Na imagem abaixo, temos a representação do processo de [Controle de Qualidade de Matérias Primas](https://drive.google.com/drive/folders/1GSZI4NXqBmW_90vwrYt99eyK7CzTbYKt) de uma indústria. Esse processo tem o objetivo de analisar os padrões de qualidades de matérias primas adquiridas de fornecedores antes da disponibilização para a etapa de fabricação. Ocorrem etapas de coletas, validação e revisão de uma amostra e, na sequência, a geração do laudo; assim, havendo aprovação em todas as etapas, a matéria prima é liberada para as áreas de produção da indústria.

![flow13.png](https://ajuda.sankhya.com.br/hc/article_attachments/4403903985431)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Processo de Controle de Qualidade</strong></span></p></td></tr></tbody></table>

Em nosso caso de uso, iremos configurar a tarefa de serviço **"Aprovação da amostra"** (destacada em amarelo na imagem acima) com Web Service Interno para, a partir do Flow, aprovarmos amostras utilizando o serviço nativo do Sankhya Om.

É importante ressaltar que o serviço nativo de aprovação de amostrar, quando acionado, registra diversas operações nos módulos de nosso ERP, dentre elas, a baixa de estoque da amostra que foi coletada.

 **![essencial FINAL (1).png](https://ajuda.sankhya.com.br/hc/article_attachments/16117217120023)**Com o Web Service Interno teremos apenas scripts para chamarmos o serviço de aprovação de amostra. Dessa forma, não teremos a necessidade de desenvolver códigos complexos em nosso processo de negócio com finalidade específica de gerar essas baixas, o que torna o desenvolvimento de scripts mais simples.

Também utilizaremos dados de retorno do serviço para registrar o número da requisição de baixa de estoque no formulário do Flow, para visualização em tarefas subsequentes, garantindo melhor rastreabilidade das informações do processo.

[\[voltar ao topo\]](#top)

#### **Configurando tarefa de serviço com Web Service Interno**

---

**Identificando o Serviço**

O primeiro passo para configurar uma tarefa de serviço com Web Service é identificar qual serviço nativo do ERP iremos utilizar. Uma maneira prática para identificá-lo é acessar o recurso nativo do ERP e executá-lo.

Em nosso exemplo, para identificar o serviço da tarefa Aprovação de amostra, iremos acessar a tela [Registro de Amostras](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044611334-Registro-de-Amostras) do Sankhya Om e deixar a amostra no ponto para ser aprovada (preencher os campos **"Dh. Amostragem"** e **"Dh. Verificação"**) ou seja, momento antes da execução do serviço que iremos identificar.

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4403910480791)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Tela Registro de Amostras</strong></span></p></td></tr></tbody></table>

Antes de clicar no botão ![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/4403904285463) **"Aprovar"**, abra a ferramenta de desenvolvimento do seu navegador para que possamos localizar o serviço que será executado quando tentarmos aprovar a amostra.

Nesse exemplo, estamos utilizando o navegador Mozilla Firefox. Assim, após pressionar a tecla **"F12"** (atalho para ferramentas de desenvolvimento), a janela abaixo será aberta. Na sequência, acesse a aba **"Rede"** para consultar o serviço que será utilizado para aprovar a amostra:

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4403910579991)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Propriedades da Página</strong></span></p></td></tr></tbody></table>

Nesse momento, na tela de Registro de Amostras, clique no botão Aprovar. Então, após a aprovação, será apresentado o registro do serviço que foi utilizado, conforme destacado na imagem abaixo:

![mceclip3.png](https://ajuda.sankhya.com.br/hc/article_attachments/4403910790679)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Serviço Identificado</strong></span></p></td></tr></tbody></table>

Ao clicar sobre o serviço, será apresentado o cabeçalho. Nele podemos consultar informações importantes como o nome do serviço apresentado no campo **"serviceName"** (que será utilizado na configuração do Web Service Interno).

Também é possível visualizar no cabeçalho o **"Content-Type"**, que define o formato aceito pelo serviço para gerar a requisição, podendo ser JSON ou XML.

**Observação:** o formato aceito determinará a forma como iremos chamar o serviço. No exemplo da imagem abaixo, temos o formato JSON:

![mceclip4.png](https://ajuda.sankhya.com.br/hc/article_attachments/4403910840727)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Primeira parte do cabeçalho do serviço</strong></span></p></td></tr></tbody></table>

![mceclip5.png](https://ajuda.sankhya.com.br/hc/article_attachments/4403910861975)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Segunda parte do cabeçalho do serviço</strong></span></p></td></tr></tbody></table>

 ![essencial FINAL (1).png](https://ajuda.sankhya.com.br/hc/article_attachments/16117217120023)Se o formato fosse XML, em **"Content-Type"** teríamos: **'text/xml;charset=UFT-8'**.

[\[voltar ao subtítulo\]](#configurandotarefadeservi%C3%A7ocomwebserviceinterno) [\[voltar ao topo\]](#top)

---

**Identificação dos Parâmetros da Requisição do Serviço**

Acessando a aba **"Requisição"**, podemos verificar os parâmetros que foram utilizados para a chamada do serviço.

Conforme podemos visualizar na imagem abaixo, a requisição contém o nome do serviço e seus parâmetros são apresentados em **"requestBody"**. Nesse caso, verificamos que nessa chamada foi requisitada a aprovação da amostra de número 53:

![mceclip6.png](https://ajuda.sankhya.com.br/hc/article_attachments/4403911076631)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Requisição do Serviço</strong></span></p></td></tr></tbody></table>

**Observação:** o conteúdo contido em **"requestBody"** será utilizado para definirmos o script de requisição na nossa tarefa de serviço **"Aprovação da amostra"**.

[\[voltar ao subtítulo\]](#configurandotarefadeservi%C3%A7ocomwebserviceinterno) [\[voltar ao topo\]](#top)

---

**Identificação de Dados da Resposta do Serviço**

A visualização do retorno de serviço é apresentada na aba **"Resposta"**. No exemplo da imagem abaixo, foi respondido o status = 1. Por padrão do Sankhya Om, quando o status for 1, significa que houve sucesso na tentativa de execução do processo, no caso, a aprovação da amostra:

![mceclip7.png](https://ajuda.sankhya.com.br/hc/article_attachments/4403904988311)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Propriedade de Retorno do Serviço</strong></span></p></td></tr></tbody></table>

**Nota:** quando o resultado for diferente de 1, significa que por algum motivo não houve sucesso na requisição solicitada.

 **![essencial FINAL (1).png](https://ajuda.sankhya.com.br/hc/article_attachments/16117217120023) Importante:** os dados da resposta poderão facilmente serem registrados em campos de formulários do Flow, que será apresentado em exemplo no decorrer desse artigo.

[\[voltar ao subtítulo\]](#configurandotarefadeservi%C3%A7ocomwebserviceinterno) [\[voltar ao topo\]](#top)

---

**Configurando a Tarefa de Serviço com Web Service Interno**

Para a tarefa de serviço **"Aprovação da amostra"**, selecione o tipo de serviço **"Web Service Interno"** e, em seguida, clique no botão de configurações. Após isso, procure pelo serviço de aprovação de amostra que identificamos anteriormente (_RegistroAmostraSP.aprovarReprovarAmostra_). Observe abaixo:

![flow13.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4403911395095)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configuração do Web Service e Pesquisa do Serviço</strong></span></p></td></tr></tbody></table>

Agora já podemos definir o script de requisição do serviço de aprovação. Em tarefas anteriores do processo, será registrado o número da amostra em campo do formulário. Como esse é o parâmetro que identificamos como necessário para a requisição, vamos definir uma variável (nuAmostra) para registrar esse número e utilizá-la na requisição. Nesse exemplo, a requisição será realizada para o formato JSON que foi identificado anteriormente no cabeçalho:

![mceclip8.png](https://ajuda.sankhya.com.br/hc/article_attachments/4403911543959)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Script da Requisição</strong></span></p></td></tr></tbody></table>

Script completo contido na imagem acima:

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre><em><span class="wysiwyg-font-size-small wysiwyg-color-black50">//Variáveis para registrar o número da amostra inserido em campo de formulário do Flow</span></em><br><span class="wysiwyg-font-size-small"><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">buscarFormulario</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">=</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">getLinhasFormulario</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"AD_TWFTGFRAM"</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small"><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">nuAmostra</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">= </span><span class="wysiwyg-color-blue80" style="font-weight: 400;">buscarFormulario</span><span style="font-weight: 400;">[</span><span class="wysiwyg-color-pink110" style="font-weight: 400;">0</span><span style="font-weight: 400;">].</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">getCampo</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"NURAM"</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-color-black50"><em><span class="wysiwyg-font-size-small" style="font-weight: 400;">//Parâmetros da requisição</span></em></span><br><span class="wysiwyg-font-size-small"><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">payload</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">=</span> <span style="font-weight: 400;">"{</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">serviceName</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">:</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">RegistroAmostrasSP.aprovarReprovarAmostra</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">,</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">requestBody</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">:{</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">params</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">:{</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">isAprovacao</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">:true,<br></span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">nuRam</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">:[{</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">$</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">:"</span><span style="font-weight: 400;">+</span><span style="font-weight: 400;">nuAmostra</span><span style="font-weight: 400;">+</span><span style="font-weight: 400;">"}]},</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">clientEventList</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">:{</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">clientEvent</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">:{</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">$</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">:</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">br.com.sankhya.actionbutton.clientconfirm</span><span style="font-weight: 400;">\"</span><span style="font-weight: 400;">}]}}}"</span><span style="font-weight: 400;">;</span></span><br><span class="wysiwyg-color-black50"><em><span class="wysiwyg-font-size-small" style="font-weight: 400;">//A função JSON.parse() converte texto para formato JSON</span></em></span><br><span class="wysiwyg-font-size-small"><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">payloadJS</span> <span style="font-weight: 400;">=</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">JSON</span><span style="font-weight: 400;">.</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">parse</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">payload</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small"><span class="wysiwyg-color-yellow120" style="font-weight: 400;">return</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">payloadJS</span></span></pre></td></tr></tbody></table>

Observe que declaramos a variável **"payload"** com todos os parâmetros de requisição que havíamos identificado anteriormente e, no lugar do número da amostra, inserimos a variável **"nuAmostra"**, que se refere a um valor registrado anteriormente em formulário do Flow.

Caso o serviço identificado no cabeçalho aceitasse apenas o formato XML, a requisição seria realizada nesse formato, conforme o script abaixo:

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre class="wysiwyg-text-align-justify"><span class="wysiwyg-color-black50 wysiwyg-font-size-small"><em><span style="font-weight: 400;">//Variáveis para registrar o número da amostra inserido em campo de formulário do Flow</span></em></span><br><span class="wysiwyg-font-size-small"><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">buscarFormulario</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">=</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">getLinhasFormulario</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"AD_TWFTGFRAM"</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-font-size-small"><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">nuAmostra</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">= </span><span class="wysiwyg-color-blue80" style="font-weight: 400;">buscarFormulario</span><span style="font-weight: 400;">[</span><span class="wysiwyg-color-pink110" style="font-weight: 400;">0</span><span style="font-weight: 400;">].</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">getCampo</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"NURAM"</span><span style="font-weight: 400;">);</span></span><br><em><span class="wysiwyg-font-size-small wysiwyg-color-black50" style="font-weight: 400;">//Parâmetros da requisição</span></em><br><span class="wysiwyg-font-size-small wysiwyg-color-yellow120" style="font-weight: 400;">return</span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">&nbsp;&nbsp;&nbsp;<span class="wysiwyg-color-cyan110">&nbsp;</span></span><span class="wysiwyg-color-cyan110"><span style="font-weight: 400;">"&lt;params isAprovacao=true&gt;&lt;nuRam&gt;"</span><span style="font-weight: 400;">+</span><span style="font-weight: 400;">nuAmostra</span><span style="font-weight: 400;">+</span><span style="font-weight: 400;">"&lt;/nuRam&gt;&lt;/params&gt;"</span></span><span style="font-weight: 400;">;</span></span></pre></td></tr></tbody></table>

**Observação:** a **"nuAmostra"** representa a variável que deve ser declarada para obter o valor do campo contido no formulário.

Após definidas as configurações da requisição, podemos também configurar o retorno da requisição, sendo possível obter dados desse retorno e registrar em campos de formulários do Flow.

Em nosso exemplo, quando uma amostra é aprovada, é gerada uma mensagem de aprovação pelo Sankhya Om e um número de requisição da baixa de estoque da amostra. Iremos obter esse número pelo retorno do Web Service e registrar em campo do Flow, para que esse dado possa ser consultado nas tarefas subsequentes do processo.

**Nota:** o retorno de dados do Web Service sempre é obtido utilizando a variável **"retornoWSI"**.

Como já vimos anteriormente, o retorno do Web Service de aprovação contém os seguintes dados:

![mceclip9.png](https://ajuda.sankhya.com.br/hc/article_attachments/4403911664407)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Retorno do Serviço</strong></span></p></td></tr></tbody></table>

No script, iremos armazenar na variável **"retornoJS"** todo o conteúdo do retorno. Na variável **"retornoString"** vamos obter o conteúdo do objeto **"{msg'.$}"** e, por fim, registramos a variável **"retornoString"** no campo **"NUMREQ"**, que pertence ao formulário do Flow, utilizando funções para selecionar apenas os números:

![mceclip10.png](https://ajuda.sankhya.com.br/hc/article_attachments/4403911710231)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configuração do script de Retorno</strong></span></p></td></tr></tbody></table>

Script completo de retorno:

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre class="wysiwyg-text-align-justify"><span class="wysiwyg-color-black50"><em><span class="wysiwyg-font-size-small" style="font-weight: 400;">//JSON.parse() realiza a conversão do conteúdo para string</span></em></span><br><span class="wysiwyg-font-size-small"><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">retornoJS</span> <span style="font-weight: 400;">=</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">JSON</span><span style="font-weight: 400;">.</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">parse</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">retornoWSI</span><span style="font-weight: 400;">);</span></span><br><span class="wysiwyg-color-black50"><em><span class="wysiwyg-font-size-small" style="font-weight: 400;">//Obtém o conteúdo específico do objeto </span></em></span><br><span class="wysiwyg-font-size-small"><strong>var</strong> <span class="wysiwyg-color-blue80" style="font-weight: 400;">retornoString</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">=</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">retornoJS</span><span style="font-weight: 400;">.</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">msg</span><span style="font-weight: 400;">.</span><span style="font-weight: 400;">$</span><span style="font-weight: 400;">;</span></span><br><span class="wysiwyg-color-black50"><em><span class="wysiwyg-font-size-small" style="font-weight: 400;">//Identifica na mensagem o número da requisição e registra no campo do formulário do Flow o número da requisição, utilizando <br>o “método replace(), que retorna uma nova string com algumas ou todas as correspondências de um padrão substituídas por um <br>determinado caractere (ou caracteres)”.<br></span></em></span><span class="wysiwyg-font-size-small wysiwyg-color-black" style="font-weight: 400;"><span class="wysiwyg-font-size-small"><strong>var </strong></span></span><span class="wysiwyg-color-black50"><span class="wysiwyg-font-size-small" style="font-weight: 400;"><span class="wysiwyg-font-size-small"><span class="wysiwyg-color-blue80" style="font-weight: 400;">buscarFormulario</span> <span class="wysiwyg-color-yellow120" style="font-weight: 400;">=</span> <span class="wysiwyg-color-blue80" style="font-weight: 400;">getLinhasFormulario</span><span style="font-weight: 400;">(</span></span></span><span class="wysiwyg-font-size-small" style="font-weight: 400;"><span class="wysiwyg-font-size-small"><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"AD_TWFTGFRAM"</span></span></span><em><span class="wysiwyg-font-size-small" style="font-weight: 400;"><span class="wysiwyg-font-size-small"><span style="font-weight: 400;">);</span></span></span></em></span><br><span class="wysiwyg-font-size-small"><span style="font-weight: 400;"><span class="wysiwyg-color-black50"><em><span class="wysiwyg-font-size-small" style="font-weight: 400;"><span class="wysiwyg-color-blue80" style="font-weight: 400;">buscarFormulario</span></span></em></span>[</span><span class="wysiwyg-color-pink110" style="font-weight: 400;">0</span><span style="font-weight: 400;">].</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">setCampo</span><span style="font-weight: 400;">(</span><span class="wysiwyg-color-cyan110" style="font-weight: 400;">"NUMREQ"</span><span style="font-weight: 400;">,</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">retornoString</span><span style="font-weight: 400;">.</span><span class="wysiwyg-color-blue80" style="font-weight: 400;">replace</span><span style="font-weight: 400;">(</span><span style="font-weight: 400;">/</span><span style="font-weight: 400;">\D</span><span style="font-weight: 400;">/</span><span style="font-weight: 400;">g</span><span style="font-weight: 400;">, </span><span style="font-weight: 400;">''</span><span style="font-weight: 400;">));</span></span></pre></td></tr></tbody></table>

Realizadas as configurações de requisição e retorno do Web Service, basta salvar e publicar o processo.

[\[voltar ao subtítulo\]](#configurandotarefadeservi%C3%A7ocomwebserviceinterno) [\[voltar ao topo\]](#top)

#### **Resultados**

Para visualizar o resultado das configurações, acesse a [Lista de Tarefas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044595434-Lista-de-Tarefas) e inicie o processo **"Controle de Qualidade de Matérias Primas"**. Em seguida, finalize as atividades **"Coletar amostra"** e **"Validar amostra colhida"**, e aprove a tarefa **"Analisar amostra"**.

Na sequência, o fluxo irá executar a tarefa de serviço com Web Service Interno **"Aprovação da amostra"** que configuramos anteriormente.

O Web Service realiza a aprovação da amostra e a mesma é direcionada para a tarefa de usuário seguinte (Gerar laudo), em que podemos verificar que o número da requisição de baixa foi identificado no retorno do Web Service e inserido no campo específico que determinamos no script de retorno:

![flow14.png](https://ajuda.sankhya.com.br/hc/article_attachments/4403905591575)

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Tela do processo no Flow após execução da Tarefa de Serviço</strong></span></p></td></tr></tbody></table>

[\[voltar ao topo\]](#top)