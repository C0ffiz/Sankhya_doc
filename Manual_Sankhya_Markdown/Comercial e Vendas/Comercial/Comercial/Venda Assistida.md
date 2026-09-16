# Venda Assistida

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/4466143201431-Venda-Assistida](https://ajuda.sankhya.com.br/hc/pt-br/articles/4466143201431-Venda-Assistida)

---

# Venda Assistida

<table style="border-collapse: collapse; border-spacing: 0,5;"><tbody><tr><td style="text-align: center; width: 100%;"><pre class="wysiwyg-text-align-justify wysiwyg-code-block"><code class="language-auto"> Módulo: Comercial &gt; Rotinas                Versão disponível: A partir da 4.12</code></pre></td></tr></tbody></table>

---

**![essencial FINAL (1).png](https://ajuda.sankhya.com.br/hc/article_attachments/16949120394519)** Para utilizar essa rotina, sua empresa deve possuir a licença **"30602 - COMERCIAL/W**" e/ou **"30612 - PEDIDO WEB/W"**.

A Venda Assistida possibilita que os lançamentos dos Pedidos de Venda sejam realizados de forma mais ágil e prática, pelos vendedores de telemarketing e também de venda balcão, quando não há o recebimento junto ao próprio vendedor. Esta tela também permite que seja efetuada a consulta e a edição dos pedidos que foram lançados ou excluídos. Para conhecer mais sobre essa funcionalidade acesse o tópico [Consulta de carrinhos](#consultadecarrinhos).

Pode-se ainda, por meio da tela [Config. e Layout da Venda Assistida](https://ajuda.sankhya.com.br/hc/pt-br/articles/4540179213079), definir o layout desta tela, por exemplo, os painéis e/ou campos que serão exibidos na tela, e ainda, as diretrizes que eles deverão seguir.

Ressaltamos que, essa tela foi disponibilizada em forma de MVP (Mínimo produto viável) e não possui todas as funcionalidades disponíveis na [Central de Vendas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612414), tais como Análise de Rentabilidade, Ficha de Parceiro, visualização dos componentes de kits de produto, suporte para venda de produtos com controle adicional de estoque do tipo Grade e Série. Verifique as funcionalidades que abrangem esta tela, no tópico [Funcionalidades](#Funcionalidades).

**Nota:** Não é recomendado utilizar _processos personalizados_ na tela Venda Assistida. Essa prática pode gerar atritos operacionais e comprometer o desempenho do sistema, resultando em baixa performance durante o uso da funcionalidade.

Além disso, a Venda Assistida trabalha com o conceito de carrinho de compras. Dessa forma, não há reserva de estoque e lançamento financeiro durante a elaboração do pedido de venda. As validações ocorrerão após a conclusão do pedido, conforme configuração da TOP utilizada.

<table style="border-collapse: collapse;"><tbody><tr style="height: 74px;"><td style="height: 74px; text-align: center; width: 100%;"><pre class="wysiwyg-code-block"><code class="language-auto"> Para executar esta rotina de forma mais ágil, confira os atalhos
da tela por meio do botão “Outras Opções”, opção "Mapa de Atalhos".</code></pre></td></tr></tbody></table>

Caso haja maiores dúvidas, procure sua unidade Sankhya.

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4467551878679)

---

Conforme apresentado no fluxograma abaixo, existem duas formas de realizar o lançamento de um pedido de venda; iniciando pelo preenchimento das informações dos Detalhes da Negociação ou pela busca dos Produtos. Assim, defina o processo desejado e conheça cada etapa a ser efetuada clicando no fluxograma.

<table style="border-collapse: collapse;"><tbody><tr style="height: 22px;"><td style="height: 22px; text-align: center; width: 24.2857%;" colspan="7"><img src="/hc/article_attachments/42312209075991" alt="mceclip27.png"></td></tr><tr style="height: 58px;"><td style="height: 129px; text-align: right; width: 24.2857%;" rowspan="3"><img src="/hc/article_attachments/42312225518871" alt="mceclip8.png" width="140" height="157"></td><td style="height: 58px; width: 18.8572%;"><a href="#detalhesdanegocia%C3%A7%C3%A3o" target="_self"><img src="/hc/article_attachments/42312225519639" alt="mceclip10.png"></a></td><td style="height: 58px; text-align: center; width: 6.42854%;"><img src="/hc/article_attachments/42312209078295" alt="mceclip22.png"></td><td style="height: 58px; width: 18.8571%;"><a href="#painelprodutos" target="_self"><img src="/hc/article_attachments/42312225521559" alt="mceclip14.png"></a></td><td style="height: 58px; text-align: center; width: 6.28591%;"><img src="/hc/article_attachments/42312225522583" alt="mceclip22.png"></td><td style="height: 58px; width: 19.2857%;"><a href="#painelapoio%C3%A0svendas" target="_self"><img src="/hc/article_attachments/42312225523223" alt="mceclip15.png"></a></td><td style="height: 129px; width: 5.99994%;" rowspan="3"><img src="/hc/article_attachments/42312225523735" alt="mceclip13.png" width="29" height="46"></td></tr><tr style="height: 13px;"><td style="height: 13px; width: 18.8572%;">&nbsp;</td><td style="height: 13px; width: 6.42854%;">&nbsp;</td><td style="height: 13px; width: 18.8571%;">&nbsp;</td><td style="height: 13px; width: 6.28591%;">&nbsp;</td><td style="height: 13px; width: 19.2857%;">&nbsp;</td></tr><tr style="height: 58px;"><td style="height: 58px; width: 18.8572%;"><a href="#concluir" target="_self"><img src="/hc/article_attachments/42312209083799" alt="mceclip16.png"></a></td><td style="height: 58px; width: 6.42854%;"><img src="/hc/article_attachments/42312209084311" alt="mceclip20.png"></td><td style="height: 58px; width: 18.8571%;"><a href="#irparaocarrinho" target="_self"><img src="/hc/article_attachments/42312225525911" alt="mceclip17.png"></a></td><td style="height: 58px; width: 6.28591%;"><img src="/hc/article_attachments/42312209084311" alt="mceclip20.png"></td><td style="height: 58px; width: 19.2857%;"><a href="#adicionaraocarrinho" target="_self"><img src="/hc/article_attachments/42312209085207" alt="mceclip18.png"></a></td></tr><tr style="height: 79px;"><td style="height: 79px; width: 24.2857%;" colspan="2"><img src="/hc/article_attachments/42312209086103" alt="mceclip23.png" width="179" height="88"></td><td style="height: 79px; width: 6.42854%;">&nbsp;</td><td style="height: 79px; width: 18.8571%;">&nbsp;</td><td style="height: 79px; width: 6.28591%;">&nbsp;</td><td style="height: 79px; width: 19.2857%;">&nbsp;</td><td style="height: 79px; width: 5.99994%;">&nbsp;</td></tr><tr style="height: 58px;"><td style="height: 58px; text-align: right; width: 24.2857%;"><img src="/hc/article_attachments/42312225528599" alt="mceclip26.png" width="124" height="51"></td><td style="height: 58px; width: 18.8572%;"><a href="#painelprodutos" target="_self"><img src="/hc/article_attachments/42312225521559" alt="mceclip14.png"></a></td><td style="height: 58px; width: 6.42854%;"><img src="/hc/article_attachments/42312225529239" alt="mceclip6.png" width="36" height="22"></td><td style="height: 58px; width: 18.8571%;"><a href="#painelapoio%C3%A0svendas" target="_self"><img src="/hc/article_attachments/42312225523223" alt="mceclip15.png"></a></td><td style="height: 58px; width: 6.28591%;"><img src="/hc/article_attachments/42312225529239" alt="mceclip6.png" width="37" height="22"></td><td style="height: 58px; width: 19.2857%;"><a href="#adicionaraocarrinho" target="_self"><img src="/hc/article_attachments/42312209085207" alt="mceclip18.png"></a></td><td style="height: 138px; width: 5.99994%;" rowspan="3"><img src="/hc/article_attachments/42312209089943" alt="mceclip9.png" width="28" height="46"></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 24.2857%;">&nbsp;</td><td style="height: 22px; width: 18.8572%;">&nbsp;</td><td style="height: 22px; width: 6.42854%;">&nbsp;</td><td style="height: 22px; width: 18.8571%;">&nbsp;</td><td style="height: 22px; width: 6.28591%;">&nbsp;</td><td style="height: 22px; width: 19.2857%;">&nbsp;</td></tr><tr style="height: 58px;"><td style="height: 58px; width: 24.2857%;">&nbsp;</td><td style="height: 58px; width: 18.8572%;"><a href="#concluir" target="_self"><img src="/hc/article_attachments/42312209083799" alt="mceclip16.png"></a></td><td style="height: 58px; width: 6.42854%;"><img src="/hc/article_attachments/42312225530135" alt="mceclip0.png" width="33" height="20"></td><td style="height: 58px; width: 18.8571%;"><a href="#detalhesdanegocia%C3%A7%C3%A3o" target="_self"><img src="/hc/article_attachments/42312225519639" alt="mceclip10.png"></a></td><td style="height: 58px; text-align: right; width: 6.28591%;"><img src="/hc/article_attachments/42312225530135" alt="mceclip0.png" width="34" height="21"></td><td style="height: 58px; width: 19.2857%;"><a href="#irparaocarrinho" target="_self"><img src="/hc/article_attachments/42312225525911" alt="mceclip17.png"></a></td></tr><tr><td style="width: 24.2857%;" colspan="7"><img src="/hc/article_attachments/42312225531159" alt="mceclip3.png"></td></tr></tbody></table>

---

#### **Detalhes da Negociação**

Esta tela permite a inclusão de produtos ao carrinho sem a necessidade de identificar o Parceiro, o Tipo de Negociação e o Tipo de Operação. Quando não informado, o preço que será mostrado para os produtos consultados será baseado na tabela de preço zero. Já quando informado esses dados, o preço praticado nos produtos será baseado na tabela de preço conforme a configuração aplicada no parâmetro **"Tabela de Preços por: - TIPTABPRECOS"**.

**Observação:** na Venda Assistida, deve-se trabalhar exclusivamente com uma única tabela.

 ![Atenção FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16949292321559) A tela **Venda Assistida** não utiliza a configuração do campo **"Usar como preço"** da aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abageral) da [TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114) para definição do **"Valor Unitário"** do produto no carrinho, pois este valor é preenchido com base na tabela de preços.

Optando por não informar os dados em Detalhes da Negociação, para realizar o lançamento de um pedido de venda, basta efetuar a consulta do produto desejado e adicioná-lo ao carrinho, informando os campos em Detalhes da Negociação ao final da venda, por meio do botão **"Detalhes da Negociação"**.

**Nota:** o preço dos produtos adicionados ao carrinho, serão atualizados conforme configuração dos parâmetros **"Tabela de Preços por: - TIPTABPRECOS"** e **"Recalcula preços quando altera Tipo de Negociação: - RECPRECOTPV"**.

Já para os casos em que a empresa trabalha com tabelas de preços diferenciadas, tal como, a tabela de preço por parceiro, primeiramente é necessário informar os dados da negociação, como, por exemplo, a **"Empresa"** que efetuará a venda, o **"Parceiro"**, o **"Tipo de Negociação"**, entre outras. Desse modo, acione o botão Detalhes da Negociação e preencha essas informações no pop-up:

![detalhes-da-negociacao-venda-assistida.png](https://ajuda.sankhya.com.br/hc/article_attachments/24970544560535)

Depois, clique em **"Salvar"**. Feito isso, você poderá conferir no painel superior os dados preenchidos no pop-up:

![mceclip5.png](https://ajuda.sankhya.com.br/hc/article_attachments/4468268780183)

<table style="border-collapse: collapse;"><tbody><tr><td style="width: 100%;"><pre class="wysiwyg-code-block"><code class="language-auto"> Caso seja necessário alterar alguma das informações preenchidas no pop-up, basta
            clicar novamente no botão Detalhes da Negociação e editar os dados.</code></pre></td></tr></tbody></table>

**Observação:** se um evento de liberação de item for registrado na tabela TSILIB e o botão ![Botão remover FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/21293375745047) **"Remover Pedido \[F9\]"** for acionado, o sistema irá automaticamente excluir da tabela TSILIB o evento gerado para o produto que está sendo removido.

---

**Botão Ficha de Parceiro**

**Dica:** utilize o atalho **"Control+Alt+F"** para acessar esta funcionalidade de forma rápida.

O botão ![Botão Ficha de Parceiro FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/19427030909463) Ficha de Parceiro dá acesso a tela [Ficha de parceiro](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601934-Ficha-de-Parceiros), que permite a consulta de informações sobre a situação financeira dos parceiros, incluindo vencimentos e pagamentos de receitas e despesas. Dessa forma, é possível obter dados relevantes para a definição das negociações com o parceiro.

Ao acionar este botão, o sistema abrirá a tela Ficha de parceiro com os dados do parceiro informado no cabeçalho da nota. Caso esse parceiro seja alterado, é necessário clicar no botão **"Usar Parceiro"** para substituir o parceiro definido por meio do botão Detalhes da Negociação. Observe:

![Botão Usar parceiro.gif](https://ajuda.sankhya.com.br/hc/article_attachments/19427046552983)

Se o parceiro não estiver preenchido no cabeçalho da nota, o mesmo poderá ser informado ao abrir a tela, por meio do campo **"Parceiro"**.

Para retornar a tela Venda Assistida, basta acionar o botão **"Voltar"**.

---

![informações adicionais FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/18912674975767) **Informações adicionais referentes à aplicação de descontos:** 

Dado que as configurações abaixo sejam realizadas:

![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28451005929879) Os Produtos a serem utilizados nas vendas com seus devidos descontos inseridos na sub-aba **"Regras"** da tela [Tabela de Preços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603854-Tabelas-de-Pre%C3%A7os);  
![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28451005929879) Na tela [Descontos Promocionais](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044600034), o Produto seja informado no desconto a ser utilizado;

![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28451005929879) O desconto promocional será aplicado no carrinho de compras somente quando os campos Tipo Negociação, Empresa e Tipo Operação estiverem preenchidos. Esses campos são apresentados por meio do botão Detalhes da Negociação.

**Observação:** caso o desconto promocional seja associado a um parceiro, o campo Parceiro também deve ser preenchido para que o desconto seja aplicado.

![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28451005929879) Por fim, configurar o [Tipo de Negociação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045109173) que será utilizado nas vendas com desconto.

Desse modo, teremos que:

![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28451005929879) Quando o campo **"Tipo da taxa"** da aba [Características](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045109173-Tipos-de-Negocia%C3%A7%C3%A3o#abacaractersticas) da tela Tipos de Negociação for configurado com a opção **"Desconto"**, ao incluir um item o sistema irá atualizar o preço do produto e subtrair o valor do preço de tabela, além de aplicar o desconto.  
![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28451005929879) Porém, se a opção **"Juro taxa Única"** for definida no campo Tipo da taxa, na inclusão do item o sistema irá atualizar o preço do produto com o valor de preço de tabela aplicando os juros.  
![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28451005929879) Por fim, com o campo Tipo da taxa definido com a opção Desconto e na tela Descontos Promocionais possua um **"Percentual"** (aba Características) configurado para o registro do Produto a ser utilizado na venda, o preço do item será atualizado aplicando o desconto no valor de preço de tabela.

**Observação:** caso a opção **"Considerar Maior"** do campo Desconto Promocional seja selecionada, o sistema irá considerar o maior desconto entre o Desconto Promocional e aquele do Tipo de Negociação. Porém, lembre-se que se houver esse desconto, este será considerado apenas quando o parâmetro **"Usar o maior desconto promocional? - USAMAIDESCPROMO"** for habilitado.

![acesse também FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16949313983127) Caso queira saber a funcionalidade de cada opção do campo Desconto Promocional, acesse o artigo [Tipos de Negociação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045109173-Tipos-de-Negocia%C3%A7%C3%A3o#abacaractersticas:~:text=O%20%22-,Desconto%20Promocional,-%22%20inserido%20neste).

---

[\[voltar ao topo\]](#top)

#### **Painel Produtos**

Agora, no painel Produtos busque pelo(s) produto(s) desejado(s), por meio do campo de pesquisa localizado na parte superior do painel. Assim, ao informar o produto, serão apresentados na grade os seguintes dados referentes a ele:

<table style="border-collapse: collapse;"><tbody><tr><td style="width: 33.3333%;"><ul><li data-renderer-start-pos="194" data-list-item-id="e6e2dbf3287a78c5525df89ced4f0bfd1"><p class="wysiwyg-text-align-justify">Código</p></li><li data-renderer-start-pos="194" data-list-item-id="e9d8f91159ed0f270d1fdacb442662e80"><p class="wysiwyg-text-align-justify">Descrição</p></li><li data-list-item-id="e845fe8d2f03c2aae50d6b77f17e08e27">Unidade</li></ul></td><td style="width: 33.3333%;"><ul><li data-list-item-id="e4cc683f3fdadd62d28961d6630aaf466">Preço</li><li data-list-item-id="efb79e1ab69c4cdc99b6fda36f4f47472">Estoque</li></ul></td><td style="width: 33.3333%;"><ul><li data-renderer-start-pos="241" data-list-item-id="e5bdad4629b2271c00a545a341f1b5451">Preço Promoção</li><li data-renderer-start-pos="260" data-list-item-id="e3b6d163d87efacb26f87c264dcdbec1c">Local Promoção</li></ul></td></tr></tbody></table>

![painel\_produtos.png](https://ajuda.sankhya.com.br/hc/article_attachments/9175442193303)

Caso esteja utilizando filtros e/ou layout personalizados, ao clicar no botão ![pesquisar.png](https://ajuda.sankhya.com.br/hc/article_attachments/21739723547671) **"Pesquisar"** sem informar qualquer texto no campo de pesquisa, o resultado trará produtos relacionados ao filtro determinado limitado a configuração feita pelo campo **"Qtd. máx. de registros"** no painel de Produtos. 

No entanto, caso utilize o layout embarcado, padrão do sistema, e realize a pesquisa sem qualquer informação, o resultado será baseado nos filtros, mas será limitado a quantidade de 100 registros.

<table style="border-collapse: collapse;"><tbody><tr><td style="width: 100%;"><pre class="wysiwyg-code-block"><code class="language-auto"> A coluna Estoque é a soma do total disponível de todos os locais ativos de 
estoque .</code></pre></td></tr></tbody></table>

Para facilitar no uso desta rotina, após salvar a inclusão do produto no carrinho, o sistema retornará para o campo de busca com o termo informado já selecionado, para que você possa pesquisar novos produtos de maneira mais rápida. 

![adicionar\_novos\_produtos.gif](https://ajuda.sankhya.com.br/hc/article_attachments/7599509408791)

**Observação:** na tela Venda Assistida é possível registrar os impostos do pedido, tais como: DIFAL, PIS, COFINS e ICMS, essas informações são guardadas na tabela TGLVRDINVR. Porém, diferente da [Central de Vendas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612414-Central-de-Vendas), não existe opção de visualizar os registros desta tabela. 

---

 **![informações adicionais FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/18912674975767) Informações adicionais sobre Produtos com Controle por Local** 

Ao incluir um item com controle por local (configuração realizada no [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#top), aba [Medidas e Estoque](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#abamedidaseestoque), por meio da marcação **"Usa Local"**), o sistema seguirá as seguintes etapas:

1.  Inicialmente, será verificado se o campo **"Local Padrão"** na aba [Impostos/Informações por empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#abaimpostosinformaesporempresa), do Cadastro do Produtos, foi preenchido para a empresa do cabeçalho. Se estiver preenchido, será utilizado esse local padrão.
    
2.  Caso a informação não seja encontrada na tela anterior, o sistema procurará o local preenchido no campo **"Local Padrão"** da aba [Estoque/Preço](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaestoquepreo) nas [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa)**.**
    
3.  Se na tela anterior não houver local definido, o sistema buscará o **"Local Padrão"** informado na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113#abageral) do Cadastro do Produto.
    
4.  Na ausência de local definido até esse ponto, será verificado se há um local determinado no parâmetro **"Local Padrão para Pedidos e Notas- LOCALPADRAO"**, lembrando que esse parâmetro é por usuário.
    
5.  Por último, se o parâmetro **"Informa menor local de armazenagem com estoque - INFMINLOC"** estiver ativado, o sistema buscará na tabela de estoque (TGFEST) o menor local com estoque para esse produto, seguindo as restrições para o local da TOP e a informação do parâmetro **"Filtro de empresas/local de estoque- FILEMPLOCALEST"**.
    

---

Ao acionar o botão ![botão filtros cinza FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16950832597399) **"Filtros"** será possível criar e salvar filtros personalizados para que sejam apresentados na grade apenas os produtos configurados conforme as regras definidas para o filtro. 

![filtro\_venda\_assistida.png](https://ajuda.sankhya.com.br/hc/article_attachments/14781674894231)

Caso seja necessário, também é possível excluir os filtros cadastrados. 

Ainda neste painel, temos o botão ![botão Ver.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16951115946135) **"Detalhes do produto"** que, quando acionado será aberto um pop-up de mesmo nome contendo as características do layout padrão do produto. 

![Detalhes do produto.png](https://ajuda.sankhya.com.br/hc/article_attachments/21703601639191)

Na aba **"****Detalhes"** serão exibidas as informações configuradas nos Detalhes do Produto, por meio do botão ![Botão Outras Opções.. FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16950817568279) **"****Outras Opções..."** da tela [Config. e Layout da Venda Assistida](https://ajuda.sankhya.com.br/hc/pt-br/articles/4540179213079).

 ![essencial FINAL (1).png](https://ajuda.sankhya.com.br/hc/article_attachments/16949120394519) Caso queira visualizar informações diferentes das apresentadas no painel Detalhes do Produto, basta criar um novo layout através da tela [Config. e Layout da Venda Assistida](https://ajuda.sankhya.com.br/hc/pt-br/articles/4540179213079), onde será possível incluir ou remover os campos apresentados neste painel. 

A aba **"Perfil"** é habilitada mediante liberação do opcional **"Telemarketing"**.

Na aba **"Componentes"** é possível consultar os componentes dos produtos similares na grade principal da tela [Consulta de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045109353), assim como, na grade de Produtos Alternativos que apresenta os componentes cadastrados na aba [Componentes](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#abacomponentes) da tela Cadastro de Produtos.

**Observação:** o botão Detalhes do Produto será apresentado também nas abas [Produtos Alternativos](https://ajuda.sankhya.com.br/hc/pt-br/articles/4466143201431#abaprodutosalternativos) e [Produtos Sugeridos](https://ajuda.sankhya.com.br/hc/pt-br/articles/4466143201431#abaprodutossugeridos) da grade Apoio às Vendas.

---

**Configurar consulta de produtos**

É possível definir os critérios de localização dos produtos, por meio do botão **"Outras Opções"**, opção **"Configurar consulta de produtos"**, onde pode-se realizar as seguintes configurações:

O campo **"Tipo de Busca"** possibilita que você alterne o tipo da busca entre **"Contendo..."**, **"Começando com..."** ou **"Palavra Inteira"**. A primeira opção faz com que a busca inclua resultados que contenham o texto digitado. Por exemplo, a busca com o texto "Azul" retornaria resultados como:

*   Pasta Azul;
    
*   Caderno Azul;
    
*   Azul Marinho.
    

Já a busca com a segunda opção denominada **"Começando com..."** mostrará apenas os resultados que comecem com o texto digitado, ou seja, ainda nesse exemplo, a busca do texto "Azul" só retornaria o resultado:

*   Azul Marinho.
    

> Ressaltamos que essas opções **"Contendo..."** e **"Começando com..."** não são aplicáveis em buscas efetuadas em campos do tipo numérico, como, por exemplo, o campo código.

No campo **"Considerar termos digitados"** você define qual será a regra a ser utilizada na consulta indexada por termos, podendo ser **"Todos os termos"** ou **"Qualquer termo"**. Ou seja, quando você digitar mais de uma palavra-chave, poderá decidir se a pesquisa deve retornar apenas os produtos que possuem a descrição com todas as palavras-chaves ou aqueles produtos que contêm apenas uma delas.

**Nota****:** A marcação **"Utiliza na Venda Assistida"** (acessada via _Cadastro de Produtos > Outras Opções > Consulta indexada por termos_) define o comportamento da busca nesta tela:

*   **Se a marcação estiver ATIVADA:** O sistema prioriza a consulta indexada por termos, e as definições de "Configurar consulta de produtos" da Venda Assistida (Tipo de Busca e Considerar termos digitados) **não** serão aplicadas.
    
*   **Se a marcação estiver DESATIVADA:** O sistema passará a respeitar integralmente as regras configuradas na Venda Assistida.
    

Por fim, a marcação **"Buscar também pelo código do produto"**, quando habilitada, fará com que o sistema busque um produto cujo código seja igual ao digitado no campo de pesquisa, exibindo-o na primeira linha do painel Produtos.

[\[voltar ao topo\]](#top)

#### **Painel Apoio às Vendas**

Ao clicar em um dos registros do painel Produtos, nas abas localizadas no painel Apoio às Vendas, você poderá verificar as seguintes informações:

<table style="border-collapse: collapse;"><tbody><tr><td style="width: 42.0475%;"><a href="#abadetalhesdeestoque" target="_self"><img src="/hc/article_attachments/42312209091351" alt="Aba_detalhes_de_estoque.jpg"></a></td><td style="width: 16.3334%;">&nbsp;</td><td style="width: 41.619%;"><a href="#abaprodutossugeridos" target="_self"><img src="/hc/article_attachments/42312225532311" alt="Aba_Produtos_Sugeridos_1.jpg"></a></td></tr><tr><td style="width: 42.0475%;"><a href="#abadetalhesdepre%C3%A7o" target="_self"><img src="/hc/article_attachments/42312225533335" alt="Aba_detlahes_de_pre_o_1.jpg"></a></td><td style="width: 16.3334%;">&nbsp;</td><td style="width: 41.619%;"><a href="#abareservas" target="_self"><img src="/hc/article_attachments/42312225537431" alt="Aba_Reservas_1.jpg"></a></td></tr><tr><td style="width: 42.0475%;"><a href="#abaprodutosalternativos" target="_self"><img src="/hc/article_attachments/42312225538199" alt="Aba_Produtos_Alternativos_1.jpg"></a></td><td style="width: 16.3334%;">&nbsp;</td><td style="width: 41.619%;">&nbsp;</td></tr></tbody></table>

---

![Atenção FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16949292321559) Todas as abas deste painel estão ligadas diretamente ao carregamento do painel Produtos. Portanto, mesmo que seja criado um [componente de BI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044605354) em uma aba personalizada, esta dependerá do carregamento do painel Produtos ainda que existam apenas informações do Parceiro no componente de BI.

**Aba Detalhes de estoque**

Nesta aba, confira a disponibilidade de estoque dos produtos. 

![mceclip3.png](https://ajuda.sankhya.com.br/hc/article_attachments/4587450430615)

<table style="border-collapse: collapse;"><tbody><tr style="height: 74px;"><td style="height: 74px; text-align: center; width: 100%;"><pre class="wysiwyg-code-block"><code class="language-auto"> Para filtrar apenas locais de estoque permitidos para a venda dos 
   produtos, crie um filtro personalizado, por meio do botão  "Filtros". </code></pre></td></tr></tbody></table>

Caso você queira adicionar o produto ao carrinho por esse painel, clique duas vezes sobre o registro.

[\[voltar ao subtítulo\]](#painelapoio%C3%A0svendas) 

**Aba Detalhes de preço**

Consulte nesta aba, os detalhes do preço de venda do produto.

![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/4474462237207)

Quando você realizar a consulta de um produto que possui Controle Adicional do tipo **"Lista"** ou **"Número do Lote"**, cadastrado na tela [Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113), aba [Medidas e Estoque](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113#abamedidaseestoque), sub-aba [Controle Adicional](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113#sub-abacontroleadicional), e o parâmetro **"Controla Preços por Controle? - PRECOPORCONT"** estiver ligado, será apresentado o campo **"Controle"**, onde pode-se visualizar o preço do produto de acordo com o controle selecionado.

O campo Controles também é exibido quando o produto selecionado possui cadastro de desconto na tela [Desconto Promocional](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044600034), com a marcação **"Usa desconto por controle"** ativa.

![mceclip3.png](https://ajuda.sankhya.com.br/hc/article_attachments/4475436248855)

De forma semelhante, o campo **"Locais"** será exibido na tela quando o parâmetro **"Controla Preços por Local? - PRECOPORLOC"** estiver ligado. Nele, você poderá visualizar o preço do produto para diferentes Locais. 

Ainda nesse contexto, temos que, os preços serão exibidos conforme a [Tabelas de Preços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603854-Tabelas-de-Pre%C3%A7os) configurada para os locais e controles do produto selecionado, em conformidade com a ativação dos parâmetros **"Controla Preços por Local? - PRECOPORLOC"** e **"Controla Preços por Controle? - PRECOPORCONT".**

![mceclip5.png](https://ajuda.sankhya.com.br/hc/article_attachments/4475524666135)

Pode-se verificar também, por meio do painel **"Desconto promocional por quantidade"** as informações dos descontos promocionais, como o **"% Desconto"**, o **"Vlr. Desconto"**, o **"Preço"**, entre outras.

Esse painel será exibido quando o produto selecionado estiver cadastrado na tela Desconto Promocional, com a marcação **"Usa desconto por quantidade"** ativa e os descontos cadastrados na aba **"Geral"**.

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4484539811095)

---

<table style="border-collapse: collapse;"><tbody><tr><td style="text-align: center; width: 100%;" colspan="3"><img src="/hc/article_attachments/42312209096215" alt="mceclip4.png"></td></tr><tr style="height: 156px;"><td class="wysiwyg-text-align-justify" style="height: 156px; width: 46.4286%;">Nas abas <span class="wysiwyg-underline">Detalhes de preço</span> e&nbsp;<span class="wysiwyg-underline">Detalhes de estoque</span>, caso o produto tenha unidade alternativa cadastrada na tela <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113" target="_blank" rel="noopener noreferrer">Produtos</a>, aba <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113#abaunidadesalternativas" target="_blank" rel="noopener noreferrer">Unidade Alternativas</a>, no painel lateral serão exibidos os botões de acordo com a unidade configurada, para que você possa visualizar e efetuar as vendas dos produtos na unidade desejada.</td><td style="width: 3.57143%;">&nbsp;</td><td style="height: 192px; width: 50%;"><img src="/hc/article_attachments/42312209097111" alt="unidade.gif"></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 100%;" colspan="3"><img src="/hc/article_attachments/42312225540503" alt="mceclip28.png"></td></tr></tbody></table>

---

[\[voltar ao subtítulo\]](#painelapoio%C3%A0svendas)

**Aba Produtos Alternativos**

Nesta aba, serão listados os produtos cadastrados na tela de [Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113), aba [Produtos Alternativos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#abaprodutosalternativos), que podem substituir outros produtos por terem características semelhantes. 

![mceclip15.png](https://ajuda.sankhya.com.br/hc/article_attachments/4488818701335)

Caso o parâmetro **"Permite cadastro de produtos substitutos? - PERCADPRODSUBST"** esteja ligado e o parâmetro **"Tipo de direção para considerar na visualização de Produtos alternativos - TIPDIRPROALT"** esteja definido como **"Bidirecional"**, quando você consultar, por exemplo, pelo produto X que possui os produtos Y e Z como alternativos, o sistema irá considerar que os produtos Y e Z terão X como alternativo dele, mas não serão alternativos entre si.

[\[voltar ao subtítulo\]](#painelapoio%C3%A0svendas)

**Aba Produtos Sugeridos**

Você poderá consultar nesta aba, os produtos cadastrados na tela [Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113), aba [Produtos sugeridos para venda](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113#sub-abacontroleadicional), que poderão ser utilizados como sugestão ao cliente.

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4497153094167)

[\[voltar ao subtítulo\]](#painelapoio%C3%A0svendas) [\[voltar ao topo\]](#top)

**Aba Reservas**

Nesta aba pode-se consultar as reservas do Produto que está sendo negociado.

![aba\_reserva.png](https://ajuda.sankhya.com.br/hc/article_attachments/12810583684759)

Você poderá visualizar essa aba em modo grade ou em modo formulário, sendo que, quando os campos forem configurados para serem exibidos no modo formulário, aqueles referentes ao número do pedido, empresa, parceiro e vendedor, contarão com o recurso de link, em que, ao clicar sobre eles, você será redirecionado para as telas correspondentes aos seus cadastros. Lembrando que, estas telas só serão abertas se o usuário logado tiver acesso liberado as mesmas.

Observe:

*   **Nro Único**: será aberta a [Central de Vendas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612414) já com o Pedido selecionado;
    
*   **Cód. ou nome da Empresa**: será aberta a tela [Empresas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112913) com a Empresa selecionada;
    
*   **Cód. ou nome do Parceiro**: será aberta a tela [Parceiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494) com o Parceiro selecionado;
    
*   **Cód. ou nome do Vendedor**: será aberta a tela [Vendedores/Compradores](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045111133) com o Vendedor selecionado.
    

[\[voltar ao subtítulo\]](#painelapoio%C3%A0svendas) [\[voltar ao topo\]](#top)

---

#### **Adicionar ao carrinho**

Agora que você já verificou as informações complementares dos produtos no painel Apoio às Vendas, adicione os produtos desejados no carrinho por meio do botão ![Botão Adicionar produto FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16951127407767)  **"Adicionar ao carrinho"**. Ao acionar este botão, o produto será apresentado na grade **"****Itens do carrinho"**, onde pode-se informar a **"Quantidade"**, a **"Unidade"**, o **"Local"**, entre outras.  

![gif\_17.gif](https://ajuda.sankhya.com.br/hc/article_attachments/8131463578775)

**Observações:** 

*   O campo Local origem da grade Itens do Carrinho será preenchido automaticamente apenas se o produto for selecionado por meio da aba [Detalhes de Estoque](https://ajuda.sankhya.com.br/hc/pt-br/articles/4466143201431-Venda-Assistida#abadetalhesdeestoque).
    
*   Com o parâmetro **"Pode alterar Vlr. Unit. Liq.? - EDITVLRUNITLIQ"** ligado, o campo **"Preço líq."** da grade Itens do carrinho será habilitado para edição. Ao informá-lo com um valor inferior ao definido na tabela do produto, o sistema preencherá automaticamente os campos **"% desconto"** e **"Vlr. desconto"**.
    

Realizadas as alterações, clique em **"Salvar"**. Em seguida, caso você queira incluir novos produtos, clique novamente no botão Adicionar ao carrinho.

![dica FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16949085020439) É possível executar esta rotina de maneira mais eficiente utilizando as teclas do seu teclado. Observe:

*   Ao adicionar o produto ao carrinho, o sistema direcionará automaticamente o foco no primeiro campo editável da grade Itens do Carrinho.
    
*   Para avançar para o próximo campo editável, pressione a tecla **"Tab"**. Se desejar retornar ao campo anterior, utilize as teclas **"Shift+Tab"**.
    
*   Por fim, ao pressionar a seta para baixo, o sistema salvará esse registro e retornará o foco ao campo de busca.
    

**Observação:** se um evento de liberação de item for registrado na tabela TSILIB e o botão ![Botão Remover produtos selecionados do carrinho FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/21293423632791) **"Remover produtos selecionados do carrinho"** ou  **![Botão Limpar produtos do carrinho FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/21293485536151) "Limpar produtos do carrinho"** for acionado, o sistema irá automaticamente excluir da tabela TSILIB o evento gerado para o produto que está sendo removido.

[\[voltar ao topo\]](#top)

#### **Ir para o carrinho**

Com os produtos adicionados, clique em **"Ir para o carrinho"**, assim você será direcionado a uma nova tela com o resumo do pedido. Nela, você pode editar as informações dos **"Itens do Carrinho"** e os **"Detalhes da Negociação"**.

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4581977110295)

Além disso, na parte inferior temos as **"Informações complementares"**, sendo que, na aba **"Financeiros"** você pode visualizar os dados financeiros do pedido que serão lançados na [Movimentação Financeira](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114753).

Nesta aba, tem-se o botão ![Botão Ações FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16950859958167) **"****Ações"**, onde é possível realizar a criação de ações personalizadas configuradas na tela [Dicionário de Dados](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044597294). 

Na aba **"Transporte"** você pode preencher as informações a respeito do frete do documento que está sendo lançado, tais como, o **"Parceiro Transportadora"**, a **"Quantidade de Volumes"** destinados à carga da nota, qual será o **"Tipo do frete"**, ou seja, se **"Incluso"** ou **"Extra nota"**, entre outras informações.

Para que a despesa acessória do Tipo do frete Incluso seja considerada no valor total do pedido é necessário observar os seguintes requisitos: 

*   Na tela [Tipos de Operação TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114), as marcações **"Soma ST no total da nota"** (aba [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abaimpostos)) e **"S.T. proporcional para Frete"** (aba [Despesas Acessórias](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abadespesasacessrias)) devem estar habilitadas;
    
*   No [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113), aba [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos#abaimpostos), o campo **"Tipo de substituição"** deve estar configurado;
    
*   No [Cadastro de Parceiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494), aba [Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros#abafiscal), os campos **"Código Sit.Trib.IPI Entrada"** e **"Código Sit.Trib.IPI Saída"** devem estar preenchidos;
    
*   A [Alíquota de ICMS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044602934) também deve estar devidamente configurada.
    

**Observação:** atualmente, na Venda Assistida não existem recursos para aplicar o Desconto no total do carrinho; sendo assim, somente será possível inserir o Desconto por item.

[\[voltar ao topo\]](#top)

#### **Concluir**

Realizadas as configurações e as conferências do pedido, clique no botão ![botão-concluir-FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16950926393495) **"Concluir"**. Assim, será apresentado um pop-up com as informações do **"Nro Único"**, **"Nro. Nota"** e **"Vlr. Nota"**. Além disso, você pode abrir o pedido na [Central de Vendas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612414), por meio do botão **"Abrir Pedido"**, ou no [Portal de Vendas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612654), por meio do botão **"Mostrar no Portal"**.

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4586963978007)

Ainda neste pop-up, temos o botão **"Faturar"**, sendo que, por meio da configuração realizada no parâmetro **"Opção de Faturamento na Central de Vendas - TIPFATCENTRAL"** você pode determinar qual o tipo de faturamento será trabalhado aqui. Temos as seguintes opções:

*   Faturar Direto;
    
*   Faturar pelo Estoque;
    
*   Faturar pelo Estoque deixando pendente.
    

**Observação:** ao definir a opção Fatura pelo Estoque deixando pendente, quando a opção Faturar do Pedido de Venda for selecionada, o faturamento será realizado conforme quantidades em estoque, de forma que o pedido de venda com a coluna **"Pendente"** esteja configurado como **"Sim"**. 

Além disso, visando um controle maior sobre os usuários que podem ou não realizar faturamentos de pedidos de venda, tem-se o parâmetro **"Controla acesso de faturamento para pedidos? - CONTROLAFATPED"**, que, quando habilitado, fará com que o acesso ao faturamento de pedidos de venda seja concedido aos usuários através da marcação ou não do acesso especial Faturar, presente na tela [Acessos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044596854-Acessos), módulo Comercial > Rotinas > Venda Assistida e Pedido Web > Venda Assistida. 

**Nota**: o módulo Pedido Web > Venda Assistida esta disponível a partir da versão 4.14.

Pode-se ter as seguintes situações:

*   Caso o parâmetro mencionado esteja habilitado, e o acesso especial Faturar desmarcado, o botão Faturar ficará indisponível para o usuário;
    
*   Caso o parâmetro esteja habilitado, e o acesso especial Faturar marcado, o botão Faturar ficará disponível para o usuário;
    
*   Caso o parâmetro esteja desabilitado, o botão Faturar estará disponível para o usuário, independente da marcação do acesso especial Faturar.
    

**Configurações necessárias para manter o registro no carrinho**

Para manter na Venda Assistida os registros de vendas que podem ser reaproveitados para vendas recorrentes, siga os passos abaixo: 

1.  Ligue o parâmetro **"Manter registros da Venda Assistida ao concluir - MANVDACONC"** para que os registros na tela de Venda Assistida sejam mantidos para futuras duplicações;
    
2.  Em seguida, configure o parâmetro **"Qtde dias P/manter Carrinho convertido em ped. venda - QTDIAMANCARVEN"** para definir por quantos dias um carrinho de venda da Venda Assistida será mantido na base de dados após ser associado a um pedido de venda gerado na [Central de Vendas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612414-Central-de-Vendas). Por padrão, esse parâmetro está configurado para 30 dias, sendo o valor máximo permitido 90 dias.
    

**Nota:** uma vez que um pedido seja gerado na Central de Vendas através da Venda Assistida, o usuário não poderá incluir, alterar ou excluir itens. Para garantir maior segurança nesse processo, habilite o parâmetro **"Bloqueia alterações de pedidos da venda assistida? - BLOQCENTPEDVR"**. Se o parâmetro estiver desativado, o carrinho na Venda Assistida poderá apresentar produtos e quantidades diferentes do pedido de venda. 

**Observação:** a tabela TGFCVRQTD armazenará a quantidade de carrinhos que foram convertidos em pedidos de venda. Essa tabela é utilizada exclusivamente para gerar indicadores de quantos orçamentos foram transformados em pedidos de venda. Não há uma tela específica para visualizar os dados dessa tabela. 

[\[voltar ao topo\]](#top)

#### **Consulta de carrinhos**

Você pode verificar todos os carrinhos que foram excluídos ou salvos, mas que não foram concluídos por meio do botão ![botão-consulta-carrinhos-FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16951013562391) **"Consulta carrinhos"**.

![mceclip9.png](https://ajuda.sankhya.com.br/hc/article_attachments/4588681704087)

Assim, ao acionar o botão, será aberta uma nova tela, nela aplique primeiramente os filtros desejados, sendo eles:

No campo **"Tipos de Carrinhos"** você pode selecionar o tipo de busca dos registros, de acordo com as opções abaixo:

*   **Todos:** serão exibidos todos os carrinhos abertos e excluídos;
    
*   **Abertos:** serão apresentados somente os carrinhos que ficarão abertos e/ou pendentes;
    
*   **Excluídos:** serão exibidos somente os carrinhos que foram excluídos em algum momento, mas ainda estão disponíveis para recuperação;
    
*   **Concluídos:** exibirá os carrinhos de vendas finalizados, ou seja, aqueles que já geraram um registro na [Central de Vendas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612414-Central-de-Vendas). 
    

Sendo que, os carrinhos do tipo Aberto, serão mantidos nesse status conforme o período definido no parâmetro **"****Qtd. dias p/ manter carrinho aberto (CVR) - QTDIASCARABCVR"**, cujo padrão é 30 (trinta) dias. Após esse período, os carrinhos serão automaticamente alterados para o tipo Excluídos.

Já para os carrinhos do tipo Excluídos, esses serão mantidos no período definido no parâmetro **"Qtd. dias p/ manter carrinho lixeira (CVR) - QTDIASCARLXCVR"**, cujo padrão é 7 (sete) dias, sendo excluídos definitivamente do banco de dados após esse período.

A marcação **"Meus Carrinhos"** quando habilitada, fará com que seja apresentado todos os carrinhos abertos do usuário logado.

Você também pode, realizar a busca pelo código do **"Parceiro"** e/ou **"Empresa"**, pelo período que foi negociado o carrinho por meio do campo **"Data de Negociação"**, e ainda, pelo **"Nro Pedido"**. 

Ao clicar em ![botão Aplicar.FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16951024336791) **"Aplicar"**, os registros serão exibidos no painel, sendo que, você poderá selecionar qualquer um deles para recuperar e realizar a edição e a conclusão. Para isso, basta clicar duas vezes sobre o registro desejado ou acionar o botão  **![botão-abrir-carrinho-FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16951038081047) "Abrir Carrinho"**.

Para duplicar o registro é necessário ligar o parâmetro **"Permite duplicar pedidos/notas? - PODEDUPNF"**. Após essa configuração, o botão ![botao-duplicar FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/22589293913879) **"Duplicar"** será disponibilizado. Ao acioná-lo, o pop-up **"Duplicar/Copiar Carrinho"** será exibido.

![Pop-up Duplicar-Copiar Carrinho.png](https://ajuda.sankhya.com.br/hc/article_attachments/22589293916311)

Caso queira que o registro seja duplicado com os preços atualizados, acione a marcação **"Atualiza preço"**. No entanto, se preferir apenas duplicar o registro mantendo os preços conforme o pedido de origem, desative a marcação.

**Observação:** ao duplicar o registro, os eventos padrão ou personalizados configurados através da tela [Regras de Negócio](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044598014-Regras-de-Neg%C3%B3cio) serão acionados, caso existam. 

[\[voltar ao topo\]](#top)

####   .

![funcionalidades.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/19636406772503)

<table style="border-collapse: collapse;"><tbody><tr style="height: 55px;"><td style="height: 55px; width: 50%;"><img src="/hc/article_attachments/42312209097879" alt="funcionalidade É.jpg"></td><td style="height: 55px; width: 50%;"><img src="/hc/article_attachments/42312209098775" alt="funcionalidade não é.jpg"></td></tr><tr style="height: 10px;"><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="e2551ae052fcec826f1ca188da476181a">Ferramenta de venda balcão e televendas;</li></ul></td><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="ed94f5db3ca76fde249190698caa9144b">PDV;</li></ul></td></tr><tr style="height: 10px;"><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="e2a7d872c6a4a2971d0173d2ca2cac95e">Ágil;</li></ul></td><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="e3188e6b3e87b44e044385df05b3e12ce">Não é a Central/Portal de Vendas;</li></ul></td></tr><tr style="height: 10px;"><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="e743fd8cc08ee12ddbdff3cd784b36665">Simples;</li></ul></td><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="e9aaef0cfe69ddb7dca904d4be573f101">Força de vendas;</li></ul></td></tr><tr style="height: 10px;"><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="e975263357b1b306d0df65a4fed34c11c">Intuitivo;</li></ul></td><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="efb09f5ae5b5cb04eeb48b634dc7fd891">Integrado com discador;</li></ul></td></tr><tr style="height: 10px;"><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="efa664013cda92c528e5661d8d271e6fd">Rápido para implantação;</li></ul></td><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="ef4bd3e2a1028bba5bb192b3961f87668">Integrado com agenda de telemarketing;</li></ul></td></tr><tr style="height: 10px;"><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="edf15cd5b0a9ca791d80b6570e46b4eab">Baseado na jornada do vendedor;</li></ul></td><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="eda8e97dbbb848df63e80ac9eb048e7f7">CRM;</li></ul></td></tr><tr style="height: 10px;"><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="e01540d77192633d0cb557fbdd630d2b2">Mais rápido do que a Central de Vendas;</li></ul></td><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="ebb8f10c4f0b74d993a3299933fd49591">Mobile;</li></ul></td></tr><tr style="height: 10px;"><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="e8e498871941c501726de66085e6e6d34"><p class="wysiwyg-text-align-justify">Licenciado no Comercial/W e Pedido Web/W;</p></li></ul></td><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="eb0e205d66757031836fdb526926ff5d1">Off-line;</li></ul></td></tr><tr style="height: 10px;"><td style="height: 10px; width: 50%;">&nbsp;</td><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="e26083f95a88fc4f05a4c0bd5eaa164d0">Não é integrado com plataforma de mensageria.</li></ul></td></tr></tbody></table>

---

<table><tbody><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><img src="/hc/article_attachments/42312225542551" alt="Faz.png"></td><td style="height: 22px; width: 50%;"><img src="/hc/article_attachments/42312209100567" alt="Não faz.png"></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="ec376fb878a5296cdd7ef0eaf213eeb77">Consulta de Produtos indexada;</li></ul></td><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e26236239d391dd357e4421ed1b68ec68">Consulta a análise de rentabilidade;</li></ul></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="ec515580960d55657a8795bd1353b78c9">Pedido de venda;</li></ul></td><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e7091bf8471f2611a595a032c573312ca">Recebimentos financeiros;</li></ul></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="ed838842f685d159dc3db32146daafc2b"><p class="wysiwyg-text-align-justify">Lançamento de carrinho de compras com ou sem informar o parceiro;</p></li></ul></td><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="ed50836c0868cac741678011b98d98f85">Não monta as formas de pagamentos;</li></ul></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e0c94a24b48bb7bef18a4d4a1b698b336">Salvamento automático do carrinho;</li></ul></td><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e9dca466362f340f8ffac04b04b78dd45">Não emite boleto;</li></ul></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e68a010cee851268ad6f51db5f151adc1">Detalhamento de estoque;</li></ul></td><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e8d4e9992cf19d8edb20a4c3a66b9bf5d">Não emite cupom fiscal;</li></ul></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e6da1b29fe8cfb15438610991b2c768a9">Detalhamento de preço;</li></ul></td><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="ed7af2b2d558ddfa70a86fbe8fd866780">Não faz gestão de agenda do vendedor;</li></ul></td></tr><tr style="height: 44px;"><td style="height: 44px; width: 50%;"><ul><li data-list-item-id="edf683e8342f4a082785829518d5f441b"><p class="wysiwyg-text-align-justify">Lançamento de produtos alternativos e sugeridos;</p></li></ul></td><td style="height: 44px; width: 50%;"><ul><li data-list-item-id="e988177a2dca512ae6dff65e7e3f35753">Não faz gestão da agenda de clientes;</li></ul></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e5234ddb4994c8d6bc5b91f16f5ab4f11">Faz lançamento de frete;</li></ul></td><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e2c8ff2f699bc8e717d218d348ddf0d82">Não faz consulta por código de barras;</li></ul></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e8579b9992787e56260762ed5314680fe">Pré-visualização do financeiro;</li></ul></td><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="ec5dfa740d496fc469f5496300734d107">Liberação de limites na própria tela;</li></ul></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e1395466435d0ddf3e862997435670f59">Utilização de teclas de atalho;</li></ul></td><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="ea4b5264391a689ae44dc1d0e92c76826">Sugestão de produtos com inteligência artificial;</li></ul></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e6ad3228a6842609c3b57afb4d82ca15f">Mostra descontos e cálculo de impostos;</li></ul></td><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="eaf1d2ead3dfd838fda1ee9842f150edb">Edição de pedidos concluídos;</li></ul></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="eb4f6d899066eed965f4be337e30d1bc2">Personalização do layout;</li></ul></td><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e2528e83f56d9274e4da44e0057f3c30c">Cadastramento de parceiros, endereço de entrega e contatos;</li></ul></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e7ca3d565ffc549c60ae272c3c6085f9c">Aplicação de descontos no item;</li></ul></td><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e72a4d8ed8698096d0dcda2f8e0b2470c">Reservas de estoque e financeiros durante o lançamento do carrinho;</li></ul></td></tr><tr style="height: 44px;"><td style="height: 44px; width: 50%;"><ul><li data-list-item-id="e93d6745e2ade0cc6bf34b13f169564b5"><p class="wysiwyg-text-align-justify">Mostra histórico de carrinhos abertos e excluídos;</p></li></ul></td><td style="height: 44px; width: 50%;"><ul><li data-list-item-id="ea42cf76ec1ee4c08b56e029b8d97f473">Utilização de preço dinâmico;</li></ul></td></tr><tr style="height: 44px;"><td style="height: 44px; width: 50%;"><ul><li data-list-item-id="ed833f15c6c28025f030564882554223f"><p class="wysiwyg-text-align-justify">Limpeza automática de carrinhos vencidos;</p></li></ul></td><td style="height: 44px; width: 50%;"><ul><li data-list-item-id="e9f52c951a0ffe986a460a122fdfc58f5">Não envia carrinho e pedido via e-mail;</li></ul></td></tr><tr style="height: 67px;"><td style="height: 67px; width: 50%;"><ul><li data-list-item-id="e836e4565aa4994459d3005acdc95d032"><p class="wysiwyg-text-align-justify">Suporta campos adicionais das tabelas detalhes da negociação e itens do carrinho;</p></li></ul></td><td style="height: 67px; width: 50%;"><ul><li data-list-item-id="e4eb869e41f8b5a959603f62ec2b09f80">Reimpressão de pedidos;</li></ul></td></tr><tr style="height: 44px;"><td style="height: 44px; width: 50%;"><ul><li data-list-item-id="ef29bb872677d15134193e5526fcd02f9">Destaca os produtos com descontos promocionais;</li></ul></td><td style="height: 44px; width: 50%;"><ul><li data-list-item-id="ebca482832bf9b6da0f624b252209893f">Devolução de pedidos;</li></ul></td></tr><tr style="height: 22px;"><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="ec3526aebc4a720b783af385528359c13">Execução de botões de ação;</li></ul></td><td style="height: 10px; width: 50%;"><ul><li data-list-item-id="ef5268730b76a0c5459ebc37c9431b844">Visualização e alteração de componentes de kits de produto;</li></ul></td></tr><tr style="height: 44px;"><td style="height: 11px; width: 50%;"><ul><li data-list-item-id="e9166054d7e036b535b6bd7312aec95cd"><p class="wysiwyg-text-align-justify">Transformação do carrinho de compra em pedido de venda na conclusão;</p></li></ul></td><td style="height: 11px; width: 50%;"><ul><li data-list-item-id="ed785b57563f1a1ca480a7727232989d0">Seleção de itens de produtos com controle adicional de estoque do tipo Grade e Série.</li></ul></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e4075c93083130afc3c7c0e4c8844379a">Faturamento de pedido;</li></ul></td><td style="height: 22px; width: 50%;">&nbsp;</td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e774a1cf20e7cf19db48c8a0d8028d461">Consulta as características do produto;</li></ul></td><td style="height: 22px; width: 50%;">&nbsp;</td></tr><tr style="height: 67px;"><td style="height: 67px; width: 50%;"><ul><li data-list-item-id="e422054794a56a19254565b5057870e46"><p class="wysiwyg-text-align-justify">Destaque de cores para produtos sem estoque ou com estoque negativo;</p></li></ul></td><td style="height: 67px; width: 50%;">&nbsp;</td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="ead22fba0eaa100e841f7465fab50a491">Acessa a ficha de parceiro;</li></ul></td><td style="height: 22px; width: 50%;">&nbsp;</td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="eaae8c79cf8cf98ea611aeeac7d50a453"><p class="wysiwyg-text-align-justify">Personalização de informação de estoque dos produtos;</p></li></ul></td><td style="height: 22px; width: 50%;">&nbsp;</td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="eb9df33a9f63d3b3552f6d35b104d6240">Execução das regras de negócio;</li></ul></td><td style="height: 22px; width: 50%;">&nbsp;</td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e6f8efab35b0dcca86db8af85fab197c7"><p class="wysiwyg-text-align-justify">Sugere local de estoque do produto automaticamente;</p></li></ul></td><td style="height: 22px; width: 50%;">&nbsp;</td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e31982ce441901265afa645b06a2a9398"><p class="wysiwyg-text-align-justify">Utiliza as configurações de desconto e/ou juros do tipo de negociação;</p></li></ul></td><td style="height: 22px; width: 50%;">&nbsp;</td></tr><tr style="height: 22px;"><td style="height: 22px; width: 50%;"><ul><li data-list-item-id="e244550d354e805579e86bd1c601a7505">Cria painel personalizado;</li></ul></td><td style="height: 22px; width: 50%;">&nbsp;</td></tr><tr style="height: 44px;"><td style="height: 44px; width: 50%;"><ul><li data-list-item-id="e83da7c87e69d2ea64b7b25c9189fa7bb"><p class="wysiwyg-text-align-justify">Pintar cor da fonte no painel personalizado;</p></li></ul></td><td style="height: 44px; width: 50%;">&nbsp;</td></tr><tr style="height: 44px;"><td style="height: 44px; width: 50%;"><ul><li data-list-item-id="eb36b0504e4f328aa910f8e6fb94ec430"><p class="wysiwyg-text-align-justify">Edição no campo valor líquido (conforme configurações).</p></li></ul></td><td style="height: 44px; width: 50%;">&nbsp;</td></tr></tbody></table>

Além das funcionalidades descritas acima, também é possível que as **"Restrições/Exceções"** por Empresa, Local, Parceiro, Perfil Principal, Tipo de Negociação, Vendedor, Centro de Resultado e Natureza configuradas na TOP sejam aplicadas na Venda Assistida, assim como ocorre na Central de Vendas. Sendo assim, apenas os registros permitidos pela TOP serão apresentados antes da conclusão do pedido pela rotina de Venda Assistida. 

**Observação:** você poderá cadastrar os Detalhes da Negociação, adicionar os itens no carrinho e apenas no final informar o Tipo de Operação. Por conta disso, após informar a TOP que possua Restrições/Exceções configuradas, o sistema fará as validações dos registros informados ao salvar os Detalhes da Negociação.

[\[voltar ao topo\]](#top)

![acesse também FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16949313983127) Acesse também:

[Config. e Layout da Venda Assistida](https://ajuda.sankhya.com.br/hc/pt-br/articles/4540179213079)

[Regras de Negócio](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044598014-Regras-de-Neg%C3%B3cio)