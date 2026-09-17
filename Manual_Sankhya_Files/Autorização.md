# Autorização

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114993-Autoriza%C3%A7%C3%A3o](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114993-Autoriza%C3%A7%C3%A3o)

---

# Autorização

<table style="font-size: 15px; width: 100%;" cellspacing="0,5"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre class="wysiwyg-text-align-justify"><span class="wysiwyg-font-size-medium"><strong><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42312435302423" alt="Módulo 36x36 FINAL.png"> Módulo: </strong>Financeiro &gt; Rotinas &gt; Operações de Crédito</span></pre></td></tr></tbody></table>

---

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 5.99999%;">&nbsp;</td><td class="wysiwyg-text-align-right" style="width: 10.4286%;"><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42312422679063" alt="essencial FINAL (1).png"></td><td class="wysiwyg-text-align-left" style="width: 83.5715%;">&nbsp; &nbsp;Rotina exclusiva de Parceiro habilitada por parâmetro específico.</td></tr></tbody></table>

---

O lojista usará esta tela para registrar/autorizar uma compra realizada e paga com cartão de crédito, no RG ou no CPF do cliente.

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4420968432791)

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 7.71428%;"><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42312435304215" alt="Atenção FINAL.png"></td><td class="wysiwyg-text-align-justify" style="width: 92.2858%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">O usuário </span><span style="font-family: Verdana,Geneva,Arial,sans-serif; font-weight: bold;">B2B</span>,<span style="font-family: Verdana,Geneva,Arial,sans-serif;"> e o usuário normal tem acesso à tela abaixo. No caso de usuário</span><span style="font-family: Verdana,Geneva,Arial,sans-serif; font-weight: bold;"> B2B</span>,<span style="font-family: Verdana,Geneva,Arial,sans-serif;"> não será visível na grade o campo <strong>"Data Vencimento"</strong>.</span></td></tr></tbody></table>

O **"Logista"**, é o parceiro do usuário B2B logado.

Informe também o **"Cliente"**, o parceiro para o qual a venda está sendo realizada.

No campo **"Data do primeiro vencimento"**, é preciso informar a data do primeiro vencimento correspondente à negociação realizada junto ao Cliente.

É preciso ainda, considerar a influência do parâmetro **"Qtd. dias para primeiro vencimento da autorização de crédito - DIASTOLPRIVCTO"**. Observe:

*   Primeiro, é encontrada a data para primeiro vencimento de cada tipo de negociação.
*   Assim, a Data Atual + 'Prazo máx. 1ª parcela' do Cadastro do [Tipo de Negociação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045109173-Tipos-de-Negocia%C3%A7%C3%A3o) = Data do primeiro vencimento do tipo de negociação.
*   Com isso, é feito o cálculo de diferença em quantidade de dias entre a Data do primeiro vencimento dessa tela, e a Data do primeiro vencimento do Tipo de Negociação, em que, será igual à Quantidade de dias entre as datas.
*   Porém, se a quantidade de dias entre as datas menor ou igual a Quantidade de dias informada no parâmetro Qtd. dias para primeiro vencimento da autorização de crédito - DIASTOLPRIVCTO, então a negociação será apresentada no combo, caso contrário, ela não será apresentada.

Considere o seguinte exemplo:

**Parâmetro DIASTOLPRIVCTO** = 3

**Data Atual:** 15/12/2016

**Prazo Máx. 1ª parcela** = 60

**Data do Primeiro vencimento do tipo de negociação** = '15/12/2016' + 60  = 13/02/2017

**Data do primeiro vencimento** (tela Autorização)**:** 15/02/2017

**Diferença:** 15/02/2017 - 13/02/2017 = 2 dias

2 menor ou igual 3 à foi apresentado as negociações

Alterado o parâmetro para:

**Parâmetro DIASTOLPRIVCTO** = 1

2 maior ou igual 1 à não foi apresentado as negociações

Em **"Tipo negociação"**, informe o tipo da negociação a ser utilizado para registrar a venda realizada no cartão ou no CPF do cliente.

Ao clicar no botão ![Gerar Parcelas FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16090565110295)**"Gerar Parcelas"**, o sistema irá gerar as parcelas conforme a quantidade negociada no Tipo de Negociação.

No botão ![Botão confirmar autorização FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16090575741719) **"Confirmar autorização"** confirmará a compra realizada. Sendo que, quando esta for confirmada, o sistema exibirá a seguinte mensagem:

_**"Autorização realizada com sucesso! O número único da autorização é xxxxxx."**_

Referente ao botão descrito acima, pode acontecer de quando a solicitação das parcelas for confirmada, o sistema emita a seguinte mensagem:

_**"Entre em contato com a Administradora."**_

Essa mensagem é geralmente apresentada quando as seguintes situações existirem:

*   O Parceiro está bloqueado para venda a prazo;
*   Parceiro sem limite de crédito para realizar a compra;
*   Existência de títulos de receitas em atraso para este parceiro.

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-right" style="width: 7.42857%;"><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42312435304215" alt="Atenção FINAL.png"></td><td class="wysiwyg-text-align-justify" style="width: 92.5715%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Verifique também a tolerância para inadimplência do mesmo.</span></td></tr></tbody></table>

---

 **![informações adicionais FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16088908675607) Informações Adicionais** 

*   Somente se você estiver logado com um usuário não B2B, o campo **"Data da venda"** ficará visível;
*   A data de negociação (data da venda) não pode ser maior que a data atual;
*   A propriedade de permissão de usuário **"Permite autorizações retroativas"** permitirá ou não lançamentos/autorização retroativos no campo **"Data da venda",** ou seja, se este tiver permissão poderá alterar a Data da venda, se não houver permissão, essa data ficará desabilitada e apresentando a Data atual do sistema, não permitindo alteração;
*   Caso você tente realizar uma compra com um cartão que esteja com o status **"Embossamento"** ou **"Bloqueado"**, o sistema não permitirá e emitirá uma mensagem alertando-o que a compra deverá ser realizada com CPF/CNPJ ou RG. Se o cartão estiver ativado a compra, obrigatoriamente deverá ser realizada pelo mesmo e se estiver nos demais status (Cancelado, Roubado ou Perdido) a compra não poderá ser realizada por nenhuma das opções.