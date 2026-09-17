# Multiplicidade Paralela

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/4409363885591-Multiplicidade-Paralela](https://ajuda.sankhya.com.br/hc/pt-br/articles/4409363885591-Multiplicidade-Paralela)

---

# Multiplicidade Paralela

![Versão - 32x32 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313326986647) **Versão disponível:** a partir da 4.7

---

A multiplicidade é um recurso do SankhyaFlow que possibilita ao modelador configurar a abertura de uma determinada Tarefa de Usuário quantas vezes forem necessárias, de forma paralela ou sequencial.

A Multiplicidade Paralela permite que uma atividade possa ocorrer diversas vezes ao mesmo tempo, ou seja, usuários diferentes podem trabalhar simultaneamente em uma mesma Tarefa de Usuário.

Geralmente, esse recurso é utilizado quando várias pessoas precisam realizar uma mesma tarefa simultaneamente.

Como exemplo, podemos mencionar uma tarefa de confecção de parecer sobre pedido de reembolso feito por um cliente da empresa; a depender do tipo de reembolso, diversas pessoas irão atuar simultaneamente na tarefa para registrarem o seu parecer a respeito do pagamento do reembolso.

Nessa documentação trataremos sobre nosso [Caso de Uso](#casodeuso), a [Configuração de uma Tarefa de Usuário com Multiplicidade Paralela](#configura%C3%A7%C3%A3odeumatarefadeusu%C3%A1riocommultiplicidadeparalela), as [Demais configurações do Caso de Uso](#demaisconfigura%C3%A7%C3%B5esdocasodeuso), [Outras informações sobre Multiplicidade Paralela](#outrasinforma%C3%A7%C3%B5essobremultiplicidadeparalela) e os [Resultados](#resultados).

---

#### **Caso de Uso**

A empresa Alpha Ltda utiliza o SankhyaFlow em seu processo de **"Separação de Produtos"**, apresentado na imagem abaixo:

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409357487895)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><strong>Processo de Pedido de vendas simplificado</strong></p></td></tr></tbody></table>

Esse processo possibilita a solicitação de forma ágil, através de um Pedido de Vendas, Separação e Conferência de Produtos.

Na solicitação do pedido, caso os produtos solicitados sejam de diferentes grupos de produtos, será aberta uma instância para cada grupo de produto dessa solicitação, pois há diferentes separadores para cada grupo de produtos da empresa.

Após a separação dos produtos, é realizada a conferência para verificar se os itens dos pedidos estão conforme o solicitado e, por fim, o solicitante recebe um e-mail informando que sua solicitação foi finalizada.

![essencial FINAL (1).png](https://ajuda.sankhya.com.br/hc/article_attachments/16111000300439) Esse é um processo apenas ilustrativo e não gera pedido.

[\[voltar ao topo\]](#top)

#### **Configuração de uma Tarefa de Usuário com Multiplicidade Paralela**

Para que seja aberta uma instância para cada grupo de produto da solicitação, iremos configurar a tarefa **"Separar produtos"** com a **"Instância Múltipla Paralela"**:

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409357657495)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><strong>Instância Múltipla Paralela</strong></p></td></tr></tbody></table>

Após inserir a Instância Múltipla Paralela na tarefa, devemos configurar a quantidade de tarefas a serem geradas, através da aba **"Multiplicidade"**, sub-aba **"Quantidade de tarefas"**:

![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409357693591)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><strong>Configuração Quantidade de Tarefas</strong></p></td></tr></tbody></table>

**Observação:** a quantidade de tarefas pode ser definida através de um script, ou então, inserindo um número inteiro positivo.

Nesse exemplo, iremos configurar uma expressão dinâmica. Ela contará quantos grupos de produtos existem na solicitação que foi aberta, em função dos produtos que ele inseriu.

Segue abaixo o script que definimos:

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre class="wysiwyg-text-align-justify"><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">var<span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium">query</span></span><span class="wysiwyg-font-size-medium wysiwyg-color-yellow120">=</span> </span></span><span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium">getQuery</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">();<br></span></span><span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium">query</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">.</span></span><span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium">setParam</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">(</span></span><span class="wysiwyg-color-cyan110"><span class="wysiwyg-font-size-medium">"IDINSTPRN"</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">, </span></span><span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium">getIdInstanceProcesso</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">()); <br><span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium">query</span></span>.</span></span><span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium">nativeSelect</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">(</span></span><span class="wysiwyg-color-cyan110"><span class="wysiwyg-font-size-medium">"SELECT COUNT(1) AS quantidade FROM TGFPRO WHERE CODPROD IN<br>(SELECT DISTINCT (CODPROD) FROM AD_ITEMPEDIDO WHERE IDINSTPRN = {IDINSTPRN})"</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">);<br><span class="wysiwyg-color-yellow110"><span class="wysiwyg-font-size-medium">if</span></span>(</span></span><span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium">query</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">.</span></span><span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium">next</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">()) {<br><span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium"><span class="wysiwyg-color-yellow110">return</span>query</span></span>.</span></span><span class="wysiwyg-color-blue70"><span class="wysiwyg-font-size-medium">getInt</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">(</span></span><span class="wysiwyg-color-cyan110"><span class="wysiwyg-font-size-medium">"quantidade"</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">);</span></span><span class="wysiwyg-color-black40"><span class="wysiwyg-font-size-medium"><em>/*Essa linha retorna o valor contido em "quantidade", <br>ou seja, quantas tarefas serão criadas.*/</em></span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black"><br>}<span class="wysiwyg-color-yellow110"><span class="wysiwyg-font-size-medium">else</span></span> { <br><span class="wysiwyg-color-yellow110"><span class="wysiwyg-font-size-medium">return</span></span></span></span><span class="wysiwyg-font-size-medium wysiwyg-color-pink110">0</span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black">; <br>}<br></span></span></pre></td></tr></tbody></table>

[\[voltar ao topo\]](#top)

#### **Demais configurações do Caso de Uso**

Em função do caso de uso, para que a tarefa Separar produtos tenha diferentes separadores para cada grupo de produto, configuramos o script abaixo:

![mceclip3.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409357872919)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><strong>Configurando Usuários candidatos dinâmicos</strong></p></td></tr></tbody></table>

**Nota:** para mais informações sobre configurações de usuários candidatos dinâmicos, acesse a documentação [Candidato executante dinâmico](https://ajuda.sankhya.com.br/hc/pt-br/articles/4405488432663-Candidato-executante-din%C3%A2mico).

Para que em cada instância da tarefa gerada seja apresentado no formulário apenas o conteúdo que o responsável precisa ver, ou seja, apenas os produtos que fazem parte do grupo de produto que ele é responsável, configuramos um Evento na criação da tarefa Separar produtos:

![flow18.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4409357929623)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><strong>Configuração de Eventos</strong></p></td></tr></tbody></table>

**Observação:** para mais detalhes sobre configurações de eventos acesse a documentação [Eventos de Processos e Eventos de Tarefa](https://ajuda.sankhya.com.br/hc/pt-br/articles/4406903288855-Eventos-de-Processo-e-Eventos-de-Tarefa).

**Importante:** para que seja possível gerar um registro diferente em cada instância dessa tarefa, o formulário precisa estar configurado como **"Escopo"** de **"Atividade"** e **"Política de reentrância"** para **"Criar sempre um novo registro"**.

[\[voltar ao topo\]](#top)

#### **Outras informações sobre Multiplicidade Paralela**

Podemos definir uma expressão em JavaScript ou Groovy na **"Condição de Parada"**; caso essa expressão retorne verdadeiro, ao finalizar uma execução de uma das instâncias de uma tarefa com multiplicidade paralela, as demais instâncias dessa tarefa que ainda estiverem em aberto serão canceladas:

![mceclip4.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409364296855)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><strong>Configuração Condição de Parada</strong></p></td></tr></tbody></table>

**Nota:** em tarefas canceladas, o responsável não poderá fazer nenhum tipo de manipulação da mesma (alteração de campos dos formulários, desatribuição/atribuição de dono, apontamento e finalização).

Ao configurar uma Condição de Parada, se ainda existirem Tarefas de Usuários com Multiplicidade Paralela em aberto, quando as demais instâncias forem canceladas, os usuários candidatos e/ou donos da Tarefa de Usuário poderão receber uma notificação (via e-mail e/ou sistema) informando sobre o cancelamento:

![mceclip5.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409358161431)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><strong>Configuração de Notificações</strong></p></td></tr></tbody></table>

[\[voltar ao topo\]](#top)

#### **Resultados**

Conforme as configurações realizadas anteriormente, agora apresentaremos os resultados. O responsável fará a solicitação do Pedido de Separação de Produtos na inicialização do processo:

![mceclip6.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409358317207)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><strong>Solicitação Pedido de Separação de Produtos</strong></p></td></tr></tbody></table>

Pelo cadastro da base utilizada, o produto **"Calça Jeans"** está no grupo de Varejo (Código 1100103), enquanto a **"Toalha"** está no grupo Material de limpeza (Código 3000000). Definimos anteriormente que o usuário candidato dinâmico do grupo Varejo será a Júlia e para o grupo Material de limpeza será a Amanda.

Portanto, ao concluir a solicitação do processo Separação de Produtos, serão geradas duas instâncias da Tarefa de Usuário **"Separar produtos"**, uma para Júlia e outra para Amanda:

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409710069527)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><strong>Instância da tarefa Separar produtos (Grupo Varejo)</strong></p></td></tr></tbody></table>

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409716402967)

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.9985%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><strong>Instância da tarefa Separar produtos (Grupo Material de limpeza)</strong></p></td></tr></tbody></table>

[\[voltar ao topo\]](#top)