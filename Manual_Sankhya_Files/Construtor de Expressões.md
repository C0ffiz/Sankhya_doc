# Construtor de Expressões

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360045109213-Construtor-de-Express%C3%B5es](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045109213-Construtor-de-Express%C3%B5es)

---

# Construtor de Expressões

O Sankhya-Om dispõe do componente Construtor de Expressões que pode ser acessado através das seguintes telas:

*   [Fórmulas para Desconto Máximo](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044600314-F%C3%B3rmulas-para-Desconto-M%C3%A1ximo);
*   [Fórmulas de Comissão](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045108013-F%C3%B3rmulas-de-Comiss%C3%A3o);
*   [Fórmulas para Cálculo de frete](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044600334-F%C3%B3rmulas-para-C%C3%A1lculo-de-frete);
*   [Fórmulas de Custo/Preço](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044599874-F%C3%B3rmulas-de-Custo-Pre%C3%A7o);
*   [Fórmulas para ICMS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601534-F%C3%B3rmulas-para-ICMS).

Dessa forma, você pode conferir as usabilidades do Construtor de Expressões por meio dos seguintes links:

[Acessando o Construtor Expressões](#acessandooconstrutorexpress%C3%B5es)                        [Construtor MGE x Sankya-Om](#construtormgexsankhya-om)

[Campos adicionais MGE...](#camposadicionaismge...)                                            [Variáveis disponíveis no Componente](#vari%C3%A1veisdipon%C3%ADveisnocomponente)

[Funções empregadas na Edição de Fórmulas](#fun%C3%A7%C3%B5esempregadasnaedi%C3%A7%C3%A3odef%C3%B3rmulas)

## Acessando o Contrutor Expressões

Para acessá-lo, basta clicar no botão  ![botão-Fx-construtor.FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16190944763927) **"f(x) Construtor"**; como na tela Fórmulas para Desconto Máximo. Dessa forma, o contrutor listará as categorias de funções, variáveis e banco de dados.

![atalho\_construtor.gif](https://ajuda.sankhya.com.br/hc/article_attachments/1500008984021)

No lado esquerdo do componente temos a árvore de categorias, onde são exibidas as categorias, suas sub-categorias e os itens. Esses itens podem ser adicionados ao campo de expressão localizado no lado direito do componente, com duplo clique ou sendo arrastado.

Entre a árvore de categorias e a área para a contagem da expressão, temos os operadores, que você pode adicioná-los com apenas um clique.

![data.gif](https://ajuda.sankhya.com.br/hc/article_attachments/1500008984741)

No Construtor, temos a marcação **"Acrescentar no final da expressão"**, em que, quando estiver selecionada e um novo item for adicionado, este irá para o final da expressão criada. Se a marcação não for realizada, o item será inserido de acordo com a posição do cursor do mouse na expressão.

O botão **"Limpar"** é utilizado para apagar toda a expressão.

Ao clicar em **"OK"**, a expressão construída irá para o campo **"Fórmula"** da tela que chamou o componente, em seguida, você pode clicar no botão **"Salvar"** para gravar a nova expressão.

Se você clicar no botão **"Cancelar"**, o componente é fechado e nada será inserido no campo **"Fórmula"** da tela que chamou o componente.

[\[voltar ao topo\]](#top)

## Construtor de Expressões MGE x Sankhya-Om

Ao escolher uma função no MGE, o sistema apresenta os parâmetros dessa função para que valores sejam adicionados. Já no Sankhya-Om, quando uma função for escolhida na descrição, os parâmetros dela irão para a expressão, assim, você deve inserir os valores dos parâmetros manualmente.

No MGE, é possível alterar os valores de variáveis quando a expressão for montada; no Sankhya-Om, essa funcionalidade não está disponível.

[\[voltar ao topo\]](#top)

## Campos adicionais do MGE e Categoria Banco de Dados

Quando houverem campos adicionais na categoria de banco de dados do componente de expressão do MGE, o Sankhya-Om irá listá-los somente ao selecionar a opção **"Processar campo MGE/Mitra"** da tela [Dicionário de Dados](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044597294-Dicion%C3%A1rio-de-Dados#botooutrasopes).

Dependendo da tela, os campos adicionais poderão aparecer de duas formas no construtor. São elas:

*   Ao apresentar o nome do campo; como: **AD\_CAMPO1**, ou **CAMPOADICIONAL**.
    
*   Ou ambém, com o sufixo da tabela correspondente; por exemplo, se houver um campo na **TGFCAB**, ao visualizarmos pelo Construtor de Expressões o nó "queCab", teremos os campos adicionais representados da seguinte forma: **TGFCABAD\_CAMPO1**, ou **TGFCABCAMPOADICIONAL**.
    

[\[voltar ao topo\]](#top)

## Variáveis disponíveis no Componente Contrutor de Expressões

Abaixo, listamos algumas variáveis que podem aparecer no componente. Observe: 

**TOTITENS:** Valor total dos itens na nota, desconsiderando os valores informados no Cabeçalho da Nota (Frete, desconto total, juro, destaque, embalagem,...). Assim, temos a fórmula:

_TotalItens := TGFCAB.VLRNota  - TGFCAB.VLRSEG  - TGFCAB.VLRDESTAQUE_

_\- TGFCAB.VLRJURO  + TGFCAB.VLRDESCTOT  + TGFCAB.VLRDESCSERV ;_

_SE TGFCAB.TIPIPIEMB = 'I' ENTAO_

_TotalItens: = TotalItens - TGFCAB.IPIEMB - TGFCAB.VLREMB ;_

_SE TGFCAB.ISSRETIDO = 'S' ENTAO_

_TotalItens := TotalItens + TGFCAB.VLRISS ;_

_SE TGFCAB.TIPFRETE = 'S' ENTAO_

_TotalItens := TotalItens - TGFCAB.VLRFRETE ;_

_TotItens := TotalItens ;_

**VLRICM:** Valor do ICMS na Nota. Observe a fórmula:

_ICMSTotal := TGFCAB.VLRICMS ;_

_SE TGFCAB.TIPFRETE <> 'S' ENTAO_

_ICMSTotal := ICMSTotal + TGFCAB.ICMSFRETE ;_

_SE not FSegICMS ENTAO_

_ICMSTotal := ICMSTotal + TGFCAB.VLRICMSSEG ;_

_SE TGFCAB.TIPIPIEMB <> 'I' ENTAO_

_ICMSTotal := ICMSTotal + TGFCAB.VLRICMSEMB ;_

**VLRIPI:** Refere-se ao valor do IPI total do item para chegar no IPI unitário. Esse valor será dividido pelo TGFITE.QtdNeg. Considere a seguinte fórmula:

_VlrIPI  = TGFITE.VlrIPI;_

**INDFRE:** Corresponde ao índice do frete, calculado pelo valor do frete dividido pelo valor total da nota. Sendo assim, temos a fórmula:

_VlrIPI := 0 ;_

_SE TGFCAB.VLRIPI > 0 ENTAO_

_SE queTGFPAR.IPIINCICMS = 'N' ENTAO_

_VlrIPI := TGFCAB.VLRIPI ;_

_SE TGFCAB.TIPFRETE = 'S' ENTAO_

_IndFre := TGFCAB.VLRFRETE / (TGFCAB.VlrNota - TGFCAB.VLRFRETE - VlrIPI)_

_SENAO_

_IndFre := TGFCAB.VLRFRETE / TGFCAB.VlrNota ;_

_SE TGFCAB.TIPFRETE <> 'S' ENTAO_

_IndFre := 0 ;_

**INDDES:** Será o índice de desconto, calculado a partir do valor de desconto informado e o valor total da nota. Observe a fórmula:

_IndDes := TGFCAB.VLRDESCTOT / (TGFCAB.VlrNota + TGFCAB.VLRDESCTOT)_

**INDTOT:** Refere-se ao índice Total dos produtos, calculado a partir do valor total da nota dividido pelo Valor total de itens na nota. Assim, teremos:

_curTotal := TGFCAB.VlrNota ;_

_SE TGFCAB.ISSRETIDO <> 'S' ENTAO_

_curTotal := curTotal - TGFCAB.VLRISS ;_

_SE TGFCAB.TIPIPIEMB <> 'I' ENTAO_

_curTotal := curTotal + TGFCAB.IPIEMB + TGFCAB.VLREMB ;_

_SE (TGFCAB.TIPFRETE <> 'S') ENTAO_

_curTotal := curTotal + TGFCAB.VLRFRETE ;_

_IndTot := curTotal / TotalItens_

**INDICMS:** Índice de ICMS total incidido na nota, calculado pelo valor total de ICMS, incluindo ICMS frete, ICMS do seguro e outros, dividido pelo valor ICMS da nota. Considere:

_IndICMS := ICMSTotal / TGFCAB.VlrICMS_

**VLRITE:** Valor unitário do Item na Nota. Dessa forma, teremos:

_VlrIte  = TGFITE.VlrUnit_  

**QTDITE:** Quantidade Negociada de cada Item da nota. Fórmula:

_QtdIte  = TGFITE.QtdNeg;_  

**VLRXQTD:** Valor Unitário do Produto multiplicado pela TGFITE.QtdNeg. Considere a fórmula:

_VlrXQtd = TGFITE.VLRTOT;_

**VLRSUB:** Valor Total da Substituição Tributária do Item, para chegar no valor unitário da ST, dividir esse valor pelo TGFITE.QtdNeg.  Fórmula:

_VlrSub  = TGFITE.VlrSubst;_

**APPNAME:** APPSTARTDATE - APPSTARTTIME - São parâmetros internos.

**CASASDECIMAIS:** Número de casas decimais usadas para quantidade no item da nota.

**VLRPRO:** Corresponde ao valor do produto com IPI, Substituição Tributária e Desconto por Item. considere a seguinte fórmula:

_SE (TGFITE.CODCFO  = 111) or_

_(TGFITE.CODCFO  = 211) or_

_(TGFITE.CODCFO  = 1101) or_

_(TGFITE.CODCFO  = 2101) ENTAO_

_VlrPro = TGFITE.VlrUnit_

_SENAO_

_VlrPro = TGFITE.VlrUnit + (TGFITE.VLRIPI / TGFITE.QtdNeg);_

_FIM SE_

_VlrPro = Round2(VlrPro +      (TGFITE.VLRSUBST / TGFITE.QtdNeg) -_

_(TGFITE.VLRDESC / TGFITE.QtdNeg), fCustoDec);_

**ALIQICM:** É o percentual da alíquota utilizada na entrada da Mercadoria, para que calculemos o crédito do ICMS.

**ALIQVENDA:** É a alíquota de ICMS provável de venda, obtida através da simulação da Saída do Produto dentro do Estado. Considere a seguinte fórmula:

_SE TGFPRO.TIPSUBST = 'C’ ENTAO_

_VlrICM = 0;_

_Aliquota = 0;_

_AliqVenda = 0;_

_SENAO_

_VlrICM = (TGFITE.VLRICMS / TGFITE.QtdNeg);_

_Aliquota = TGFITE.ALIQICMS;_

_AbreAliqCusto(CodUF, TGFITE.CodProd, TGFPRO.CodGrupoProd, codCid);_

_AliqVenda = dmEst.queAliqALIQ \* (100 - dmEst.queAliqREDBASE) / 100);_

_FIM SE_

_AliqICM = Aliquota;_

_Procedure AbreAliqCusto_

_ABREALIQCUSTO_

_SELECT_

_I.CODTRIB,_

_I.ALIQUOTA AS ALIQ,_

_I.REDBASE,_

_I.ALIQFRETE,_

_I.REDBASEFRETE,_

_I.MARGLUCRO,_

_I.ALIQSUBTRIB,_

_P.PRIORIDADE,_

_I.CODOBSPADRAO AS CODOBS,_

_I.REPREDBASE_

_FROM TGFICM I, TGFPRI P_

_WHERE I.UFORIG = :CODUFORIG_

_AND I.UFDEST = :CODUFDEST_

_AND I.TIPRESTRICAO = P.TIPRESTRICAO1_

_AND I.TIPRESTRICAO2 = P.TIPRESTRICAO2_

_AND ( (I.TIPRESTRICAO = 'P' AND I.CODRESTRICAO = TGFITE.CODPROD) OR_

_(I.TIPRESTRICAO = 'G' AND I.CODRESTRICAO = TGFPRO.CODGRUPOPROD) OR_

_(I.TIPRESTRICAO = 'T' AND I.CODRESTRICAO = 0) OR_

_(I.TIPRESTRICAO = 'O' AND I.CODRESTRICAO = 0) OR_

_(I.TIPRESTRICAO = 'C' AND I.CODRESTRICAO = :CIDORIGEM) OR_

_(I.TIPRESTRICAO = 'D' AND I.CODRESTRICAO = :CIDDESTINO) OR_

_(I.TIPRESTRICAO = 'I' AND I.CODRESTRICAO = :GRUPOICMSPROD) OR_

_(I.TIPRESTRICAO = 'J' AND I.CODRESTRICAO = :GRUPOICMSGRUPOPROD) OR_

_(I.TIPRESTRICAO = 'R' AND I.CODRESTRICAO = 0) OR_

_(I.TIPRESTRICAO = 'S') )_

_AND ( (I.TIPRESTRICAO2 = 'P' AND I.CODRESTRICAO2 = TGFITE.CODPROD) OR_

_(I.TIPRESTRICAO2 = 'G' AND I.CODRESTRICAO2 = TGFPRO.CODGRUPOPROD) OR_

_(I.TIPRESTRICAO2 = 'T' AND I.CODRESTRICAO2 = 0) OR_

_(I.TIPRESTRICAO2 = 'O' AND I.CODRESTRICAO2 = 0) OR_

_(I.TIPRESTRICAO2 = 'C' AND I.CODRESTRICAO2 = :CIDORIGEM) OR_

_(I.TIPRESTRICAO2 = 'D' AND I.CODRESTRICAO2 = :CIDDESTINO) OR_

_(I.TIPRESTRICAO2 = 'I' AND I.CODRESTRICAO2 = :GRUPOICMSPROD) OR_

_(I.TIPRESTRICAO2 = 'J' AND I.CODRESTRICAO2 = :GRUPOICMSGRUPOPROD) OR_

_(I.TIPRESTRICAO2 = 'R' AND I.CODRESTRICAO2 = 0) OR_

_(I.TIPRESTRICAO2 = 'S') )_

_ORDER BY P.PRIORIDADE_

**CUSCOMICM:** Custo com ICMS

**CUSMEDSEMICM:** Custo Médio

**Nota:** os custos médios não podem ser utilizados no cálculo dos custos da própria nota, pois eles dependem da nota em questão. Nesse caso, para a realização do cálculo, pode-se usar os custos médios anteriores, ou os custos da nota não médios, como por exemplo o CUSSEMICM.

**CUSGER:** Custo Gerencial.

**CUSREP:** Custo de Reposição

**CUSSEMICM:** Custo sem ICMS

**CUSTOFIXO:** Custo Fixo leva em consideração o percentual informado na aba preferências do Gerente on-line.

**CUSVAR:** Refere-se ao Custo Variável.  Assim, considere a seguinte fórmula:

_CusSemCal = Round2((VlrPro \* IndTot) - (VlrICM \* IndICMS) - (VlrIcm \* IndFre), fCustoDec);_

_CusComCal = Round2((VlrPro \* IndTot), fCustoDec);_

_CusVarCal = 0;_

_CusRepCal = TGFITE.VlrUnit;_

_CusGerCal = Round2(CusSemCal -_

_(TGFITE.VlrUnit \* TaxaJuro \* intPrazoMedio / 3000), fCustoDec);_

**PRAZOMEDIO:** Prazo médio do financeiro da nota. Fórmula:

_Se fDtPAtuCust = 0 então_

_'SELECT SUM(VLRDESDOB \* (DTVENC - DTNEG)) / SUM(VLRDESDOB) AS PRZMED'_

_senão se fDtPAtuCust = 1 então_

_'SELECT SUM(VLRDESDOB \* (DTVENC - NVL(DTENTSAI, DTNEG))) / SUM(VLRDESDOB) AS PRZMED'_

_senao_

_'SELECT SUM(VLRDESDOB \* (DTVENC - DHMOV)) / SUM(VLRDESDOB) AS PRZMED';_

**TAXAJURO:** A taxa dessa variável vem do parâmetro **"Taxa de Juro - TAXAJURO"**.

**Nota:** quando a quantidade negociada da nota for igual a zero, para as TOP’s indicadas no parâmetro **"TOP para aceitar Qtd. igual a zero - TOPQTDZERO"**, o sistema carregará as variáveis AntCusComICM, AntCusSemICM, AntCusVar, AntCusRep, AntCusGer, da **"Fórmula de Custo/Preço"** com o custo anterior.

**TOTALDETALHE:** Essa variável contabiliza a quantidade de registros que estão sendo enviados em uma remessa. Alguns bancos exigem que seja enviada no HEADER (cabeçalho), a quantidade de títulos contidos no arquivo de remessa. É importante ressaltar que esta variável contabiliza apenas as linhas do detalhe, não considera HEADER e TRAILLER. Caso seja necessário, esses valores podem ser somados na expressão do campo, por exemplo, **TOTALDETALHE + 1**.

**FIMLINHA:** Acrescenta uma quebra de linha na posição final + 1 do texto retornado pela consulta; como por exemplo, **"abcd  asas aas aaaa"**.

**FIMLINHATRIMRIGHT:** Acrescenta uma quebra de linha após o último caractere diferente de espaço no texto retornado pela consulta. Como, **"abcd  asas aas aaaa"**.

**Nota:** aplicam-se apenas à configuração de arquivos de remessa de EDI.

[\[voltar ao topo\]](#top)

## Funções empregadas na Edição de Fórmulas

Nesse tópico, abordaremos sobre as funções na formatação de fórmulas, como precificação, comissão e contabilização, etc. Dessa forma, acesse os links abaixo para saber sobre cada um deles:

[Funções Lógicas](#fun%C3%A7%C3%B5esl%C3%B3gicas)                                                                          [Função BUSCATSIPAR](#fun%C3%A7%C3%A3obuscatsipar)

[Funções de Pesquisa](#fun%C3%A7%C3%B5esdepesquisa)                                                                  [Funções de Formato de Dados](#fun%C3%A7%C3%B5esdeformatodedados)

[Funções Matemáticas](#fun%C3%A7%C3%B5esmatem%C3%A1ticas)                                                                [Funções de Datas](#fun%C3%A7%C3%B5esdedatas)

## Funções Lógicas

O **"IF"** é uma função de Condição que tem o objetivo de retornar uma ou outra informação, de acordo com o atendimento à condição estabelecida.

Na tradução do Inglês para o Português, **"IF"** quer dizer **"SE"**, ou seja "no caso de", "dado a circunstância de". Portanto, é utilizada para que seja avaliada uma situação. Caso a condição seja verdadeira, a função retornará uma informação e caso seja falsa, retornará outra informação. Sendo que, a estrutura utilizada na construção de um IF, será a seguinte:

```auto
IF(<CONDIÇÃO>,<VALOR_SE_VERDADEIRO>,<VALOR_SE_FALSO>)
```

Abaixo, trouxemos alguns exemplos da utilização do IF. Observe:

*   _IF(VLRDESDOB=VLRBAIXA,VLRDESDOB,0)_: Essa fórmula é utilizada na contabilização do valor do desdobramento em uma determinada linha, se o valor do desdobramento for igual ao valor da baixa. Se os valores forem diferentes, o IF retornará zero, ou seja, não será contabilizado.
    
*   _IF(queCab.TIPMOV='V',1,-1)_: Esse exemplo sempre é empregado na construção de fórmulas de comissão. Ela diz que, se o Tipo de Movimento for Venda, deverá se considerado **"1"** e se não for, deve ser considerado **"-1"**. O resultado dessa condição será multiplicado pelo valor dos itens posteriormente para calcular comissões positivas, em casos de vendas e negativas, em casos de devoluções de vendas, sendo esses outro tipo de movimento para cálculo de comissões. 
    
*   _IF(queProd.COMVEND < queVend.COMVENDA, queProd.COMVEND, queVend.COMVENDA)_: Temos aqui, outro exemplo de condição em fórmulas de comissionamento. Aqui, considere que deseja-se obter o menor percentual na comparação entre os percentuais de comissão definidos nos cadastros de produtos e de vendedores.
    
*   _IF(queItens.VLRSUBST=0,queItens.VLRICMS/queItens.QTDNEG,0)_: Empregado em uma fórmula de precificação, esse exemplo está sendo definido que o valor do ICMS por unidade só será considerado caso o Valor da Substituição do item seja igual a zero.
    

[\[voltar ao subtítulo\]](#fun%C3%A7%C3%B5esempregadasnaedi%C3%A7%C3%A3odef%C3%B3rmulas)

---

## Funções de Pesquisa

O **"PDES"** é uma função de consulta ou busca de valores que não podem ser obtidos através das variáveis preexistentes. Com o PDES, pode ser obtido qualquer valor, ou tabela do sistema, desde que a consulta realizada através do comando retorne um único valor. Isso é possível ao realizar ligações entre o PDES e variáveis existentes que retornem campos Chave das tabelas envolvidas. Assim, temos a seguir a estrutura utilizada na construção de um PDES:

```auto
PDES('<COLUNA>','<TABELA(S)>', '<CONDIÇÃO(ÕES)> ')
```

A estrutura da função é semelhante à estrutura do SELECT, utilizado para consultar informações no banco de dados; porém, para o uso do PDES, é necessário possuir noções sobre Banco de Dados e a estrutura das tabelas utilizadas pelo sistema.

Quanto às condições, normalmente é realizada uma ligação entre a tabela que está sendo consultada e uma variável pré-existente. A união entre uma parte fixa do comando e uma parte variável, deve ser realizada através do sinal **"+"**, sendo que as partes fixas do comando devem estar entre aspas simples da seguinte forma:

```auto
PDES('<COLUNA>','<TABELA(S)>',<'PARTE_FIXA'+PARTE_VARIAVEL>)
```

Por meio dos exemplos descritos a seguir, temos suas aplicações:

*   _VAL(PDES('SUM(VLRICMS)','TGFITE','VLRSUBST=0 AND NUNOTA='+NUNOTA))_: Esse PDES pode ser aplicado em uma Fórmula de Contabilização e retornará a soma do valor do ICMS dos itens que não possuem Substituição Tributária, na nota que está sendo contabilizada. A variável **"NUNOTA"** foi utilizada como ligação para que o PDES retornasse um único resultado. Além do PDES, foi utilizada a função VAL, para converter o valor encontrado pelo PDES em VALOR. Os dados retornados pelo PDES estão sempre em formato de texto. Se for necessário utilizar o dado retornado como valor na contabilização, utilize também a função VAL para converter o valor retornado pelo PDES em número.
    
*   _VAL(IF(PDES('ISSRETIDO','TGFCAB','NUNOTA='+NUNOTA)='S',PDES('VLRISS','TGFCAB','NUNOTA='+NUNOTA),0))_: Aqui, foi utilizado também o IF. Ao realizar a leitura, o IF verifica se o campo **"ISS Retido"** do cabeçalho da nota está igual à **"Sim"**, se estiver, o sistema buscará o conteúdo do campo **"Valor do ISS"** da Nota. Essa expressão pode ser utilizada, por exemplo, nas fórmulas das parcelas dos [Tipos de Negociação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045109173-Tipos-de-Negocia%C3%A7%C3%A3o), para gerar uma parcela de despesa para pagamento do ISS retido de um prestador de serviços. A variável **"NUNOTA"** também foi utilizada como ligação para que o **PDES** retornasse um único resultado.
    

[\[voltar ao subtítulo\]](#fun%C3%A7%C3%B5esempregadasnaedi%C3%A7%C3%A3odef%C3%B3rmulas)

---

## Função BUSCATSIPAR

Essa função é utilizada para retornar o valor contido em um determinado parâmetro. Sendo que, minimiza as alterações em fórmulas, principalmente de precificação e comissionamento, quando algum dos percentuais fixos envolvidos nesses cálculos, forem alterados. Como, por exemplo: _BuscaTSIPAR('PERCCUSFIXO')_

O percentual de Custo Fixo utilizado na análise de rentabilidade de notas e pedidos é definida através das [preferências do Gerente On-line](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045108853-Prefer%C3%AAncias-Gerente-On-line) e armazenada no parâmetro **"Percentual custo fixo - PERCCUSFIXO"**. Para que as fórmulas de precificação considerem o mesmo percentual definido nas [Preferências](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601834-Prefer%C3%AAncias), basta utilizar a expressão **"BuscaTSIPAR('PERCCUSFIXO')"** na fórmula.

O mesmo pode ser realizado com o percentual de comissão fixo definido nas Preferências do Gerente On-line, que fica armazenado no parâmetro **"Percentual de Comissão -PERCCOMISSAO"**, ou qualquer outro parâmetro que contenha valores a serem empregados nas fórmulas do sistema. Você também pode criar um parâmetro personalizado para armazenar determinado valor e utilizá-lo com a função BuscaTSIPAR. Assim, se o valor for alterado, basta mudar o conteúdo do parâmetro.  
 

⚠️ **Atenção:** A função `BuscaTSIPAR()` utiliza como parâmetro o **código do usuário logado** no momento da execução. Como é possível criar parâmetros individualizados **por usuário** no sistema, caso esta função seja utilizada em **Fórmulas de Comissão ou de Custo/Preço**, o cálculo e o recálculo poderão apresentar **valores diferenciados para uma mesma nota ou período**, dependendo de qual usuário estiver logado ao processar as informações.

Por isso, recomenda-se atenção ao utilizar a função `BuscaTSIPAR()` em fórmulas que exijam consistência de valores entre diferentes usuários.

[\[voltar ao subtítulo\]](#fun%C3%A7%C3%B5esempregadasnaedi%C3%A7%C3%A3odef%C3%B3rmulas)

---

## Funções de Formato de Dados

Funções de formato de dados, normalmente são empregadas para criação de EDI's, onde os valores de cada campo, devem respeitar os padrões definidos em um layout. Abaixo, você pode conferir algumas das mais importantes funções de definição de formato de dados.

A funções **"Copy"** e **"Substr"** são utilizadas para extrair uma parte de uma variável e funcionam exatamente da mesma forma; por exemplo, extrair apenas o "DDD" do número de telefone, a raiz do CEP, parte do CNPJ, etc. Dessa forma, a estrutura utilizada na construção dessas funções é a seguinte:

```auto
COPY(<VARIÁVEL>,<CARACTERE_INICIAL>,<NÚMERO_DE_CARACTERES>)

SUBSTR(<VARIÁVEL>,<CARACTERE_INICIAL>,<NÚMERO_DE_CARACTERES>)
```

Considere o seguinte exemplo:

A variável **"Dados\_Detalhe.CEP\_PARCEIRO"** retorna no CEP do parceiro com 8 posições, sem separadores. Se o layout do EDI solicitar a impressão de CEP com a máscara "99.999-999", por exemplo, poderá ser utilizado:

```auto
COPY(Dados_Detalhe.CEP_PARCEIRO,1,2)+'.'+COPY(Dados_Detalhe.CEP_PARCEIRO,3,3)+'-'+COPY
(Dados_Detalhe.CEP_PARCEIRO,6,3)
```

Primeiramente pegamos a partir do primeiro, dois caracteres e relacionamos com um ponto final. Em seguida, conectamos com os três próximos caracteres, a partir do terceiro e com um hífen. Por último, unimos também com os três últimos, a partir do sexto caractere.

Na geração do EDI, a concatenação é realizada através do sinal **"+"**.

O objetivo das funções **"Left"** e **"Right"**, é imprimir apenas uma parte de um texto, de forma semelhante ao que ocorre nas funções Copy e Substr. A diferença é que nas funções Left e Right não é apontado o caractere inicial do "corte", pois a geração sempre acontece do início do texto à esquerda ou à direita. Dessa forma, considere a estrutura para utilização dessas funções:

```auto
LEFT(<VARIÁVEL>,<NÚMERO_DE_CARACTERES>)

RIGHT(<VARIÁVEL>,<NÚMERO_DE_CARACTERES>)
```

Como exemplo, suponhamos que na geração de determinado arquivo de EDI, serão permitidos 30 caracteres para o nome do parceiro. Para gerar apenas os 30 primeiros caracteres do nome do parceiro, podemos utilizar:

```auto
LEFT(Dados_Detalhe.NOME_PARCEIRO,30)
```

Para alcançar o mesmo resultado utilizando o COPY, pode ser utilizado:

```auto
COPY(Dados_Detalhe.NOME_PARCEIRO,1,30)
```

Observe que no Copy, é necessário apontar que seria gerado a partir do primeiro caractere e haveria a opção de gerar uma parte intermediária do texto. Perceba como o Left não apontou o caractere inicial; a geração se dá sempre a partir do primeiro caractere, respeitando o tamanho especificado.

[\[voltar ao subtítulo\]](#fun%C3%A7%C3%B5esempregadasnaedi%C3%A7%C3%A3odef%C3%B3rmulas)

---

## Funções Matemáticas

A função **"ABS"** tem o objetivo de retornar o módulo de um número, ou seja, seu valor absoluto, sem sinal. É utilizada quando na geração de um arquivo, o sinal para números negativos não foi gerado. Para utilizar a função:

```auto
ABS(<VARIÁVEL>)

INT / FRAC
```

As funções **"Int"** e **"Frac"** são utilizadas para extrair a parte inteira ou a parte fracionada de um número. Essas funções são empregadas normalmente na geração de arquivos de EDI, nos quais podem existir campos separados para a parte inteira e para os decimais de um valor. Sua utilização ocorre da seguinte forma:

```auto
INT(<VARIÁVEL>)

FRAC(<VARIÁVEL>)

ROUND / TRUNC
```

Referente às funções **"Round"** e **"Trunc"**, destacamos que são utilizadas para tratar as dízimas de valores, em cálculos ou na geração de arquivos de EDI. Observe a seguir, estrutura das funções:

```auto
ROUND(<VARIÁVEL>,<QTD_CASAS>)

TRUNC(<VARIÁVEL>,<QTD_CASAS>)
```

A estrutura para utilização das duas funções é semelhante. A diferença está no tratamento dado aos decimais; enquanto a função Round realiza o arredondamento, a função Trunc despreza as casas decimais que possam estar além da quantidade de casas informada como parâmetro. Como, por exemplo:

Suponhamos que determinada variável esteja retornando o valor "1,995". Se for utilizada a função Round, com duas casas decimais, o valor final será "2,00". Já com a função Trunc, o valor final seria "1,99".

[\[voltar ao subtítulo\]](#fun%C3%A7%C3%B5esempregadasnaedi%C3%A7%C3%A3odef%C3%B3rmulas)

---

## Funções de Datas

As funções **"Dia"**, **"Mes"** e **"Ano"** são utilizadas para retornar uma parte de uma data. Normalmente utilizadas na formatação de EDI, quando o layout possui campos separados para cada parte da data, ou para gerar no arquivo apenas dia e mês, ou mês e ano de uma determinada data. A sintaxe destas funções é simples, observe:

```auto
DIA(<VARIÁVEL_DATA>)

MES(<VARIÁVEL_DATA>)

ANO(<VARIÁVEL_DATA>)
```

Assim, no exemplo em que a variável _Dados\_Detalhe.DATA\_VENCIMENTO_ retorna a data de vencimento do título na configuração do EDI Bancário, no formato DDMMAAAA.

Se o layout de EDI solicita a informação do **"Mês"**, você pode utilizar MÊS, ao invés das funções _COPY/SUBTR_, dessa forma:

```auto
MES(Dados_Detalhe.DATA_VENCIMENTO)
```

Ao utilizar a função mês é importante utilizar a opção **"Inteiro com zeros a esquerda"** do [Tipo do Campo](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110273-Configura%C3%A7%C3%A3o-Arquivo-de-Remessa#abacampos), para que seja adicionado um 0 à esquerda nos meses de 1 a 9.

[\[voltar ao subtítulo\]](#fun%C3%A7%C3%B5esempregadasnaedi%C3%A7%C3%A3odef%C3%B3rmulas) [\[voltar ao topo\]](#top) [](#fun%C3%A7%C3%B5esempregadasnaedi%C3%A7%C3%A3odef%C3%B3rmulas)