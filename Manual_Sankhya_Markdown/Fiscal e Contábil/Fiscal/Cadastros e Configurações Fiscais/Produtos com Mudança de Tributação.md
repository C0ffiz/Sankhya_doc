# Produtos com Mudança de Tributação

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360044597614-Produtos-com-Mudan%C3%A7a-de-Tributa%C3%A7%C3%A3o](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044597614-Produtos-com-Mudan%C3%A7a-de-Tributa%C3%A7%C3%A3o)

---

# Produtos com Mudança de Tributação

 ![Módulo 36x36 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42312946395543) **Módulo:** Livros Fiscais > Arquivos

---

Por meio desta tela, é possível gerar as informações que compõem o **Inventário de Mudança de Tributação de Produtos em Estoque**, sempre que houver **alterações na tributação aplicável aos itens**. Esse inventário será registrado por meio da tela [EFD - Escrituração Fiscal Digital - ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607614), utilizando o **Bloco H do SPED Fiscal**, especificamente o **registro H020**, que reflete os valores processados conforme os parâmetros definidos nesta rotina.

**Importante:** para que o **registro H020** seja gerado corretamente, é necessário que ele esteja **habilitado nas** [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa), aba [EFD - Escrituração Fiscal Digital](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaefdescrituraofiscaldigital).

Além disso, vale destacar que o **SPED (Sistema Público de Escrituração Digital)** tem como objetivo **padronizar e oficializar** a escrituração fiscal e contábil das empresas por meio de arquivos digitais, garantindo maior controle e integração entre os fiscos.

Serão considerados os **lançamentos de notas fiscais de compras e vendas de produtos que possuam saldo em estoque**, pois são esses itens que integrarão o inventário gerado. Para isso, observe as seguintes etapas:

1.  **Realize a contagem de estoque** na tela [Contagem de Estoque](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044609694), com base na **data da mudança da tributação**;
    
2.  **Configure as novas regras de tributação** correspondentes aos tributos que sofreram alteração;
    
3.  Após esses procedimentos, **inicialize os lançamentos dos registros necessários nesta tela**, para que os dados sejam devidamente processados.
    

**Importante:** As tabelas diretamente vinculadas a esta rotina são:

*   **TGFMTP** – Inventário de Tributação de Produtos
    
*   **TGFPMT** – Produtos para Mudança de Tributação
    

Essas tabelas armazenam tanto os produtos contados na data da mudança de tributação, quanto os valores resultantes da aplicação das novas regras de tributação. Assim, na geração do arquivo da EFD, os registros do Bloco H serão validados e preenchidos com base nas informações contidas nessas tabelas.

<table style="border-collapse: collapse; width: 100%; height: 154px;" border="1"><tbody><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 50%; height: 22px;" colspan="2"><span class="wysiwyg-color-black70"><strong>Funcionalidades da tela</strong></span></td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;">&nbsp;<a href="#DetalhamentodaTela">Detalhamento da tela</a></td><td style="width: 50%; height: 22px;">&nbsp;<a href="#abaProdutoMudan%C3%A7aTributa%C3%A7%C3%A3o">Aba Produto Mudança Tributação</a></td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;">&nbsp;<a href="#Bot%C3%B5esdaTela">Botões da tela</a></td><td style="width: 50%; height: 22px;">&nbsp;<a href="#Gera%C3%A7%C3%A3odeInvent%C3%A1rioparaoRegistroH020">Geração de Inventário para o registro H020</a></td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;">&nbsp;<a href="#Gera%C3%A7%C3%A3oBlocoH-Ressarcimento/ComplementoICMSST-RS">Geração Bloco H - Ressarcimento...&nbsp;</a></td><td style="width: 50%; height: 22px;">&nbsp;</td></tr></tbody></table>

## **Aba Detalhamento da tela**

Ao acessar esta tela, inicialmente, o sistema disponibilizará a visualização das seguintes opções:

![PMT1.png](https://ajuda.sankhya.com.br/hc/article_attachments/17998890270103)

Diante disso, ao acionar o botão ![botão novo registro. FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/17999337045399)**"Novo Registro"**, pode-se realizar a inserção de um cadastro. 

**Importante:** em relação a esta tela serão considerados dois tipos de registros, sendo estes **"Digitados"** e **"Não Digitados"**.

Inicialmente, insira as devidas informações nos campos contidos no Cabeçalho desta tela, conforme especificações abaixo:

![Produtos com Mudança de Tributação.png](https://ajuda.sankhya.com.br/hc/article_attachments/31912052121495)

Por meio do campo **"Empresa"** insira o código da empresa correspondente ao inventário.

Por meio do campo **"Status EFD"** o sistema irá verificar na tela a situação em que encontra-se a Escrituração Fiscal Digital; posto isto, estas informações serão inseridas automaticamente pelo sistema considerando as opções **"Liberado"** ou **"Pendente"**.

**Observação:** esse campo não poderá ser alterado, uma vez que se trata de um campo informativo.

Informe no campo **"Dt. Ref. da escrituração"** em qual referência de geração da EFD as informações desta tela serão utilizadas.

No campo **"Dt. Mud. Tributação"**, realize o registro a data da mudança da tributação. Caso tente inserir um horário neste campo, o sistema apresentará a mensagem:

_**"Não é permitido informar hora em "Dt. Mud. Tributação". Por favor, revise o cadastro!"**_

**Nota:**  para registros de inventário que não tenha relação com mudança de tributação, a data do inventário deve ser indicado na tela [EFD - Escrituração Fiscal Digital - ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607614-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI), aba [Parâmetros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607614-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI#abaparmetros), campo **"Data do Inventário"** ou na tela [EFD - Fiscal ICMS IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/7267044122263-EFD-Fiscal-ICMS-IPI), na aba [Configurações](https://ajuda.sankhya.com.br/hc/pt-br/articles/7267044122263-EFD-Fiscal-ICMS-IPI#abaconfigura%C3%A7%C3%B5es), campo **"Data do Inventário"**. 

Nesta aba teremos as seguintes sub-abas e seções:

<table style="border-collapse: collapse; width: 100%;" border="1"><tbody><tr><td style="width: 50%;"><span class="wysiwyg-color-black70"><span style="color: #0d0d0d; background-color: #ffffff;">&nbsp;<a href="#abaGeral">Sub-aba Geral</a></span></span></td><td style="width: 50%;"><a href="#Se%C3%A7%C3%A3oPar%C3%A2metrosdeC%C3%A1lculodeImpostos">Seção Parâmetros de Cálculo de Impostos</a></td></tr></tbody></table>

[\[voltar ao topo\]](#top)

### **Aba Geral**

Considerando as informações pertinentes a aba em referência, deve-se analisar o detalhamento a seguir:

O campo **"Custo"**, refere-se ao custo do inventário a ser considerado na geração do Bloco H. Este possui as seguintes opções:

*   Custo de Reposição;
*   Custo Gerencial;
*   Custo Médio com ICMS;
*   Custo Médio sem ICMS;
*   Custo Médio Gerencial;
*   Custo Variável;
*   Entrada com ICMS;
*   Entrada sem ICMS.

Em relação ao campo **"Motivo do Inventário"**, este deverá compor as informações do bloco H considerando também a geração do  EFD-ICMS/IPI. Posto isso, pode-se selecionar uma das opções abaixo:

*   02 - Na mudança de forma de tributação da mercadoria (ICMS);
*   04 - Na alteração de regime de pagamento;
*   05 - Por determinação dos fiscos;
*   06 - Para controle das mercadorias sujeitas ao regime de ST - restituição/ressarc/compl.

O campo **"Considerar empresa p/ busca da última compra"** será utilizado para identificar a última nota de compra do produto **somente quando** a opção **"Gerar SPED com os valores de ST (Compra)"** estiver **desmarcada**.

Quando a opção **"Gerar SPED com os valores de ST (Compra)"** estiver ativada, a rotina de **mudança de tributação** passa a considerar os **impostos retidos nas operações de entrada**, utilizando esses valores na composição do **registro de inventário** a ser gerado no arquivo SPED.

A marcação **"Pela média das notas que amparam o estoque"** determina se o processamento dos produtos será realizado com base na **média das notas de compra que compõem o estoque**. Essa opção estará habilitada **somente quando** o campo **"Motivo do Inventário"** estiver configurado com as opções **"02 - Na mudança de forma de tributação da mercadoria (ICMS)"** ou **"05 - Por determinação dos fiscos"**.

Ao efetuar a marcação e realizar o processamento, o sistema buscará as notas de entrada que amparam o estoque, apresentando-as na sub-aba **"Notas do Produto Com Mudança de Tributação"** (aba [Produto Com Mudança de Tributação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044597614#abaprodutomudanatributao)).

**Observação:** os valores processados nesta tela **impactarão diretamente a geração do registro H020 no SPED Fiscal**, uma vez que a base de cálculo dos impostos que compõem o registro de inventário será definida exatamente por esses valores.

Com a marcação **"Separa ICMS Normal e ICMS/ST em dois registros H020"** ativada, ao gerar o SPED Fiscal EFD ICMS/IPI, serão gerados **registros individuais para ICMS e ICMS/ST**. Nessa condição, as informações preenchidas nos campos da aba **Produto com Mudança de Tributação** serão utilizados para a geração dos registros.

Caso habilite a marcação **"Soma ICMS Normal e ICMS/ST em um único registro H020"**, ao gerar o SPED Fiscal EFD ICMS/IP será gerado apenas **um único registro** para ambos os impostos.

Ao acionar a marcação **"Considerar ICMS Anterior e ST Anterior e Extra Nota"**, os impostos de ICMS/ST Anterior e Extra nota serão considerados na composição dos valores.

Destaca-se ainda que, as últimas 3 marcações só estarão disponíveis se a marcação **"Gerar SPED com os valores de ST (Compra)"** for habilitada.

A marcação **"Considerar Operação com Valor Unitário"** será habilitada apenas se o campo Motivo do Inventário for definido com a opção **02 - Na mudança de forma de tributação da mercadoria (ICMS)** e **05 - Por determinação dos fiscos**, o que fará com que o sistema considere, na geração dos registros do  SPED Fiscal EFD ICMS/IPI, os valores unitários, caso a marcação esteja desativada esses valores serão gerados de forma total.

### **Seção Parâmetros de Cálculo de Impostos**

No campo **"Parceiro"** preencha o código do parceiro tendo este sido registrado anteriormente na tela [Cadastro de Parceiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Parceiros).

Insira no campo **"Tipo de Operação"** o código correspondente à [TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360025388653-Tipos-de-Opera%C3%A7%C3%A3o-TOP) utilizada.

Ao marcar a opção **"Utilizar alíquota de ICMS para cálculo"** durante a simulação dos valores, o sistema buscará uma **alíquota de ICMS cadastrada** e, se encontrada, a utilizará no cálculo dos impostos. Caso não haja uma alíquota de ICMS disponível, será considerada, para o cálculo, a **alíquota interna** mencionada anteriormente.

Ao acionar marcação **"Utilizar valor de custo quando não tiver ST na com..."** o sistema utilizará o valor de custo para compor as informações de ST.

No campo **“Alíquota Interna”** o usuário deverá preencher indicando a alíquota interna a ser aplicada na simulação dos valores.

Quando a marcação **"Usar ST anterior quando não tiver ST na compra"** for habilitada, o sistema durante o rastreamento dos produtos usará o ST anterior caso não encontre o ST na compra.

[\[voltar ao topo\]](#top)

## **Aba Produto Mudança Tributação**

Associe um produto a uma nova regra de tributação usando esta aba.

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4416288011671)

Preencha o campo **"Produto"**  para iniciar o processo. Para isso, antes de informar o código do item para vincular à regra no campo "**Produto"**, certifique-se de que está cadastrado na tela **Cadastro de Produtos** e configurado para ser considerado na contagem. 

As notas exibidas na subaba **"Notas do Produto com Mudança de Tributação"** são filtradas pela sua **Data de Entrada ou Saída**.

 ![Atenção FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/35473343115159) A opção **Consultar/Alterar Múltiplos Componentes** é habilitada ao selecionar um item.

Em relação ao campo **"Grupo"**, deve-se registrar neste, o grupo vinculado ao produto.

No campo **"NCM"**, é necessário registrar o código de oito dígitos referente a Nomenclatura Comum do Mercosul.

No campo **"Unidade Padrão"** registre a unidade de venda do produto; aqui pode ser inserido, por exemplo: unidade, caixa, pacote, dentre outros.

Por meio do campo **"Usado como"** pode-se especificar qual é a funcionalidade do produto, assim, tem-se as opções abaixo:

*   Subproduto;
*   Prod. Intermediário;
*   Brinde;
*   Consumo;
*   Revenda (por fórmula);
*   Embalagem;
*   Brinde (NF);
*   Imobilizado;
*   Matéria-Prima;
*   Outros Insumos;
*   Em Processo;
*   Revenda;
*   Terceiros;
*   Venda (fabricação própria).

No campo **"Estoque"**, será necessário registrar as informações da quantidade apresentada na contagem de estoque.

Por meio do campo **"Digitado?"**, pode-se visualizar os registros referentes aos cadastros Digitados ou Não Digitados.

Ao acionar a marcação **"Valor de custo utilizado"**, caso o sistema não tenha encontrado valores de ST no item, o custo selecionado no campo **"Custo"** da aba [Geral](#h_01EGRE5QGK4YD100WAXSSXV3HJ) será utilizado para o preenchimento dos valores do registro H020.

#### **Valores simulados**

**![Valores simulados.png](https://ajuda.sankhya.com.br/hc/article_attachments/31912052125079)**

Essa seção será apresentada quando a marcação **Gerar SPED com os valores de ST (Compra)** da aba Geral estiver desativada e os campos da seção Parâmetros de Cálculo de Impostos estiverem bem definidos. 

Os valores apresentados nessa seção serão calculados com base no custo da mercadoria aplicando a alíquota obtida durante a simulação realizada com os valores obtidos e definidos na seção **Parâmetros de Cálculo de Impostos** da aba Geral.

*   **Campos especificos desta seção**

No campo **"Cód. Alíq. ICMS"** preencha o código correspondente a Alíquota de ICMS. Este será preenchido automaticamente pelo sistema conforme os registros contidos no campo **"Código"** localizado na tela [Alíquotas de ICMS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044602934-Al%C3%ADquotas-de-ICMS), tópico [Cadastrando uma Alíquota de ICMS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044602934-Al%C3%ADquotas-de-ICMS#cadastrandoumaalquotadeicms).

Em relação ao campo **"Tributação"**, é necessário registrar neste o código da situação tributária conforme especificações contidas na tela [Alíquotas de ICMS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044602934-Al%C3%ADquotas-de-ICMS), aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044602934-Al%C3%ADquotas-de-ICMS#abageral), campo **"Tributação"**.

Para o preenchimento do campo **"Base ICMS"** considere o registro H020, , verifique se o CST for diferente de 10, 30, 60 e 70, a base de cálculo será o valor do item (valor unitário do produto x quantidade).

O campo **"Vlr. ICMS"** possui o valor da alíquota de ICMS de acordo com as estruturas de cálculos abaixo:

Se o CST for diferente de 10, 30, 60 e 70 tem-se a seguinte estrutura (Base de Cálculo H020 x Alíquota).

Diante disto, observe:

**Base de Cálculo H020:** R$ 150,00  
  
**Alíquota:** 12%  
  
**Resolução:** R$ 150,00 x 0,12 = R$ 18,00  
  

Consta no campo **"MVA"**, a Margem de Valor Agregado conforme regra fiscal atual do produto.

No caso do campo **"Alíquota ST"**, considere a alíquota da substituição tributária conforme regra fiscal atual do produto.

Para o preenchimento do campo **"Base Substituição"** considere o registro H020, , verifique se o CST for igual a 10, 30, 60 e 70, terá como inicialmente o valor do item (valor unitário do produto x quantidade), sendo majorada pelo MVA, com o Valor do item x (1+MVA). Assim, considere o exemplo a seguir:

**Valor Unitário:** R$ 150,00

**Quantidade:** 1

**Valor do item:** R$ 150,00

**MVA:** 45,33%

Portanto, R$ **150,00** x (**1**+**0,4533**) = R$ **150,00** x **1,4533** = R$ **218,00**

Já no campo **"Vlr. Substituição"**, se o CST for igual a 10, 30, 60 e 70 tem-se a estrutura (Base de Cálculo H020 x Alíquota ST) - (Quantidade do produto em estoque x Valor do ICMS Unitário). Mediante isso, segue o exemplo:  
  
**Base de Cálculo H020:** R$ 218,00  
  
**Alíquota ST:** 18%  
  
**Quantidade do produto em estoque:** 1  
  
**Valor do ICMS Unitário:** R$ 14,40  
  
**Resolução:** (R$ 218,00 x 0,18) - (1 x R$ 14,40) = R$ 39,24 - R$ 14,40 = R$ 24,84.

**Valores Recuperados (Estoque)**

**![Valores recuperados.png](https://ajuda.sankhya.com.br/hc/article_attachments/31912022827031)**

Essa seção será exibida quando a marcação **"Gerar SPED com os valores de ST (Compra)"**, localizada na aba [Geral](#abaGeral), estiver habilitada.

Os valores apresentados serão calculados com base nas notas fiscais de entrada listadas na sub-aba **Notas do Produto com Mudança de Tributação**, desde que a opção **"Pela média das notas que amparam o estoque"**, também na aba [Geral](#abaGeral), esteja ativada.

Caso essa opção esteja desativada, os valores serão obtidos com base na **última nota de compra** informada nos campos **"Nro. Único Compra"** e **"Parceiro da Compra"**, sendo proporcionalizados ao total do estoque.

[\[voltar ao topo\]](#top)

## **Botões da tela**

Em relação aos botões visualizados no canto superior esquerdo desta tela, pode-se verificar as seguintes funcionalidades:

 ![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/4416507476247) **Importar:** ao utilizar esse botão, o sistema buscará todos os produtos ativos que tenham  sido considerados na contagem de estoque conforme data da mudança da tributação,  assim como, a empresa informada, desse modo, o sistema realizará as devidas importações.

**Nota:** ao solicitar a importação de produtos considerando que tenham sido classificados como Digitados, os valores inseridos não serão sobrepostos.

**Observação:** com o parâmetro **"Somente produtos ativos ao imp. mud. tributação? - PRODATIVMUDTRIB"** desligado, pode-se realizar a importação de produtos da contagem que, em determinado período, ainda estavam ativos e, atualmente, estão desativados.

 ![mceclip3.png](https://ajuda.sankhya.com.br/hc/article_attachments/4416507541143) **Processar:** ao utilizar essa opção, o sistema irá processar as informações relacionadas aos produtos Não Digitados. 

Quando um novo processamento for realizado considerando a mesma data, o sistema irá proceder com a solicitação sobrepondo as informações anteriores.

 ![mceclip4.png](https://ajuda.sankhya.com.br/hc/article_attachments/4416520826775) **Liberar EFD:** por meio desse botão, o sistema procederá com a liberação das informações para a geração do Bloco H da EFD-ICMS/IPI. Deste modo, o campo **"Status"** contido na presente tela apresentará a opção **"Liberado"**.

**Observação:** quando realizado o registro da EFD - ICMS/IPI do mês em referência da data da mudança da tributação, o sistema considerará estas informações para o preenchimento do Bloco H.

 ![CP81](https://ajuda.sankhya.com.br/hc/article_attachments/360060985634) **Configuração da tela:** nesse botão, temos a opção **"Processar ao importar os produtos"** que irá realizar as importações e processamentos dos produtos.

**Nota:** ao realizar o procedimento acima, o sistema deverá inserir uma linha por produto.

 ![mceclip5.png](https://ajuda.sankhya.com.br/hc/article_attachments/4416508179223) **Excluir Dig./Não:** por meio deste, será exibido o pop-up **"Excluir os registros"**:

![mceclip6.png](https://ajuda.sankhya.com.br/hc/article_attachments/4416508267031)

Diante disso, pode-se remover os registros inseridos na aba Produto Mudança Tributação. Assim, considere:

1.  No campo **"Digitados"**, exclua os registros que foram inseridos no sistema;
2.  Ao considerar o campo **"Não Digitados"**,o sistema permitirá excluir os registros que foram anteriormente importados;
3.  Em relação ao campo "Ambos", pode-se realizar a exclusão de todos os registros especificados nesta tela.

Em relação à rotina de **"Processar"**, considere que, ao habilitar o parâmetro **"Exigir CR na central/financeiro/rateio? - EXIGCRCFR"**, o sistema localizará o Centro de Resultado com o menor código, que encontre-se ativo, analítico e com o código diferente de 0, e assim, este será utilizado primeiro. Caso não localize nenhum Centro de Resultado nessas condições, será exibida a mensagem a seguir:

_**"Erro ao tentar inserir modelo de Mudança de Tributação.**_

_**Não foi encontrado nenhum Centro de Resultado ativo, analítico e diferente de 0.**_

_**E como o parâmetro 'EXIGCRCFR' está ligado, a operação foi abortada."**_

[\[voltar ao topo\]](#top)

## **Geração do registro de inventário de mudança de tributação - H020 (EFD Fiscal)**

Inicialmente, deve-se realizar as configurações necessárias de acordo com as especificações desta documentação.

Após este procedimento, ao considerar a Geração de Inventário para Produtos com Mudança de Tributação, deve-se acessar a tela [EFD - Escrituração Fiscal Digital - ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607614) atentando-se as informações abaixo:

*   O **"Registro H001"** tem como finalidade gerar o conteúdo para a abertura do Bloco H especificando se existem informações no bloco mencionado;
*   No **"Registro H005"**, considere os valores totais dos produtos relacionados ao inventário;
*   Por meio do **"Registro H010"**, deve-se discriminar os produtos em estoque que compõem o inventário;
*   No **"Registro H020"** insira as informações complementares do inventário.

Ainda nesse contexto, ao acessar a tela mencionada anteriormente e considerar as informações registradas no campo **"Período"**, o sistema irá buscar e verificar as datas da mudança da tributação em um período específico.

**Nota:** o registro H020 não é gerado para o inventário físico no final do período. Caso necessário, após realizar os devidos lançamentos na tela [E](https://ajuda.sankhya.com.br/hc/pt-br/articles/360025394113-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI)[FD](https://ajuda.sankhya.com.br/hc/pt-br/articles/360025394113-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI) [-](https://ajuda.sankhya.com.br/hc/pt-br/articles/360025394113-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI) [Escritura](https://ajuda.sankhya.com.br/hc/pt-br/articles/360025394113-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI)[ção](https://ajuda.sankhya.com.br/hc/pt-br/articles/360025394113-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI) [Fiscal Digital - ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360025394113-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI), realize os registros das informações complementares sobre o inventário na tela [Preferência da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360025239374-Empresa), aba [EFD - Escrituração Fiscal Digital](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Empresa#abaefdescrituraofiscaldigital), sub-aba "Blocos e Registros" considerando o registro H020.

**Importante:** quando analisado um mesmo período para a Geração da EFD, considerando que o campo **"Data do Inventário"** ([E](https://ajuda.sankhya.com.br/hc/pt-br/articles/360025394113-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI)[FD](https://ajuda.sankhya.com.br/hc/pt-br/articles/360025394113-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI) [-](https://ajuda.sankhya.com.br/hc/pt-br/articles/360025394113-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI) [Escritura](https://ajuda.sankhya.com.br/hc/pt-br/articles/360025394113-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI)[ção](https://ajuda.sankhya.com.br/hc/pt-br/articles/360025394113-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI) [Fiscal Digital - ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360025394113-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI), aba [Parâmetros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607614?flash_digest=f31de3953cd803e803e837c011084a1e2baff0c2#abaparmetros)) esteja preenchido, e simultaneamente, as informações contidas na tela Produtos com Mudança de Tributação forem liberadas, deve-se proceder com a inserção de dois inventários.

Diante do exposto, considere as seguintes especificações:

*   Inventário padrão - final do período (Motivo 01);
*   Inventário relacionado a Mudança de Tributação de Produtos (Motivo 02).

[\[voltar ao topo\]](#top)

 ![acesse também FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16345204746519) Para maiores detalhes sobre este conteúdo, acesse os seguintes artigos:

[Dicionário de Dados](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044597294)

[Detalhamento da tela](#detalhamentodatela) 

[Aba Geral](#abageral)

[Aba Produto Mudança Tributação](#abaprodutomudanatributao)

[Botões da tela](#botesdatela)

[Geração do Inventário para](#geraodeinventrioparaoregistroh020) [o registro H020](#geraodeinventrioparaoregistroh020) 

[Geração Bloco H-Ressarcimento/Complemento ICMS ST - RS](#geraoblocoh-ressarcimentocomplementoicmsst-rs)