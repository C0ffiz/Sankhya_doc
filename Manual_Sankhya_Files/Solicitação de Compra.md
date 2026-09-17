# Solicitação de Compra

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360045111053-Solicita%C3%A7%C3%A3o-de-Compra](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045111053-Solicita%C3%A7%C3%A3o-de-Compra)

---

# Solicitação de Compra

A solicitação de compra está disponível para os tipos de movimento Pedido de Venda, Pedido de Requisição, Venda e Requisição.

Como a Solicitação de Compra é uma ponte para o módulo de **"Cotação"**, é necessário que você possua o módulo.

Ao efetuar a confirmação de um pedido/nota, o sistema gerará uma solicitação de compra.

####  **![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42312058654743) Configurações para Gerar a Solicitação de Compra na confirmação**

Na tela [Grupos de Produtos/Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044598294-Grupos-de-Produtos-Servi%C3%A7os), a marcação **"Participa da opção "Gerar Solicitação de Compra na Confirmação" do cadastro da top?"** deve estar realizada.

No [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-), aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#abageral), a marcação **"Solicita Compra?"** deve estar realizada.

No [Cadastro de Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP), a marcação **"Gera Solicitação de Compra na Confirmação"** deve estar efetuada.

Caso o parâmetro **"O responsável pela cotação tem que ser comprador?** **RESPCOTCOMPR"** esteja ligado, ao confirmar o lançamento, o sistema exibirá uma tela de pesquisa para que você indique qual comprador será utilizado na geração da solicitação de compra. Para o comprador aparecer nesta tela de pesquisa, é necessário que, no cadastro de Vendedores/Compradores o tipo seja Comprador e o Código do Funcionário tem que ser igual ao Código do Funcionário do Usuário.

####  **![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42312058654743) Gerar Solicitação de Compra através do botão "Outras Opções" nos Portais**

Será possível a geração da Solicitação de Compra, no Portal de Vendas e Portal de Mov. Internas através do botão **"Outras Opções"**. Ao selecionar o título na grade **"Resultado da seleção"**, o sistema habilitará as opções **"Gerar solicitação de compra p/ produtos sem estoque"** e **"Gerar solicitação de compra"**.

Através da opção **"Gerar Solicitação de Compra p/ produtos sem estoque"**, o sistema gerará solicitação de compra para os produtos que não possuem estoque suficiente. A quantidade gerada, será a quantidade do pedido selecionado. O sistema não calcula a diferença solicitada menos a quantidade em estoque.

**Nota:** para que a validação do estoque seja feita é necessário que na tela [Grupos de Produtos/Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044598294), aba [Estoque](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044598294-Grupos-de-Produtos-Servi%C3%A7os#abaestoque), o campo **"Valida estoque"** esteja configurado com uma opção diferente de **"Não Valida"**.  
 

A opção **"Gerar Solicitação de Compra"** criará uma solicitação de compras para os itens do lançamento, de acordo com a quantidade necessária (quantidade negociada - quantidade entregue - quantidade corte).

Caso o produto tenha estoque e mesmo assim você deseje gerar uma solicitação de compra utilizando a opção de Gerar Solicitação de Compra p/ produto sem estoque, o sistema emitirá a mensagem: _**"Não será gerada solicitação de compra, pois os produtos originais já foram todos entregues ou cortados"**_.

**Observação:** essa solicitação de compra é gerada no módulo de cotação da Sankhya.

*   #### Para a geração de **Solicitação de Compra Automática** quando o produto possui estoque disponível:
    
    <table style="border-style: solid; border-width: 1px;"><tbody><tr><td style="border-style: solid; border-width: 1px;"><p data-path-to-node="7,1,0,0"><span class="wysiwyg-font-size-medium"><strong data-path-to-node="7,1,0,0" data-index-in-node="0">Configuração:</strong> É necessário que as configurações de <strong data-path-to-node="7,1,0,0" data-index-in-node="51">Liberação de Limites</strong> para o <strong data-path-to-node="7,1,0,0" data-index-in-node="79">evento 40</strong> ("Solicitação de compra p/ produto em estoque") estejam devidamente ativadas.</span></p><p data-path-to-node="7,1,1,0"><span class="wysiwyg-font-size-medium"><strong data-path-to-node="7,1,1,0" data-index-in-node="0">Comportamento do Sistema:</strong> Neste cenário, o sistema adota um fluxo de controle. Em vez de criar a solicitação de compra de forma direta e automática, o sistema primeiro gerará uma <strong data-path-to-node="7,1,1,0" data-index-in-node="179">pendência de aprovação</strong> para o usuário ou grupo de aprovadores configurado."</span></p></td></tr></tbody></table>
    

#### **![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42312058654743)Previsão de Entrega do Produto**

Na configuração do layout da nota o campo **"Dt. Prev. Entrega"** dos itens, permite que você possa informar a Data de Previsão de Entrega do Produto. Este campo estará disponível para os tipos de movimento **"Pedido de Compra"**, **"Compra"**, **"Pedido de Venda"**, **"Pedido de Requisição"**, **"Requisição"**.

Caso você utilize o Layout Padrão do sistema para estes tipos de movimentos, este campo será visualizado como padrão.

Uma vez preenchido, ao solicitar a compra, seja pelo Pedido de Venda ou Pedido de Requisição ou Requisição, seja na confirmação seja em Outras Opções, o sistema levará esta informação a Solicitação de Compra, no campo Data Entrega.

Configurações necessárias:

*   O campo Dt. Prev. Entrega tem que estar disponível na Grade de Itens da Central de Compras. Para isto, acesse a tela [Configurador de Layout da Nota](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044602634-Configurador-de-Layout-da-Nota) e inclua este campo no Tipo movimento Compra.
    

**Nota:** se o tipo de movimento não permitir a visualização do campo, não será disponibilizado na Grade de Itens.

*   **Evento 40 (Liberação de Limites):** Para que o sistema trate solicitações de produtos que ainda possuem estoque, o evento **"40 - Solicitação de compra p/ produto em estoque"** deve estar ativado e configurado na tela _Tipos de Liberação de Limites_.
    
    **Nota** _:_ isso garantirá que, em vez da geração automática, o sistema crie uma pendência de aprovação.
    
*   No Portal de Vendas, após o preenchimento do campo e confirmação da nota foi gerado a solicitação de compra.
    

A tela de Solicitação de Compra ainda não foi convertida para o Sankhya Om, portanto, será visualizada a Data Entrega pelo MGE.

**Importante:**

*   Quando efetua-se a Entrega de um Pedido de Requisição para uma Requisição, a solicitação de compra será a mesma.
    
*   A opção de Gerar solicitação de compra ou Gerar Solicitação de Compra para produtos sem estoque estará habilitada somente se o lançamento estiver confirmado e não houver solicitação já vinculada.
    
*   Se no lançamento não for informada a Dt.Prev.Entrega, esta irá vazia para o campo Data Entrega na Solicitação de Compra.