# Aplicação de Desconto na Venda (PDV)

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/43234901082647-Aplica%C3%A7%C3%A3o-de-Desconto-na-Venda-PDV](https://ajuda.sankhya.com.br/hc/pt-br/articles/43234901082647-Aplica%C3%A7%C3%A3o-de-Desconto-na-Venda-PDV)

---

# Aplicação de Desconto na Venda (PDV)

**Módulo:** Vendas › Frente de Caixa (PDV)  
**Caminho de acesso:** Menu Principal › Vendas › Frente de Caixa (PDV)

**Você encontra neste artigo:**

<table style="border-collapse: collapse;" id="sumario"><tbody><tr><td style="border-color: rgb(153, 153, 153); padding: 8px; vertical-align: top; width: 607.333px;"><a href="#oque">O que é e para que serve</a><br><a href="#antes">Antes de começar</a><br><a href="#como">Como usar a tela</a><br><a href="#rodape">Desconto no total da venda (rodapé)</a><br>&nbsp;&nbsp;&nbsp;↳&nbsp;<a href="#rodape-aplicar">Aplicar desconto no total</a><br>&nbsp;&nbsp;&nbsp;↳&nbsp;<a href="#rodape-editar">Editar desconto no total</a><br>&nbsp;&nbsp;&nbsp;↳&nbsp;<a href="#rodape-remover">Remover desconto no total</a><br>&nbsp;</td><td style="border-color: rgb(153, 153, 153); padding: 8px; vertical-align: top; width: 607.333px;"><a href="#item">Desconto no item</a><br>&nbsp;&nbsp;&nbsp;↳&nbsp;<a href="#item-aplicar">Aplicar desconto no item</a><br>&nbsp;&nbsp;&nbsp;↳&nbsp;<a href="#item-editar">Editar desconto no item</a><br>&nbsp;&nbsp;&nbsp;↳&nbsp;<a href="#item-remover">Remover desconto no item</a><br><a href="#atencao">Pontos de atenção</a><br><a href="#faq">Perguntas frequentes</a></td></tr></tbody></table>

## O que é e para que serve

O **Processo Aplicação de Desconto na Venda** permite ao operador de caixa conceder descontos, em percentual ou em valor fixo, sobre o total da venda (rodapé) ou sobre um item específico da grade, dentro da **Tela Frente de Caixa (PDV)**. Ele serve para viabilizar negociações diretas de fechamento com o cliente, respeitando os limites parametrizados no perfil do PDV do operador e, quando existir, o limite de desconto cadastrado no próprio produto. Este processo não altera o cadastro de preços dos produtos nem cria promoções automáticas — os descontos aplicados aqui são pontuais, valem apenas para a venda em andamento e não ficam registrados como parametrização permanente.

![Grade de vendas da Frente de Caixa (PDV) com o painel do produto selecionado e o campo Desconto (item) em destaque](https://ajuda.sankhya.com.br/hc/article_attachments/43234904581271)

---

## Antes de começar

Antes de conceder um desconto na venda, confirme a parametrização abaixo no **Portal Gerencial › Perfil de PDV**, feita pelo administrador do sistema:

*   A marcação **Desconto no total da venda** precisa estar ativa para o operador conceder desconto no rodapé sem senha de gerente.
*   A marcação **Desconto no item** precisa estar ativa para o operador conceder desconto em um item específico sem senha de gerente.
*   O campo **Percentual máximo de desconto** define até quanto o operador pode conceder, nos dois casos, sem autorização do gerente. Acima desse percentual, o sistema sempre solicita a senha de gerente.

**ℹ️ Nota**

Um produto também pode ter um limite próprio de desconto, cadastrado no **Cadastro de Produtos**. Quando existir, esse limite é sempre respeitado — mesmo que o gerente autorize um desconto maior no perfil do PDV. Veja os detalhes em [Limite de desconto do produto](#descmax).

[↑ Voltar ao início](#sumario)

---

## Como usar a tela

Os dois fluxos de desconto só ficam disponíveis depois que há pelo menos um produto na grade de vendas:

*   Para aplicar desconto no **total da venda**, basta ter ao menos um produto adicionado à grade.
*   Para aplicar desconto em um **item específico**, selecione antes a linha do produto na grade — navegue entre os itens com as setas do teclado ou clique diretamente na linha desejada.

[↑ Voltar ao início](#sumario)

---

## Desconto no total da venda (rodapé)

O desconto no total da venda aplica um valor percentual ou fixo sobre o carrinho inteiro. O sistema rateia esse valor proporcionalmente entre os itens elegíveis, considerando o valor total de cada item (quantidade × valor unitário). Itens em promoção ativa e a parcela de cada produto que já ultrapassaria o limite individual de desconto (DESCMAX) ficam de fora do rateio.

![Grade de vendas com desconto no total aplicado, destacando as linhas Desconto Venda e Total da venda no resumo do rodapé](https://ajuda.sankhya.com.br/hc/article_attachments/43234904584343)

### Aplicar desconto no total

1.  Adicione os produtos à venda.
2.  Abra a modal de desconto: pressione `Alt+V` para abrir direto, ou pressione `Alt+D` e, no menu suspenso, clique em **Aplicar desconto** › **Desconto no total**.
3.  Escolha o tipo de desconto: clique em **Percentual** (ou pressione `P`) ou em **Valor** (ou pressione `V`) — a modal sempre abre no modo **Percentual** quando ainda não há desconto aplicado.
4.  Informe o valor do desconto.
5.  Clique em **Aplicar desconto** ou pressione `Enter`.

![Modal Desconto total, com o tipo de aplicação Percentual (P) ou Valor (V) e o campo Valor do desconto](https://ajuda.sankhya.com.br/hc/article_attachments/43234901064727)  
 

O sistema calcula o rateio entre os itens elegíveis e atualiza imediatamente o **Subtotal**, o **Desconto Venda** e o total da grade — sem precisar recarregar a tela.

**⚠️ Atenção**

Se o valor solicitado ultrapassar o total que os itens elegíveis conseguem receber de desconto (somando o limite individual de cada produto), o sistema bloqueia a aplicação e exibe, na própria modal, o valor máximo possível para aquele carrinho.

### Editar desconto no total

1.  Com um desconto no total já aplicado, clique em **Editar** no resumo de desconto do rodapé, ou reabra o atalho (`Alt+V` ou `Alt+D`).
2.  A modal abre com o título **Editar desconto total**, no modo **Valor** e já preenchida com o valor atual do desconto.
3.  Altere o valor ou o tipo de desconto e clique em **Aplicar desconto**.

![Modal Editar desconto total, com o campo Valor do desconto pré-preenchido com o valor atual](https://ajuda.sankhya.com.br/hc/article_attachments/43234904586519)

O sistema refaz o rateio entre os itens com base no novo valor informado, seguindo a mesma regra da aplicação inicial.

### Remover desconto no total

1.  No resumo de desconto do rodapé, clique no ícone de lixeira ao lado do valor de **Desconto Venda**.
2.  No alerta exibido, com a mensagem _"O desconto total da venda será removido. Deseja retirar mesmo assim?"_, clique em **Remover desconto** (`Enter`) para confirmar, ou em **Cancelar** (`Esc`) para manter o desconto aplicado.

![Alerta de confirmação: O desconto total da venda será removido. Deseja retirar mesmo assim?](https://ajuda.sankhya.com.br/hc/article_attachments/43234904587799)

O desconto é removido por completo, a coluna **Desconto** da grade é reprocessada e os valores voltam ao estado anterior à aplicação — inclusive quando parte desse desconto estava ratejada em itens individuais.

#### Limite do perfil do operador e autorização do gerente

**O que faz**  
Define, por perfil de PDV, se o operador pode conceder desconto sem senha e até qual percentual — a mesma regra vale tanto para o desconto no total quanto para o desconto no item.

**Quando usar**  
Use para permitir que operadores concedam pequenos descontos sozinhos, reservando descontos maiores para autorização do gerente.

**Como funciona**  
Quando o desconto solicitado está dentro do **Percentual máximo de desconto** do perfil, ele é aplicado direto. Quando ultrapassa esse limite — mas ainda respeita o limite individual do produto, se houver — o sistema abre a modal **Autorização de desconto**, pedindo CPF e PIN do gerente. Se a autenticação for confirmada, o desconto é aplicado ignorando o limite do operador (mas nunca o limite do produto). Se a autenticação falhar, o sistema exibe um aviso de CPF ou PIN incorretos e não aplica o desconto. Se o gerente clicar em **Cancelar**, a modal de autorização fecha e o desconto não é aplicado.

![Modal Autorização de desconto, solicitando CPF e PIN do gerente para liberar um desconto acima do limite do operador](https://ajuda.sankhya.com.br/hc/article_attachments/43234901067671)

**Impacto no sistema**  
Vale igualmente para o desconto no total da venda e para o desconto no item — os dois fluxos são validados pela mesma parametrização de perfil de PDV.

**Configurações relacionadas**

<table style="border-collapse: collapse; margin-left: 0px; margin-right: auto;"><tbody><tr><td style="border-color: rgb(153, 153, 153); padding: 6px;"><strong>Necessidade</strong></td><td style="border-color: rgb(153, 153, 153); padding: 6px;"><strong>Onde configurar</strong></td><td style="border-color: rgb(153, 153, 153); padding: 6px;"><strong>Config</strong></td></tr><tr><td style="border-color: rgb(153, 153, 153); padding: 6px;">Permitir desconto no total da venda sem senha</td><td style="border-color: rgb(153, 153, 153); padding: 6px;">Portal Gerencial › Perfil de PDV › Seção Descontos</td><td style="border-color: rgb(153, 153, 153); padding: 6px;"><code>PERMITIR_DESCONTO_TOTAL</code></td></tr><tr><td style="border-color: rgb(153, 153, 153); padding: 6px;">Permitir desconto no item sem senha</td><td style="border-color: rgb(153, 153, 153); padding: 6px;">Portal Gerencial › Perfil de PDV › Seção Descontos</td><td style="border-color: rgb(153, 153, 153); padding: 6px;"><code>PERMITIR_DESCONTO_ITEM</code></td></tr><tr><td style="border-color: rgb(153, 153, 153); padding: 6px;">Percentual máximo de desconto sem senha de gerente</td><td style="border-color: rgb(153, 153, 153); padding: 6px;">Portal Gerencial › Perfil de PDV › Seção Descontos</td><td style="border-color: rgb(153, 153, 153); padding: 6px;"><code>LIMITE_PERCENTUAL_DESCONTO</code></td></tr><tr><td style="border-color: rgb(153, 153, 153); padding: 6px;">Exigir senha de gerente para desconto acima do limite</td><td style="border-color: rgb(153, 153, 153); padding: 6px;">Portal Gerencial › Perfil de PDV › Seção Necessário Aprovação do Gerente</td><td style="border-color: rgb(153, 153, 153); padding: 6px;"><code>REQUER_SENHA_DESCONTO_EXCEDIDO</code></td></tr></tbody></table>

[↑ Voltar ao início](#sumario)

---

## Desconto no item

O desconto no item aplica um valor percentual ou fixo sobre uma única linha da grade de vendas, sem afetar os demais produtos do carrinho. O valor informado é somado ao desconto de rodapé eventualmente ratejado para aquele item e exibido como um único valor na coluna **Desconto** da grade.

![Painel do produto selecionado na grade, com o campo Desconto (item) (Shift+5) em destaque](https://ajuda.sankhya.com.br/hc/article_attachments/43234901069335)

### Aplicar desconto no item

1.  Na grade de vendas, selecione a linha do produto desejado.
2.  Abra a modal de desconto: pressione `Shift+5`, ou clique na célula **Desconto** da linha selecionada, ou acesse o menu suspenso e clique em **Aplicar desconto no item**.
3.  Escolha o tipo de desconto: clique em **Percentual** (ou pressione `P`) ou em **Valor** (ou pressione `V`) — a modal sempre abre no modo **Percentual** quando o item ainda não tem desconto.
4.  Informe o valor do desconto.
5.  Clique em **Aplicar desconto** ou pressione `Enter`.

![Modal Aplicar desconto ao item, com o tipo de desconto Percentual (P) ou Valor (V) e o campo Valor do desconto](https://ajuda.sankhya.com.br/hc/article_attachments/43234901071511)

O valor é aplicado somente na linha selecionada. A coluna **Desconto** da grade e o resumo de **Subtotal**, **Desconto itens** e **Desconto Venda** são atualizados imediatamente.

![Resumo de Subtotal, Desconto itens e Desconto Venda atualizado após a aplicação do desconto](https://ajuda.sankhya.com.br/hc/article_attachments/43234901072791)  
 

**⚠️ Atenção**

Itens que participam de uma promoção ativa não podem receber desconto manual. Ao tentar abrir o desconto em um item nessas condições, o sistema exibe um aviso informando que o desconto não é permitido e a modal não é aberta.

### Editar desconto no item

1.  Selecione o item que já tem desconto aplicado.
2.  Pressione `Shift+5` ou clique na célula **Desconto** da linha — a modal abre com o título **Editar desconto no item**, no modo **Valor** e já preenchida com o valor atual do desconto.
3.  Altere o valor ou o tipo de desconto e clique em **Aplicar desconto**.

![Modal Editar desconto no item, com o campo Valor do desconto pré-preenchido com o valor atual](https://ajuda.sankhya.com.br/hc/article_attachments/43234904597783)  
 

### Remover desconto no item

1.  Selecione o item com desconto aplicado.
2.  Pressione `Shift+5` ou clique na célula **Desconto** da linha.
3.  Informe **0** (zero) no campo de valor.
4.  No alerta **Remover desconto do item?**, clique em **Remover desconto** (`Enter`) para confirmar, ou em **Cancelar** (`Esc`) para manter o desconto.

![Alerta de confirmação Remover desconto do item?](https://ajuda.sankhya.com.br/hc/article_attachments/43234904600727)  
 

O item volta ao valor original. Se havia desconto de rodapé ratejado para esse mesmo item, ele é preservado — apenas o desconto manual do item é removido.

#### Limite de desconto do produto

**O que faz**  
Bloqueia a aplicação de desconto manual — no item ou na parcela do rateio do desconto no total — acima do percentual máximo cadastrado para aquele produto específico.

**Quando usar**  
Use para produtos com política comercial própria de desconto máximo, definida no cadastro do produto.

**Como funciona**  
Quando o produto tem um limite de desconto cadastrado, o sistema checa esse limite antes mesmo de avaliar a alçada do operador. Se o valor solicitado ultrapassar o limite do produto, o sistema exibe o aviso **Desconto não permitido**, informando que o desconto está acima do configurado no cadastro do produto, e o desconto não é aplicado — mesmo que o gerente autorize. Quando o produto não tem limite cadastrado, essa validação não se aplica, e o desconto segue apenas para a checagem da [alçada do operador](#limite-alcada-gerente).

![Aviso Desconto não permitido: desconto acima do configurado no cadastro de produto](https://ajuda.sankhya.com.br/hc/article_attachments/43234901076631)

**Impacto no sistema**  
Vale tanto para o desconto aplicado diretamente no item quanto para a parcela do rateio do desconto no total da venda sobre aquele item.

**Configurações relacionadas**

<table style="border-collapse: collapse; margin-left: 0px; margin-right: auto;"><tbody><tr><td style="border-color: rgb(153, 153, 153); padding: 6px;"><strong>Necessidade</strong></td><td style="border-color: rgb(153, 153, 153); padding: 6px;"><strong>Onde configurar</strong></td><td style="border-color: rgb(153, 153, 153); padding: 6px;"><strong>Config</strong></td></tr><tr><td style="border-color: rgb(153, 153, 153); padding: 6px;">Percentual máximo de desconto do produto</td><td style="border-color: rgb(153, 153, 153); padding: 6px;">Cadastro de Produtos&nbsp;<em>(confirmar caminho exato do campo antes de publicar)</em></td><td style="border-color: rgb(153, 153, 153); padding: 6px;"><code>DESCMAX</code></td></tr></tbody></table>

[↑ Voltar ao início](#sumario)

---

## Pontos de atenção

*   Quando um item tem desconto manual e desconto de rodapé ao mesmo tempo, a grade soma os dois valores e mostra um único total na coluna **Desconto** — não é possível ver os dois valores separados ali.
*   No desconto no total, eventuais diferenças de centavos do rateio (a chamada dízima de R$ 0,01) são sempre atribuídas ao item de maior valor participante — pequenas diferenças entre itens são esperadas e não indicam erro.
*   Itens em promoção ativa ficam fora dos dois fluxos: não recebem desconto manual no item e não participam do rateio do desconto no total.
*   O resumo de **Subtotal**, **Desconto itens** e **Desconto Venda** é somente leitura — não é possível editar o desconto de um item por ali. A edição sempre acontece no item da grade (desconto no item) ou na modal do rodapé (desconto no total).

[↑ Voltar ao início](#sumario)

---

## Perguntas frequentes

### Posso aplicar desconto no total da venda e desconto em um item específico na mesma venda?

Sim. Os dois valores são somados e aparecem juntos na coluna **Desconto** da grade e no campo **Desconto Venda** do resumo.

### Por que não consigo aplicar desconto em um dos itens do carrinho?

O item provavelmente participa de uma promoção ativa. Itens em promoção não recebem desconto manual, nem no item nem no rateio do desconto no total.

### O que acontece se eu digitar 0 no valor do desconto de um item que já tem desconto aplicado?

O sistema entende que você quer remover o desconto e abre o alerta de confirmação **Remover desconto do item?**.

### Por que o sistema pediu CPF e PIN do gerente ao aplicar um desconto?

O valor solicitado ultrapassou o **Percentual máximo de desconto** parametrizado no perfil de PDV do operador. É necessária a autorização do gerente, na modal **Autorização de desconto**, para prosseguir.