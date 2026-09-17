# Divergências de Estoque WMS

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/4417442682903-Diverg%C3%AAncias-de-Estoque-WMS](https://ajuda.sankhya.com.br/hc/pt-br/articles/4417442682903-Diverg%C3%AAncias-de-Estoque-WMS)

---

# Divergências de Estoque WMS

<table style="border-collapse: collapse; width: 100%; height: 58px;" cellspacing="0,5"><tbody><tr style="height: 58px;"><td class="wysiwyg-text-align-center" style="width: 100%; height: 58px;"><pre class="wysiwyg-text-align-justify"><span class="wysiwyg-font-size-medium"><strong><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42311609914391" alt="Módulo 36x36 FINAL.png"> Módulo: </strong>WMS &gt; Inventário                 <strong>    <img src="https://ajuda.sankhya.com.br/hc/article_attachments/42311609915159" alt="Versão - 32x32 FINAL.png"> Versão disponível: </strong>A partir da 4.11</span></pre></td></tr></tbody></table>

---

Esta tela possui acesso restrito a analistas de suporte, administradores do sistema, gestores de operação de estoque de armazém. Com o intuito de auxiliar no diagnóstico das divergências de estoque do WMS são apresentadas nesta tela, duas categorias de análise que podem ser ajustadas:

*   Inconsistência de data de validade;
*   Inconsistência de estoque.

Desse modo, trataremos os seguintes tópicos neste artigo:

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-right" style="width: 43.619%;"><a href="#Configura%C3%A7%C3%B5esdatela" target="_self"><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42311637430167" alt="ICONES__51_.png" width="206" height="180"></a></td><td style="width: 13.3333%;">&nbsp;</td><td style="width: 43.0476%;"><a href="#tiposdediverg%C3%AAncia" target="_self"><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42311637430551" alt="ICONES__52_.png" width="206" height="181"></a></td></tr></tbody></table>

---

### Configurações da tela

Primeiramente no Painel de Filtros, informe a **"Empresa"** para que sejam apresentados os registros que possuem divergência. Para refinar a busca, você pode informar também o **"Produto"**, um **"Complemento"**, a **"Faixa de Endereços"**, o número **"Lote (Controle)** e o **"Parceiro"**.

![mceclip3.png](https://ajuda.sankhya.com.br/hc/article_attachments/4417459532823)

Depois, para os casos de inconsistência de data de validade, configure por meio do botão ![Botão preferências FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16841600447895) as **"Preferências de ajuste do WMS"**. Ao acioná-lo, será exibido um pop-up, onde você pode habilitar uma das seguintes opções:

*   Seleciona a última data de validade conferida no Recebimento;
*   Faz o cálculo da Data de Validade por meio do Shelf Life (Cadastro do Produto): Data Atual + Shelf Life = Data de Validade.

Neste pop-up, defina também a cor de fundo da fonte para cada tipo de divergência. Como neste exemplo, em que para as divergências de data de validade, os registros serão apresentados na cor **azul**. 

![azul.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4420111095575)

Com as configurações acima realizadas, serão exibidos na grade superior os **"Dados de Estoque do WMS"**. Selecionando uma linha nesta grade, na aba **"Data de Validade"** serão apresentados os registros de estoque por data de validade.

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4419745695895)

Se o produto do registro selecionado, estiver com alguma tarefa em aberta pendente, será exibido na aba **"Tarefas Pendentes"**.

Agora, clique em ![Botão Gerar ajustes FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16841523476887) **"Gerar ajustes"** para que o sistema verifique qual cenário de divergência se encontra o registro e realize o processamento de ajuste conforme definição e parâmetros selecionados em tempo de execução. Assim, será apresentada a mensagem:

_**"Será feito o ajuste dos Registros apresentados/selecionados na Grid. Deseja confirmar?"**_

Clicando em **"Sim"**, será exibida as informações dos ajustes:

![mceclip7.png](https://ajuda.sankhya.com.br/hc/article_attachments/4417467839767)

Clicando em **"Não"**, o processo será cancelado.

Com os ajustes realizados, você pode verificar o histórico de execuções, por meio do botão ![Botão Histórico de Ajustes FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16841907746583) **"Histórico de Ajustes"**.

![mceclip8.png](https://ajuda.sankhya.com.br/hc/article_attachments/4417467879703)

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre class="wysiwyg-text-align-justify"><span class="wysiwyg-color-green120"><strong>Dica:</strong></span> Agende os ajustes por meio do botão <img src="https://ajuda.sankhya.com.br/hc/article_attachments/42311637430935" alt="Botão Agendar Relatório FINAL.png" width="36" height="26"> <strong>"Realizar agendamento"</strong>. Ao <br>acioná-lo, você será direcionado a tela <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/4419586448023" target="_blank" rel="noopener noreferrer">Agendador Divergências de Estoque WMS</a>.</pre></td></tr></tbody></table>

[\[voltar ao topo\]](#top)

---

### Tipos de divergência 

Conforme mencionado, essa tela vai identificar dois tipos de divergências: Divergência de Estoque e Divergências de Data de validade. Para um melhor entendimento do que o sistema trata como divergência, vamos mencionar abaixo todos os cenários.

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-right" style="width: 45.2857%;"><a href="#Diverg%C3%AAnciadeestoque" target="_self"><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42311637431575" alt="ICONES__54_.png" width="153" height="92"></a></td><td style="width: 7.99999%;">&nbsp;</td><td style="width: 46.7143%;"><a href="#Diverg%C3%AAnciadedatadevalidade" target="_self"><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42311609919383" alt="ICONES__55_.png" width="153" height="92"></a></td></tr></tbody></table>

---

#### **Divergência de Estoque**

O WMS faz uma "contabilização" de todas as tarefas geradas através das Entradas e Saídas pendentes no estoque, ou seja, para todas as tarefas com status em **"Aberto"**, o sistema tem que identificar a saída de um endereço e entrada em um endereço de destino. 

**Entradas e Saídas Pendentes**

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><strong>Cenário 1</strong></pre></td></tr></tbody></table>

Caso o sistema identifique que existem tarefas Abertas, porém, no sistema não existem saídas pendentes no endereço da tarefa e entradas pendentes no destino da tarefa, o sistema irá identificar como divergências.

**Correção:** Para este cenário, o sistema realizará a auditoria analisando o total de tarefas abertas para a Empresa, Produto, Lote e Endereço, em seguida, será efetuada a correção deixando as Entradas e Saídas, conforme a quantidade de tarefas com a situação **"Aberta"** ou **"Em andamento"**. Considere o exemplo a seguir:

*   Produto: Cerveja Skol 
*   Tarefas em Aberta/Em andamento: 1
*   Endereço de Origem: 01.01
*   Endereço de Destino: 01.02
*   Estoque Endereço: 01.01 | Est: 10UN | Saídas Pend:0| Será Ajustado para 1UN
*   Estoque Endereço: 01.02 | Est: 1UN | Entradas Pend:0| Será Ajustado para 1UN

Essa situação pode ocorrer somente nas saídas, ou somente nas entradas, sendo que, para os dois casos a correção será a mesma.

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><strong>Cenário 2</strong></pre></td></tr></tbody></table>

No momento da auditoria se o sistema identificar que existe Saídas e Entradas pendentes para Endereços, porém, não exista tarefas com a situação **"Aberta"** ou **"Em andamento"**, neste caso o sistema também vai apresentar a divergência.

**Correção:** Como não existem tarefas que justifiquem a saída e a entrada nos endereços com divergência, o sistema vai zerar ou subtrair a quantidade no estoque, deixando de acordo com a contabilização feita de tarefas realmente em aberto/em andamento. Por exemplo:

*   Produto: Cerveja Skol 
*   Tarefas em Aberta/Em andamento: 0
*   Endereço de Origem: 01.01
*   Endereço de Destino: 01.02
*   Estoque Endereço: 01.01 | Est: 10UN | Saídas Pend:1| Será Ajustado para 0UN
*   Estoque Endereço: 01.02 | Est: 1UN | Entradas Pend:1| Será Ajustado para 0UN

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><strong>Cenário 3</strong></pre></td></tr></tbody></table>

Existem casos em que o usuário pode realizar intervenções via banco de dados (não recomendado), nesse cenário essa intervenção pode excluir alguma linha de estoque que contenha Saídas ou Entradas pendentes, deixando assim o estoque com inconsistente. Desse modo, o sistema identificará essa situação na auditoria e aplicará a correção. Considere o seguinte exemplo:

*   Estoque: 20UN | End: 01.01| Saídas Pend: 10UN| (estoque excluído via banco de dados)
*   Estoque: 10UN | End: 01.02| Entrada.Pend: 10UN|(estoque excluído via banco de dados)

**Correção:** O sistema vai retornar o estoque, deixando igual a saídas pendentes e em caso de entradas pendentes, o sistema vai retornar a linha deixando o estoque zerado.

*   Estoque: 10UN | End: 01.01| Saídas Pend: 10UN| (estoque excluído via banco de dados)
*   Estoque: 0UN | End: 01.02| Entrada.Pend:10UN|(estoque excluído via banco de dados)

<table style="border-collapse: collapse; height: 95px; width: 96.015%; margin-right: auto; margin-left: auto;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><span style="font-weight: 400;"><img src="https://ajuda.sankhya.com.br/hc/article_attachments/16841529153687" alt="Atenção FINAL.png"><br>É recomendado neste caso que após a correção, os endereços envolvidos na divergência <br>sejam inventariados devido ao estoque inserido para atender a demanda das saídas pendentes.</span></pre></td></tr></tbody></table>

 **Saídas Pendente maior que o Estoque**

Quando o sistema identificar no estoque que existe quantidade de Saídas pendentes de um Endereço maior que o estoque, então o sistema vai apresentar como divergência, pois na execução das tarefas essa situação pode retornar no coletor a seguinte mensagem:

_**"Essa operação deixará o estoque negativo do endereço:X Produto:Y controle:W."**_

<table style="border-collapse: collapse; height: 95px; width: 96.015%; margin-right: auto; margin-left: auto;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><span style="font-weight: 400;"><img src="https://ajuda.sankhya.com.br/hc/article_attachments/16841529153687" alt="Atenção FINAL.png"><br> Neste caso, não existem entradas pendentes para cobrir as saídas pendentes, assim, o<br>estoque não vai atender a quantidade de saídas, gerando a divergência.</span></pre></td></tr></tbody></table>

Considere o seguinte exemplo desta situação:

*   Produto: 10 |Endereço: 01.01 |Estoque: 10UN| Saídas Pen: 30|

**Correção:** Quando identificada essa inconsistência, o sistema vai igualar o estoque para a mesma quantidade de saídas pendentes, desse modo, a demanda será atendida e a operação será continuada, evitando assim, que a tarefa fique parada ou aguardando outro tipo de intervenção.

*   Produto: 10 |Endereço: 01.01 |Estoque: 30UN| Saídas Pen: 30|

[\[voltar ao subtítulo\]](#tiposdediverg%C3%AAncia)

---

#### **Divergência de Data de Validade**

O controle de Data de validade no WMS é feito por meio de duas tabelas: TGWEST (estoque) e TGWESTVAL (Tabela de data de validade). O controle de Data de validade é um controle que exige mais atenção e critério por parte do setor de Planejamento de Controle de Estoque - PCE, pois deve ter coerência com a quantidade de estoque com a distribuição das datas para o Produto e Lote.

Geralmente esse controle é realizado com um lote tendo apenas uma data, porém existem operações que são registradas na Produção mais de uma Data de validade para o mesmo Lote. Mediante a este contexto, temos algumas situações que o WMS vai realizar a auditoria e identificar algumas inconsistências no estoque com Dt. de validade, conforme os cenários abaixo:

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><strong>Cenário 1</strong></pre></td></tr></tbody></table>

Para os produtos com Shelf Life configurado (tela [Cadastro do Produto](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113), aba [WMS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113#abawms)), que possui estoque, porém, sem registro de Data de validade em ambas as tabelas, temos a seguinte correção:

**Correção:** Nesta tela (Divergências de Estoque WMS) temos a opção **"Preferências de ajuste do WMS"**, que contém duas estratégias para correção do estoque sem data, são elas:

*   Seleciona a última data de validade conferida no Recebimento;
*   Faz o cálculo da Data de Validade por meio do Shelf Life (Cadastro do Produto): Data Atual + Shelf Life = Data de Validade.

Com a estratégia definida, clique na opção de ajuste, desse modo, será registrada a data de validade no estoque, conforme a opção selecionada.

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><strong>Cenário 2</strong></pre></td></tr></tbody></table>

Estoque do produto com Data de validade em somente uma das tabelas de estoque.

**Correção:** O sistema vai inserir a mesma data de validade existente em uma das tabelas, na tabela que não contêm o registro.

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><strong>Cenário 3</strong></pre></td></tr></tbody></table>

Caso tenha divergência de quantidade entre as tabelas, o sistema irá aplicar a seguinte regra:

![Tabela\_de\_estoque.png](https://ajuda.sankhya.com.br/hc/article_attachments/4420120501271)

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><strong>Cenário 4</strong></pre></td></tr></tbody></table>

Caso tenha divergência somente entre as Datas de validade entre as tabelas.

**Correção:** O sistema irá considerar a Data de validade da tabela de Dt. validade como correta, e utilizará para ambas as tabelas.

---

 ![Atenção FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16841529153687) Todas as situações tratadas nesta tela é visando uma melhor gestão da operação, evitando que essas situações impactem na produtividade dos operadores e dos usuários do WMS. 

[\[voltar ao subtítulo\]](#tiposdediverg%C3%AAncia) [\[voltar ao topo\]](#top)