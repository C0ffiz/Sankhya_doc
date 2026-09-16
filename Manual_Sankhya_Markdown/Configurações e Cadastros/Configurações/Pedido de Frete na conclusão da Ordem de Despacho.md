# Pedido de Frete na conclusão da Ordem de Despacho

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360044599154-Pedido-de-Frete-na-conclus%C3%A3o-da-Ordem-de-Despacho](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044599154-Pedido-de-Frete-na-conclus%C3%A3o-da-Ordem-de-Despacho)

---

# Pedido de Frete na conclusão da Ordem de Despacho

Analisando as etapas finais de um processo de venda, no que diz respeito a logística de transporte, as empresas possuem diferentes critérios para definição da transportadora de suas mercadorias; geralmente, é a que executa o serviço por um preço menor.

Neste processo, o serviço dos [Correios](http://www.correios.com.br/para-voce) pode ser contratado; portanto é necessário que as empresas possam consultar o preço do frete cobrado, bem como a situação de suas mercadorias.

Veremos neste artigo os detalhes e configurações acerca destes procedimentos. Assim, clique nos links abaixo para facilitar sua navegação no conteúdo.

*   [Como considerar os Correios no cálculo da melhor transportadora?](#comoconsideraroscorreiosnoclculodamelhortransportadora)
*   [Cálculo da melhor transp. na confirmação e faturamento do pedido](#clculodamelhortransportadoranaconfirmaoefaturamentodopedido)
*   [Concluindo a Ordem de Despacho](#concluindoaordemdedespacho)

---

## Como considerar os Correios no cálculo da melhor transportadora?

Para que os Correios sejam considerados pelo sistema no cálculo da melhor transportadora, são necessárias as seguintes configurações:

*   No [Cadastro de Parceiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Parceiros), deve-se criar um parceiro Transportadora correspondente aos Correios. É essencial que o campo **"Tipo"** presente na [Aba Identificação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Parceiros#abaidentificao), esteja definido como Transportadora.

![aba\_Identifica\_\_o-\_campo\_Tipo\_-\_op\_\_o\_Transportadora.png](https://ajuda.sankhya.com.br/hc/article_attachments/9778150732695)

*   Na tela [Preferências](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601834-Prefer%C3%AAncias), informa-se o Código do Parceiro cadastrado no parâmetro **"Lista de parceiros ECT - PARCEIROSECT"**.

![Tela\_Prefer\_ncias-\_campo\_Texto.png](https://ajuda.sankhya.com.br/hc/article_attachments/9778328165655)

*   Nas [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Empresa), aba **"Correios"**, deve-se informar adequadamente a identificação e senha de usuário para o serviço dos Correios; para tal medida, tem-se os campos **"Identificação Correios"** e **"Senha Correios"**, respectivamente.

![aba\_Correios.png](https://ajuda.sankhya.com.br/hc/article_attachments/9783040319127)

*   Através da tela [Tabelas para cálculo de frete](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044599534-Tabelas-para-c%C3%A1lculo-de-frete), cria-se uma tabela onde deve-se inserir qual serviço dos Correios a tabela em questão atende; este vínculo é realizado por meio do campo **"Serviço Correios"**. Para cada serviço dos Correios, é necessário que seja criada uma tabela; é importante também que nesta tabela, apenas o Parceiro Correios esteja a ela vinculado. Nesta situação, não existe a necessidade de cadastrar Região p/ Tabela de Frete e Rotas.
*   O cadastro de cada um destes serviços será realizado previamente através da tela [Serviço Correios](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594734-Servi%C3%A7o-Correios).

![aba\_Transportadoras.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/9783221015191)

*   O [Tipo de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP) utilizado no lançamento do Pedido de Venda deve estar configurado para escolha da melhor transportadora de forma automática, ou seja, a marcação **"Simulação de frete automática"** presente na aba [Financeiro](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abafinanceiro), deve estar realizada. Com esta opção marcada, o sistema selecionará a melhor transportadora na confirmação do pedido de venda e não exigirá informações adicionais para geração de frete extra nota. O inverso irá acontecer caso esta opção não esteja assinalada, ou seja, não será feita a seleção automática da melhor transportadora e também serão exigidas informações adicionais para geração de frete extra nota.

![Tela\_Tipos\_de\_Opera\_\_o\_top\_-\_aba\_Financeiro\_-\_marca\_\_o\_Simula\_\_o\_de\_frete\_autom\_tica\_ligada.png](https://ajuda.sankhya.com.br/hc/article_attachments/9783604582679)

*   Uma vez realizadas as configurações até aqui mencionadas, o Parceiro Correios também poderá ser utilizado através da opção [Simulação de frete com escolha de transportadora](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612234-Central-de-Vendas-Bot%C3%A3o-Outras-Op%C3%A7%C3%B5es#simulaodefretecomescolhadetransportadora) presente no [Botão Outras Opções](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612234-Central-de-Vendas-Bot%C3%A3o-Outras-Op%C3%A7%C3%B5es) da [Central de Vendas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612414-Central-de-Vendas).

[\[voltar ao topo\]](#top)

## Cálculo da melhor transportadora na confirmação e faturamento do pedido

Na confirmação do [Pedido de Venda](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612654-Portal-de-Vendas#oqueumpedidodevenda), quando a modalidade do frete for igual a **"CIF"** (quando o frete é pago por quem envia a mercadoria, ou seja, o Remetente) e seu Tipo igual a **"Extra Nota"**, será feito o cálculo da melhor transportadora com base no critério de preço utilizado na rotina de [Simulação de frete com escolha de transportadora](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612234-Central-de-Vendas-Bot%C3%A3o-Outras-Op%C3%A7%C3%B5es#simulaodefretecomescolhadetransportadora). Com base nas informações passadas até aqui, os Correios serão considerados nessa seleção e definição da melhor transportadora.

Além do momento da confirmação do Pedido de Venda, este mesmo cálculo irá acontecer no faturamento automático do pedido de reserva para o pedido de expedição.

Caso já exista algum pedido de expedição pendente para a mesma empresa e cliente, o cálculo da transportadora não irá selecionar a melhor com base no preço cobrado. A transportadora do pedido de reserva ou do pedido de expedição, neste caso, será igual à transportadora do pedido de expedição pendente que foi localizado.

Exceto a situação acima, caso não exista qualquer transportadora calculada para o pedido de venda, o sistema irá notificar o usuário, para que este providencie a transportadora a ser contratada na condução da mercadoria vendida.

<table style="border-collapse: collapse; height: 30px;" border="0,5"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 53px;"><img src="/hc/article_attachments/42310717643287" alt="informações adicionais FINAL.png"></td><td class="wysiwyg-text-align-justify" style="width: 624px;">Caso sejam feitas alterações da modalidade de frete do pedido de venda para <span class="wysiwyg-underline">CIF</span> e o Tipo de frete for modificado para <span class="wysiwyg-underline">Extra Nota</span>, este cálculo será acionado.</td></tr><tr><td style="width: 53px;">&nbsp;</td><td style="width: 624px;">&nbsp;</td></tr></tbody></table>

O cálculo do frete da melhor transportadora também irá ocorrer para modalidade de frete **"CIF"** e **"Incluso"**, seja de forma automática ou manual.

Caso o parâmetro **"Aquisição de serviço de frete com frete incluso - AQSERVFRETINC"** esteja ativado, o cálculo de frete para melhor transportadora (de forma automática ou manual), desde que seja Incluso, será registrado no campo **"Vlr. frete calc."**.

Além disso, no faturamento de pedidos, independente do status do parâmetro de chave AQSERVFRETINC, a informação presente no campo Vlr. frete calc. será inserida também no novo documento gerado; caso este faturamento seja parcial, tem-se a informação de Vlr. frete calc. de forma parcial.

<table style="border-collapse: collapse; height: 30px;" border="0,5"><tbody><tr style="height: 44px;"><td class="wysiwyg-text-align-center" style="width: 52px; height: 44px;"><img src="/hc/article_attachments/42310717643287" alt="informações adicionais FINAL.png"></td><td class="wysiwyg-text-align-justify" style="width: 625px; height: 44px;"><p>Na importação de um CT-e, quando este é vinculado a uma nota de venda&nbsp;com frete <strong>"Incluso"</strong>, o valor do frete do <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360044596834-Conhecimento-de-Transporte-Eletr%C3%B4nico-CT-e" target="_blank" rel="noopener noreferrer">CT-e</a> será gravado no campo<strong> "VLr. frete pago"</strong>.</p></td></tr><tr style="height: 10px;"><td style="width: 52px; height: 10px;">&nbsp;</td><td style="width: 625px; height: 10px;">&nbsp;</td></tr></tbody></table>

[\[voltar ao topo\]](#top)

## Concluindo a Ordem de Despacho

No processo de vendas da empresa, tem-se um processo denominado [Ordem de Despacho](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110253-Ordem-de-Despacho); é um documento composto por todas Notas Fiscais que formam a carga a ser transportada.

O processo de geração das Ordens de Despacho é feito quando as notas fiscais são faturadas, transmitidas e aprovadas pela SEFAZ. Feito isso, é lançada uma Ordem de Despacho, onde efetua-se o vínculo de todas as notas fiscais emitidas e que serão nela transportadas. Para cada transportadora é lançada uma Ordem de Despacho.

Depois de vinculadas as notas na Ordem de Despacho, esta precisa ser concluída (botão Concluir). Ao concluí-la, será feita a solicitação de quantos volumes o documento possui; uma vez informada esta quantidade, o sistema faz sua validação juntamente com a quantidade de volumes das notas fiscais vinculadas à ela.

Além da solicitação de volume, na conclusão da Ordem de Despacho é feita a geração dos pedidos de frete pertinentes às notas fiscais vinculadas à Ordem de Despacho; antes da geração dos pedidos de frete propriamente dita, será calculado o valor do frete de cada pedido. Para isso, é feito o agrupamento das notas por cliente, somam-se os valores do peso e metragem cúbica, e tem-se a aplicação destes valores na fórmula de cálculo do frete da transportadora.

<table style="border-collapse: collapse; width: 100%;" border="0,5"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 7.57143%;"><img src="/hc/article_attachments/42310717645591" alt="Atenção FINAL.png"></td><td class="wysiwyg-text-align-justify" style="width: 92.4286%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">A regra de cobrança de cada transportadora precisa estar definida na <a class="topiclink" href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360044599534-Tabelas-para-c%C3%A1lculo-de-frete" target="_blank" rel="noopener noreferrer">Tabelas para cálculo de frete</a>. Ao concluir a Ordem de Despacho, o valor de frete de cada pedido será obtido conforme esta fórmula. As notas de venda vinculadas ao pedido de frete gerado terão o valor de frete rateado, se necessário, e atualizado.</span></td></tr><tr><td style="width: 7.57143%;">&nbsp;</td><td style="width: 92.4286%;">&nbsp;</td></tr></tbody></table>

Os [Eventos para Cálculo de Frete](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603334-Eventos-para-C%C3%A1lculo-de-Frete) inseridos na [Tabelas para cálculo de frete](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044599534-Tabelas-para-c%C3%A1lculo-de-frete), aba Rotas, campo **"****Evento"**, devem possuir [Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Servi%C3%A7o) vinculados a eles, pois estes serão utilizados para gerar os itens dos pedidos. As Tabelas para cálculo de frete devem estar com o campo Rateio frete adequadamente configurado, dentre as opções Metro Cúbico, Valor da nota ou Peso.

<table style="border-collapse: collapse; width: 100%; height: 99px;" border="0,5"><tbody><tr style="height: 89px;"><td class="wysiwyg-text-align-center" style="width: 7.57143%; height: 89px;"><img src="/hc/article_attachments/42310717645591" alt="Atenção FINAL.png"></td><td class="wysiwyg-text-align-justify" style="width: 92.4286%; height: 89px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Nos casos em que o transporte da mercadoria for realizado pelos </span><span class="wysiwyg-underline"><span style="font-family: Verdana,Geneva,Arial,sans-serif; text-decoration: underline;">Correios</span></span><span style="font-family: Verdana,Geneva,Arial,sans-serif;">, a geração de Pedidos de Frete na finalização da Ordem de Despacho não irá ocorrer; para os Correios, o sistema irá se comportar conforme descrito no tópico <a class="topiclink" href="#comoconsideraroscorreiosnoclculodamelhortransportadora">Como considerar os Correios no cálculo da melhor transportadora?</a>.</span></td></tr><tr style="height: 10px;"><td style="width: 7.57143%; height: 10px;">&nbsp;</td><td style="width: 92.4286%; height: 10px;">&nbsp;</td></tr></tbody></table>

Na conclusão da Ordem de Despacho, serão gerados os Pedidos de Frete, além da impressão da Minuta de Despacho. Para geração dos pedidos de frete, através da tela **"Comercial > Consulta > Modelo de Notas e Pedidos"** deve-se configurar um modelo de nota e informar seu Número Único no parâmetro **"Modelo p/ pedidos de frete na Ordem de Despacho - MODELOPEDFRETE"**.

Além disso, ainda tratando sobre a conclusão da Ordem de Despacho, quando o parâmetro **"Aquisição de serviço de frete com frete incluso - AQSERVFRETINC"** estiver ativado e o Tipo de Frete for **"CIF"** e **"Incluso"**, mais precisamente no rateio do frete entre as notas do pedido de frete, o valor rateado será registrado no campo **"Vlr. frete calc."** localizado na aba [Transporte](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612414-Central-de-Vendas#abatransporte) da [Central de Vendas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612414-Central-de-Vendas).

Caso a marcação **"Transportadora própria"** presente na [Aba Identificação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Parceiros#abaidentificao) do [Cadastro de Parceiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Parceiros), estiver realizada, indica-se que o Parceiro é ou possui a própria transportadora, e portanto não será gerado pedido de frete para ela na conclusão da Ordem de Despacho.

[\[voltar ao topo\]](#top)