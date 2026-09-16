# Rastreabilidade de série - WMS

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/4418318007575-Rastreabilidade-de-s%C3%A9rie-WMS](https://ajuda.sankhya.com.br/hc/pt-br/articles/4418318007575-Rastreabilidade-de-s%C3%A9rie-WMS)

---

# Rastreabilidade de série - WMS

<table cellspacing="0,5" style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre class="wysiwyg-text-align-justify"><span class="wysiwyg-font-size-medium"><strong><img alt="Versão - 32x32 FINAL.png" src="https://ajuda.sankhya.com.br/hc/article_attachments/42311637846295"> Versão disponível:</strong> A partir da 4.11</span></pre></td></tr></tbody></table>

---

O Sistema Nacional de Controle de Medicamentos (SNCM) tem o objetivo de acompanhar os medicamentos em toda a cadeia produtiva, desde a fabricação até o consumo. 

A rastreabilidade por meio SNCM possibilitará uma maior segurança dos pacientes e profissionais em relação ao uso dos medicamentos a serem utilizados, para que assim, exista um controle maior de produção e logística, além de facilitar os fluxos e manutenções regulatórios de conformidade.

Sabendo disso, ao clicar nos tópicos apresentados na imagem a seguir, você pode ler mais sobre a rastreabilidade de série e seus processos:

![mceclip11.png](https://ajuda.sankhya.com.br/hc/article_attachments/4420364099735)

<table style="border-collapse: collapse; width: 100%; height: 45px;"><tbody><tr style="height: 45px;"><td class="wysiwyg-text-align-center" style="width: 10.3333%; height: 45px;"><a href="#P" target="_self">Códigos</a></td><td style="width: 5.9048%; height: 45px;">&nbsp;</td><td class="wysiwyg-text-align-center" style="width: 9.04767%; height: 45px;">&nbsp;<a href="#xml" target="_self">XML</a></td><td style="width: 6.47617%; height: 45px;">&nbsp;</td><td class="wysiwyg-text-align-center" style="width: 8.83318%; height: 45px;"><a href="#conf.iniciais" target="_self">Conf. Iniciais</a></td><td style="width: 5.57143%; height: 45px;">&nbsp;</td><td class="wysiwyg-text-align-center" style="width: 4.24995%; height: 45px;"><a href="#confer%C3%AAnciarecebimento" target="_self">Confer. Receb.</a></td><td style="width: 7.10709%;">&nbsp;</td><td class="wysiwyg-text-align-center" style="width: 9.83344%; height: 45px;"><a href="#recontagemrecebimento" target="_self">Rec. Receb.</a></td><td style="width: 3.97623%;">&nbsp;</td><td class="wysiwyg-text-align-center" style="width: 8.7619%; height: 45px;"><a href="#ean13" target="_self">Ean13</a></td><td style="width: 4.09521%; height: 45px;">&nbsp;</td><td class="wysiwyg-text-align-center" style="width: 15.9524%; height: 45px;"><a href="#invent%C3%A1rio" target="_self">Inventário</a></td></tr></tbody></table>

---

Você poderá realizar a leitura desses produtos de três maneiras diferentes. Observe:

**SSCC**

O SSCC, ou Serial Shipping Container Code (Código de Série da unidade Logística), é um código de dezoito dígitos que irá auxiliá-lo no momento da conferência do produto.

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4418576802583)

Utilizando esse método, você poderá efetuar a leitura em massa de várias séries, datas de validades e lotes dos produtos. 

Considere ainda que, quando um SSCC for lido, o sistema irá considerar os dados do arquivo EDI enviado pela indústria. Nesse caso, uma boa prática, é fazer o seu uso apenas quando a caixa deste SSCC estiver lacrada, pois, assim evitará que erros de contagem e/ou conferência possam ocorrer.

**DataMatrix**

O código DataMatrix é um código 2D que permite armazenar uma quantidade maior de dados em espaços menores. 

<table style="border-collapse: collapse; width: 100%; height: 95px;"><tbody><tr style="height: 89px;"><td class="wysiwyg-text-align-justify" style="width: 76.8571%; height: 89px;"><span style="font-weight: 400;">Além de que, pode ser facilmente confundido com o QRCode, pois as suas estruturas são semelhantes, porém cada um deles possui diferentes funcionalidades, como, por exemplo, o QRCode codifica e-mail's, URL's, contatos telefônicos, entre outras informações de contato.</span></td><td style="width: 2.85712%;"><span style="font-weight: 400;">&nbsp;</span></td><td style="width: 20.2857%; height: 89px;"><img alt="mceclip2.png" height="116" src="https://ajuda.sankhya.com.br/hc/article_attachments/42311637848855" width="122"></td></tr></tbody></table>

Já o DataMatrix, permite que várias informações sejam armazenadas, o que o torna ideal para peças, equipamentos, componentes e caixas. Destaca-se ainda que, para utilizá-lo, é necessário o uso de um Coletor de Dados bidimensional. Observe abaixo a estrutura de um código DataMatrix:

<table style="border-collapse: collapse; width: 100%; height: 109px;"><tbody><tr style="height: 22px;"><td rowspan="5" style="width: 22.2858%; height: 109px;"><img alt="mceclip0.png" src="https://ajuda.sankhya.com.br/hc/article_attachments/42311637849879"></td><td rowspan="5" style="width: 2.2858%;">&nbsp;</td><td style="width: 75.4285%; height: 22px;">GTIN (EAN) <strong>⇢</strong>&nbsp; (01)0789835710015<strong>&nbsp;</strong></td></tr><tr style="height: 21px;"><td style="width: 75.4285%; height: 21px;">Registro Anvisa <strong>⇢</strong> (713)3210987654321 <strong>&nbsp;</strong></td></tr><tr style="height: 22px;"><td style="width: 75.4285%; height: 22px;">Serial <strong>⇢</strong> (21)1234567890123 <strong>&nbsp;</strong></td></tr><tr style="height: 22px;"><td style="width: 75.4285%; height: 22px;">Validade <strong>⇢</strong> (17)161231 &nbsp;</td></tr><tr style="height: 22px;"><td style="width: 75.4285%; height: 22px;">Lote <strong>⇢</strong> (10) 123ABC <strong>&nbsp;</strong></td></tr></tbody></table>

Assim, ao utilizar esse método, você poderá, por meio de uma única leitura obter informações completas das séries, datas de validade, lote, entre outros dados dos produtos lidos.

Porém, assim como a leitura executada pelo SSCC, é recomendável que a leitura destes sejam realizadas apenas quando a caixa estiver totalmente lacrada para garantir a autenticidade das informações de séries obtidas.

**EAN13**

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-justify" style="width: 70.5714%;"><span style="font-weight: 400;">Sendo o mais comum dos códigos, este irá identificar os produtos de maneira individual, visto que, possui todas as informações relevantes sobre este como, seu país de origem, a empresa fabricante, o produto produzido e seu dígito verificador. Destaca-se também que, a soma deles sempre resultará em um código de 13 dígitos.</span></td><td class="wysiwyg-text-align-justify" style="width: 29.4286%;"><img alt="mceclip0.png" height="134" src="https://ajuda.sankhya.com.br/hc/article_attachments/42311643914775" width="186"></td></tr></tbody></table>

E pode ainda, ser utilizado quando por algum motivo, os códigos SSCC e/ou DataMatrix estiverem indisponíveis, sendo nesse caso, necessário informar as séries dos produtos manualmente após a leitura dos códigos de barras.

[\[voltar ao topo\]](#top)

**XML**

![mceclip10.png](https://ajuda.sankhya.com.br/hc/article_attachments/4420346277015)

Além dos códigos expostos acima, teremos o XML, que será o arquivo disponibilizado pela indústria com as informações de séries dos produtos fabricados. Nele, conterá as seguintes informações:

*   Remetente (Fabricantes);
*   SSCC;
*   Série;
*   Lote;
*   Data de Validade;
*   Chave da NFe.

[\[voltar ao topo\]](#top)

#### **Configurações iniciais**

![mceclip9.png](https://ajuda.sankhya.com.br/hc/article_attachments/4420354148887)

Para ativar a rotina do SNCM no Coletor, você deve realizar no Sankhya Om as configurações a seguir: 

Primeiramente, ligue o parâmetro **"Rastreabilidade de medicamentos por série no WMS - WMSRASTMEDSER"**, para que as marcações abaixo sejam exibidas:

*   Na tela [Preferências da empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893), aba [WMS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893#abawms), será apresentada a marcação **"Habilita controle de rastreabilidade série de medicamentos no WMS"**.
*   Na tela de [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113), aba [WMS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113#abawms), será exibida a marcação **"Produto rastreado por série e controle de medicamento"**. 

<table class="wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; height: 56px;"><tbody><tr style="height: 56px;"><td class="wysiwyg-text-align-justify" style="width: 100%; height: 56px;"><pre><strong>                                                                                      <img alt="Atenção FINAL.png" src="https://ajuda.sankhya.com.br/hc/article_attachments/16979013355415"><br>         Para que a tela SNCM seja apresentada no <span class="wysiwyg-underline">Coletor</span>, todas as <span class="wysiwyg-underline">Empresas</span> cadastradas no<br>         <span class="wysiwyg-underline">Sankhya Om</span> precisam estar com a marcação <span class="wysiwyg-underline">Habilita controle de rastreabilidade </span><span class="wysiwyg-underline">série<br></span>         <span class="wysiwyg-underline">de medicamentos no WMS</span> ligada.</strong></pre></td></tr></tbody></table>

**![Configura\_oes\_iniciais\_wms.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4418312055319)**

Com estas marcações ligadas, o coletor passará a efetuar a leitura do código do tipo SSCC e Datamatrix nos processos de Conferência de Recebimento, Pedido e Saída, e ainda, Contagem do Inventário.

Agora, realize na tela de Cadastro de Produtos as configurações a seguir:

Na aba WMS, acione a marcação **"****Usar controle adicional no WMS"** e informe no campo **"Shelflife"** o prazo de validade em dias do produto.

![aba\_wms.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4418319670295)

Depois, na aba [Medidas e Estoque](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113#abamedidaseestoque), sub-aba [Controle Adicional](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113#sub-abacontroleadicional), selecione no campo **"Controlar Por"** a opção **"Número do Lote"**. 

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4418319677847)

<table class="wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; height: 56px;"><tbody><tr style="height: 56px;"><td class="wysiwyg-text-align-justify" style="width: 100%; height: 56px;"><pre><strong>                                                                                      <img alt="Atenção FINAL.png" src="https://ajuda.sankhya.com.br/hc/article_attachments/16979013355415"><br>         O sistema não permitirá o envio da nota para o recebimento no WMS, se as duas últimas<br>         configurações, estiverem incorretas.</strong></pre></td></tr></tbody></table>

---

Com as configurações acima efetuadas, iremos agora dar início ao processo de recebimento, assim, realize o lançamento de uma nota no [Portal de Compras](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045111953). Lembrando que, o arquivo XML enviado pela indústria contém a **"****Chave NF-e"**, informação essa que efetua a conexão com a Nota de Compra, e que, em caso de divergência do XML, a importação não poderá ser efetuada.

Depois, acesse a tela **"Importação XML Série Medicamento"** para importar o arquivo XML enviado pela indústria contendo os dados de série de medicamentos. Para isso, basta acionar o botão **"Importar XML"** e selecionar o arquivo desejado. 

![importa\_ao\_com\_sucesso.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4418321750679)

Feito isso, acesse novamente o Portal de compras e envie a nota para a conferência no WMS, por meio do botão **"Outras Opções"**, opção **"Enviar para o WMS (Recebimento)"**. Desse modo, ao acionar esta opção, será apresentado o pop-up **"Dados para recebimento"**, onde você deve informar a **"Data de Recebimento"** e a **"Doca para descarga"**.

![dados\_recebimento.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4418347110807)

Ao clicar em **"Confirmar"**, a nota será enviada para conferência.

---

![Atenção FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16979013355415)

Caso você não tenha importado o arquivo XML na tela Importação XML Série Medicamento, ao enviar a nota para o recebimento o sistema irá informá-lo que a nota de compra não foi identificada nos registros de XML, e irá questioná-lo se deseja prosseguir sem a importação:

 ![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28451016141847)Clicando em **"Sim"**, a nota será enviada para o recebimento para conferência e o sistema compreenderá que os produtos contidos nesta nota, apesar de serem configurados para SNCM, ainda não foram fabricados nesta modalidade de controle, ou seja, a indústria está em fase de adequação e, portanto, na conferência será disponibilizado o mecanismo de leitura convencional EAN13 sem solicitação de séries no processo de conferência.

 ![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28451016141847) Optando por **"Não"**, a operação será cancelada e caso deseje realizar a importação, você poderá acessar a tela Importação XML Série Medicamento.

[\[voltar ao topo\]](#top)

---

Com as configurações acima realizadas, você poderá efetuar os seguintes processos:

#### **Conferência Recebimento** 

![mceclip8.png](https://ajuda.sankhya.com.br/hc/article_attachments/4420363950359)

Para realizar este processo, acesse o Coletor, selecione a função **"Conferência Entrada"** e clique em **"Conferência"**, assim, será apresentada a tela **"Conferência de S.N.C.M"**. 

Nela, informe o número da **"Doca"** e o código SSCC, desse modo, o sistema irá registrar a Quantidade, o Lote e a Data de validade dos produtos. Para finalizar a conferência clique em **"Enviar"**.

![conferencia\_recebimento.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4420276749463)

Além disso, quando houver uma avaria na conferência SNCM, você pode registrá-la por meio do botão **"Avaria"**.

 ![dica FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16978994288279) Para realizar os processos de Conferência Recebimento, Pedido e Saída, você pode efetuar as mesmas etapas descritas acima.

[\[voltar ao topo\]](#top)

---

#### **Recontagem Recebimento**

![mceclip7.png](https://ajuda.sankhya.com.br/hc/article_attachments/4420346181783)

Para realizar a Recontagem do Recebimento quando ocorre algum tipo de divergência, considere que após o envio dos produtos ao Coletor, você deve selecionar o processo **"Conferência de Entrada"** e informar a **"Doca"** de conferência, dessa forma, o sistema exibirá o produto com a divergência para que seja conferido. Porém, para isso, é importante também que o parâmetro **"Utiliza recontagem agrupada na separação? - USARECAGRUPADA"** esteja ligado; pois, dessa forma, o coletor terá acesso à tela de Recontagem.

Posteriormente, ao informar os filtros referentes à conferência na tela [Recebimento de Mercadorias](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044613034), por meio do botão ![Botão Divergência FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16979013365015) **"Divergência"**, no pop-up **"Divergências na conferência"** você pode decidir a ação seguinte. 

![recebimento\_de\_mercadorias.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4420396978839)

<table style="border-collapse: collapse; width: 100%;"><tbody><tr style="height: 56px;"><td class="wysiwyg-text-align-justify" style="width: 100%; height: 56px;"><pre><strong>                                                                                    <img alt="Atenção FINAL.png" src="https://ajuda.sankhya.com.br/hc/article_attachments/16979013355415"><br>         Quando um produto do tipo SSCC for lido com divergência, o sistema irá verificar se<br>         os i</strong><strong>tens pertencem à nota no momento da importação do XML, visto que este estará <br>         vinculado </strong><strong>à nota de compra.</strong></pre></td></tr></tbody></table>

Assim, dado que o parâmetro Rastreabilidade de medicamentos por série no WMS - WMSRASTMEDSER esteja ligado, e o XML for importado por meio da tela Importação XML Série Medicamento e vinculado à nota, quando houver divergência na conferência do produto, o sistema irá informá-lo por meio de mensagens no Coletor de Dados. Você pode conferir os exemplos abaixo:

Se na recontagem de conferência, um produto do tipo SSCC, ou DataMatrix possuir determinada informação inconsistente, o sistema irá alertá-lo da seguinte forma:

_**"O produto lido é diferente do esperado na recontagem!"**_

Ou ainda, caso o item lido esteja correto, porém o DataMatrix possua uma série internalizada em outro recebimento, ou já foi lido no mesmo recebimento, a seguinte mensagem será exibida:

_**"Existem itens coletados pelo coletor por este DATAMATRIX, que já foram conferidos!"**_

[\[voltar ao topo\]](#top)

---

#### **Leitura pelo código EAN13**

![mceclip6.png](https://ajuda.sankhya.com.br/hc/article_attachments/4420363805335)

Nos processos mencionados acima, quando os códigos SSCC ou Datamatrix não forem identificados, você pode efetuar a leitura por meio do código EAN13.

Para isso, acesse o Coletor, selecione a **"Função"** desejada e realize a leitura do código EAN13, se o código informado for valido, o campo **"Quantidade"** será apresentado para preenchimento e caso o produto contenha lote informado na nota o sistema exibirá também o campo **"Lote"** para preenchimento.

Ao clicar em **"Enviar"** a tela **"Séries"** será apresentada de acordo com o processo que esta sendo executado, observe:

 ![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28451016141847) No processo de Recebimento ela será exibida quando existirem informações internalizadas pelo xml referente ao lote lido. Caso o lote não esteja internalizado, a tela de séries não será apresentada.

 ![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28451016141847) Já no processo de Expedição a tela Séries será apresentada somente se o lote informado já estiver com uma entrada positiva e houver saldo suficiente para a série.

Além disso, se for informada uma série que não possua saldo disponível para expedição, não será possível registrar os dados da referida série. Sendo assim, você deverá entrar em contato com a administração para analisar a situação da série indisponível, tratando assim, de um erro de inventário/estoque.

Do contrário, quando uma conferência for finalizada sem divergências, o sistema registrará as séries e fará uma reserva da série, e quando houver o faturamento do pedido, a série será efetivada com uma saída negativa, ficando indisponível neste processo para outras conferências.

Com as séries informadas, ao clicar em **"Ok"**, o sistema verificará se foi informado todas as séries previstas conforme valor estabelecido no campo Quantidade, se sim, será apresentada a mensagem: **_"Item lido com sucesso."_**  

**_![Rastreabilidade\_gif.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4423010804759)_**

[\[voltar ao topo\]](#top)

---

#### **Processo de inventário** 

![mceclip4.png](https://ajuda.sankhya.com.br/hc/article_attachments/4420363078167)

Antes de você efetuar a contagem de estoque no coletor, é necessário realizar algumas configurações no Sankhya OM, que foram detalhadas no artigo [Processo de Inventário](https://ajuda.sankhya.com.br/hc/pt-br/articles/1500007989601).

Com as configurações realizadas, acesse o coletor e seleciona a função **"Contagem de Estoque"**, clique no botão **"Tarefa"** e informe o **"Endereço"** onde será inserido o estoque do produto. Depois, no campo **"Produto"** você pode informar o código SSCC, o Datamatrix ou o EAN 13.

Caso você opte pelo o código EAN 13, será apresentado o campo **"Quantidade"**, nele informe a quantidade do produto contada no estoque. Além disso, se o produto possuir número de série, assinale a marcação **"Habilitar SNCM"** .

<table style="border-collapse: collapse; width: 100%;"><tbody><tr style="height: 56px;"><td class="wysiwyg-text-align-justify" style="width: 100%; height: 56px;"><pre><strong>                                                                                    <img alt="Atenção FINAL.png" src="https://ajuda.sankhya.com.br/hc/article_attachments/16979013355415"><br>              <span style="font-weight: 400;">A marcação </span><span class="wysiwyg-underline"><span style="font-weight: 400;">Habilitar SNCM</span></span><span style="font-weight: 400;">, </span><span style="font-weight: 400;">por padrão estará ligado para informar as séries.<br>              Caso o produto não possa ser rastreado por série, ele deve ser desabilitado  <br>              antes da confirmação da leitura.</span></strong></pre></td></tr></tbody></table>

![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/4420415560599)

**Observações:**

*   Neste processo, o SSCC e o Data Matrix têm o objetivo apenas de identificar a quantidade de produto e registrar as séries.
*   A série informada neste processo é apenas a título de registro.
*   Para verificar as séries capturadas é necessário solicitar um processo personalizado.

Com os campos acima preenchidos, será exibida a tela de **"Informações adicionais"**, nela informe o número **"Lote"**, a **"Dt. Validade"** ou a **"Dt. Fabricação"** e clique em **"Salvar"**.

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4420466471319)

Agora, na tela **"Séries"** informe o número das séries dos produtos.

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4420466476183)

Feito isso, para concluir o processo clique no botão **"OK"**.

---

Por fim, ao realizar as configurações aqui expostas, e iniciar a rastreabilidade de medicamentos, você oferecerá mais qualidade e segurança ao consumidor final, além de poder traçar o histórico e o local de cada unidade do medicamento, e a certeza de autenticidade das informações de origem do produto, a fim de evitar fraudes.

[\[voltar ao topo\]](#top)