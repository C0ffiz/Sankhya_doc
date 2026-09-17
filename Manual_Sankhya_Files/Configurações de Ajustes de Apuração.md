# Configurações de Ajustes de Apuração

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110593-Configura%C3%A7%C3%B5es-de-Ajustes-de-Apura%C3%A7%C3%A3o](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110593-Configura%C3%A7%C3%B5es-de-Ajustes-de-Apura%C3%A7%C3%A3o)

---

# Configurações de Ajustes de Apuração

![Módulo 36x36 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313047963799) **Módulo:** Livros Fiscais > Arquivos            

---

Esta tela tem como finalidade melhorar a forma de inserção dos ajustes de ICMS vinculados a itens de nota no Livro Fiscal. Assim, evita-se o retrabalho e tem-se uma redução nos erros ocasionados pelo lançamento de ajustes manuais.

Assim, neste artigo trataremos dos seguintes tópicos:

<table style="border-collapse: collapse; width: 100%; height: 102px;"><tbody><tr style="height: 22px;"><td style="width: 49.7619%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#configura%C3%A7%C3%B5esiniciais" target="_self" rel="undefined">Configurações Iniciais</a>&nbsp;</span></td><td style="width: 9.04764%; height: 22px;">&nbsp;</td><td style="width: 41.1904%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#abaAjustesdeDocumentosEFDFiscal">Aba Ajustes de Documentos...</a></span></td></tr><tr style="height: 22px;"><td style="width: 49.7619%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#abaajustesdeapuraoicmsicmsst">Aba Ajustes de Apuração ICMS/ICMS ST</a></span></td><td style="width: 9.04764%; height: 22px;">&nbsp;</td><td style="width: 41.1904%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#abafiltros">Aba Filtros</a></span></td></tr><tr style="height: 22px;"><td style="width: 49.7619%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#botovalidarfiltrosfrmulas">Botão Validar Filtros/Fórmulas</a></span></td><td style="width: 9.04764%; height: 22px;">&nbsp;</td><td style="width: 41.1904%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#executandoarotina">Executando a Rotina</a></span></td></tr><tr style="height: 36px;"><td style="width: 49.7619%; height: 36px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#apura%C3%A7%C3%A3oautom%C3%A1ticafecpriodejaneiro" target="_self" rel="undefined">Apuração automática FECP Rio de Janeiro</a></span></td><td style="width: 9.04764%; height: 36px;">&nbsp;</td><td style="width: 41.1904%; height: 36px;">&nbsp;</td></tr></tbody></table>

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/1500007622082)

## Configurações Iniciais

Quando a marcação **"Utiliza doc. relacionado de outra referência"** no Painel Principal, estiver selecionada temos que o sistema buscará os documentos que se apresentam fora do período de geração, mas que estão relacionados com documentos que se encontram no período de geração.

**Observação:** a marcação Utiliza doc. relacionado de outra referência poderá ser habilitada, apenas se o campo **"Tipo de Configuração"** estiver com a opção **"2 - Ajustes de Apuração de ICMS/ICMS ST"** selecionada.

 ![essencial FINAL (1).png](https://ajuda.sankhya.com.br/hc/article_attachments/16286523310103)Caso você insira duas Configurações de Ajuste de Apuração com o campo Tipo de Configuração igual a **"1 - Ajustes de Documento"** e com o mesmo número de nota e sequência, será exibida uma mensagem informando que já foi realizada uma Configuração com o Tipo 1.

O campo **"Origem do Ajuste"** determinará a origem dos ajustes de apuração a serem feitos dentre as opções **"Nota"** ou **"Financeiro"**.

*   A opção Nota, quando selecionada, terá o comportamento atual do sistema, sendo que, a busca dos documentos considerará, primeiramente, a data de negociação e a data de entrada/saída será observada apenas na inexistência dela.
*   Já a opção Financeiro, buscará os financeiros que correspondam aos filtros.

**Observação:** para o Financeiro, as fórmulas para cálculo dos valores, deverão conter apenas campos das tabelas TGFFIN e TGFTOP, definidas por FIN e TOP, respectivamente.

[\[voltar ao topo\]](#top)

## Aba Ajustes de Documentos - EFD Fiscal

  **![versão FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16286523311767)** Em versões anteriores a **4.17**, o nome desta aba é chamada **"Ajustes de Documentos (EFD C195/C197 - D195/D197)"**.

![](https://ajuda.sankhya.com.br/hc/article_attachments/13642249260823)

Informe aqui os dados que serão empregados na aba [EFD C195/C197/C595/C597 - D195/D197](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607874-Cadastro-Livro-ICMS-IPI#abaefdc195c197c595c597d195d197) do Cadastro Livro ICMS/IPI para a geração dos seguintes registros: 

*   **C195** - Complemento do Registro Analítico - Observações do Lançamento Fiscal (código 01, 1B, 04 e 55);
*   **C197** - Outras Obrigações Tributárias, Ajustes e Informações provenientes de Documento Fiscal;
*   **C855** - Observações do lançamento fiscal (Código 59);
*   **C857** - Outras obrigações tributárias, ajustes e informações de valores provenientes de documento fiscal;
*   **C895** - Observações do lançamento fiscal (Código 59);
*   **C897** - Outras obrigações tributárias, ajustes e informações de valores provenientes de documento fiscal;
*   **D195** - Observações do lançamento (CÓDIGO 07, 08, 8B, 09, 10, 11, 26, 27, 57 e 67);
*   **D197** - Outras obrigações tributárias, ajustes e informações de valores provenientes do documento fiscal.

Através do campo **"Observação"** vincule a observação previamente criada na tela [Observações para Notas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044596474-Observa%C3%A7%C3%B5es-para-Notas).

Informe no campo **"Código Ajuste"** o código de ajuste que será utilizado. Sendo que este, está localizado na lista de [códigos](http://www.sped.fazenda.gov.br/spedtabelas/AppConsulta/publico/aspx/ConsultaTabelasExternas.aspx?CodSistema=SpedFiscal) disponibilizados pela UF.

O campo **"Indicador de Sub-Apuração"** e a marcação **"Sub-Apuração"**, indicarão se o ajuste pertence ou não a uma sub-apuração e qual seu tipo.

Caso seja necessário inserir mais informações além da observação padrão, utilize o campo **"Compl. Obs. Padrão"**.

Os registros que possuírem a marcação **"Agrupar por Documento Fiscal"** habilitada, serão agrupados por documento fiscal na geração do registro C197, sendo que, será desconsiderado o código do produto no agrupamento.

No campo **"Fórmula Base de ICMS"** relacione a fórmula que resultará no valor a ser preenchido no campo **"Base do ICMS"** no ajuste.

Temos no campo **"Fórmula Alíquota de ICMS"**, a fórmula que trará como resultado o valor que irá preencher o campo **"Alíquota do ICMS"** no ajuste.

Vincule no campo **"Fórmula Valor ICMS****"** a fórmula que tem como resultado o valor que preencherá o campo **"Vlr. do ICMS"** no ajuste.

O campo **"Fórmula Valor Outros"** deverá ser preenchido com a fórmula que resultará no valor a ser preenchido no campo **"Vlr. de outros"** no ajuste.

**Observação:** os campos que permitem a inserção de fórmula desta aba, comportarão as seguintes tabelas:

*   TGFITTE;
*   TGFPRO;
*   TSIEMP;
*   TGFTOP;
*   TGFDIN - Tendo-se dados de ICMS;
*   TGFDIN - Quando se tratar de dados de ICMS ST;
*   TGFDIN - Tratando-se de dados de IPI;
*   TGFADST - Quando se tratar de [Apuração de Divergências de ICMS-ST](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044595094-Apura%C3%A7%C3%A3o-de-Diverg%C3%AAncias-de-ICMS-ST);
*   TGFIDST - Tratando-se de Apuração de Divergências de ICMS-ST.

![](https://ajuda.sankhya.com.br/hc/article_attachments/13642416568087)

[\[voltar ao topo\]](#top)

## Aba Ajustes de Apuração ICMS/ICMS ST

As informações inseridas nesta aba irão popular a tela [Ajuste da Apuração de ICMS e ICMS ST](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607654-Ajuste-da-Apura%C3%A7%C3%A3o-de-ICMS-e-ICMS-ST).

![](https://ajuda.sankhya.com.br/hc/article_attachments/13642375290007)

Informe no campo **"Tipo Ajuste"** os últimos 4 dígitos do código do ajuste.

O campo **"Código Ajuste"** tem a finalidade de atender a legislação do estado de Pernambuco (PE) em relação ao Sintegra e deve ser preenchido de acordo com as regras dos campos 05 e 06 do REGISTRO TIPO 88 - SUBTIPO 77 - DETALHE 00.

No campo **"Tipo Apuração"** aponte qual será a natureza deste ajuste. Este campo influenciará também na formação do código de ajuste, pois cada opção representa um caractere que será o quarto dígito do código do ajuste. Temos as seguintes opções:

*   0 - Outros débitos;
*   1 - Estorno de créditos;
*   2 - Outros créditos;
*   3 - Estorno de débitos;
*   4 - Deduções do imposto apurado;
*   5  - Débito especial.

Será definido no campo **"UF"** a Unidade da Federação do destinatário da NF-e a ser buscada. Quando não preenchido, todas as notas virão conforme os filtros relativos aos outros campos.

Caso o ajuste tenha origem em um processo, o número do mesmo deverá ser informado no campo **"Número Processo"**.

**Nota:** na geração dos registros do bloco E, bloco C, 1922 e 1926, este campo se comporta da seguinte maneira:

*   Arquivos gerados até o exercício 2022, o campo permite até 15 caracteres;
*   Arquivos gerados a partir do exercício 2023 poderão ter até 60 caracteres.

O campo **"Origem Processo"** será preenchido quando existir um processo relacionado ao ajuste. As opções são:

*   Sefaz;
*   Justiça Federal;
*   Justiça Estadual;
*   Outros.

Através do campo **"Observação Padrão"** temos o vínculo com a observação previamente criada na tela [Observações para Notas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044596474-Observa%C3%A7%C3%B5es-para-Notas).

Informe no campo **"Tipo Imposto"** o tipo de imposto que o ajuste está vinculado. São eles:

*   0 - ICMS;
*   1 - ICMS ST.

O campo **"Indicador de Sub-Apuração"** será preenchido quando o ajuste em questão fizer parte do Registro 1923 - EFD ICMS/IPI.

Será possível ainda gerar estornos de crédito nos itens 60 e 65, utilizando o campo **“Registro do Ajuste na DIME SC”** que possui as seguintes opções: 

*   Item 60 - Outros Estornos de Crédito;
*   Item 65 - Estorno de Crédito da Entrada em Decorrência da Utilização de Crédito Presumido.

Nesse caso, ao selecionar uma delas, o sistema somará os valores do campo **“Valor do Ajuste”** da aba [Ajuste](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607654-Ajuste-da-Apura%C3%A7%C3%A3o-de-ICMS-e-ICMS-ST#abaajuste) da tela [Ajuste da Apuração de ICMS e ICMS ST](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607654-Ajuste-da-Apura%C3%A7%C3%A3o-de-ICMS-e-ICMS-ST) e apresentar a soma no item 60 ou 65 do quadro 25 da DIME SC, assim quando gerar o arquivo txt, será apresentado uma linha para o registro 25 com o item 60 ou 65.

Para que a configuração do campo Indicador de Sub-Apuração seja validada, a opção **"Sub-Apuração"** deve estar marcada.

Em relação ao SPED Fiscal, são apresentados na quarta posição do campo COD\_AJ\_APUR com o valor 5 (no registro E111 e E220) e seu valor é totalizado no campo **"Débitos Especiais"** do registro E110 e no campo DEB\_ESP\_ST do registro E210.

A marcação **"Agrupar registros em um único ajuste?"** permite a geração de um único ajuste para várias notas ou de um ajuste para cada nota.

O campo **"Inserir Ajuste Por"** possibilita a geração de um único ajuste para a nota inteira ou o vínculo de um ajuste para cada item da nota. Existem três possibilidades de filtros: **"Item"**, **"Nota"** ou **"Referência"**.

Se optar por filtrar por Nota e for informado o campo **"Produto"** da aba [Filtros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110593-Configura%C3%A7%C3%B5es-de-Ajustes-de-Apura%C3%A7%C3%A3o#abafiltros), a função não terá utilidade, pois ele agrupará somente pelas notas. Caso queira filtrar por Produtos, selecione no campo Inserir Ajuste por a opção Item.

Se houver a necessidade de incluir mais informações além da Observação Padrão, o campo **"Observação"** poderá ser preenchido.

Caso o ajuste esteja vinculado há um processo, a descrição deste processo será inserida no campo **"Descrição do Processo"**.

No campo **"Fórmula Valor Ajuste"** será vinculada a fórmula que resultará no valor a ser preenchido no campo **"Valor do Ajuste"**.

**Observação:** os campos que permitem a inserção de fórmula desta aba, comportarão as seguintes tabelas e campos:

Quando o campo Inserir Ajuste por  estiver configurado com a opção **"Item"**:

*   TGFITTE;
*   TGFPRO;
*   TSIEMP;
*   TGFTOP;
*   TGFDIN - Tendo-se dados de ICMS;
*   TGFDIN - Quando se tratar de dados de ICMS ST;
*   TGFDIN - Tratando-se de dados de IPI.

![](https://ajuda.sankhya.com.br/hc/article_attachments/13642473977879)

Se estiver configurado com a opção **"Nota"**:

*   TGFCAB;
*   TSIEMP;
*   TGFTOP;
*   VLRSUBSTANT(campo);
*   BASESUBSTITANT(campo);
*   VLRICMSANT(campo);
*   BASESTANT(campo);
*   BASESTFCPINTANT(campo);
*   VLRSTFCPINTANT(campo).

![](https://ajuda.sankhya.com.br/hc/article_attachments/13642475471511)

[\[voltar ao topo\]](#top)

## Aba Filtros

Defina nesta aba, os filtros pertinentes a busca dos documentos que serão vinculados aos ajustes.

![mceclip5.png](https://ajuda.sankhya.com.br/hc/article_attachments/1500007795401)

Caso as variáveis pré-estabelecidas não atendam as necessidades, é possível criar um filtro personalizado. Nesse filtro, você pode fazer uma consulta via comandos SQL para especificar melhor quais documentos devem ser vinculados ao ajuste.

 ![acesse também FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16256013735575) Para conhecer os detalhes das opções do campo Tributação, acesse o artigo Alíquotas de ICMS, aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044602934-Al%C3%ADquotas-de-ICMS#tributa%C3%A7%C3%A3o).

[\[voltar ao topo\]](#top)

## Botão Validar Filtros/Fórmulas

Este botão está localizado na parte superior da tela e tem como funcionalidade validar os filtros avançados e fórmulas criadas para que se tenha certeza de que tudo está estruturalmente de acordo com as regras aceitas pela rotina. Ao acioná-lo, tem-se a exibição de um pop-up de mesma nomenclatura:

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/1500007626002)

Informe a **"Empresa"** e o **"Período"** pelo qual se deseja efetuar a validação.

Sendo que, se a validação não for realizada o campo **"Status"** ficará como **"Pendente"** e a regra não será executada no momento da geração do livro.

[\[voltar ao topo\]](#top)

## Executando a Rotina

Para que o ajuste seja efetuado, é necessário realizar a geração do livro através da tela [Geração ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045115953-Gera%C3%A7%C3%A3o-ICMS-IPI). Após a execução da rotina, basta verificar se as informações foram populadas nas telas [Cadastro Livro ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607874-Cadastro-Livro-ICMS-IPI) (aba [EFD C195/C197/C595/C597 - D195/D197](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607874-Cadastro-Livro-ICMS-IPI#abaefdc195c197c595c597d195d197)) e [Ajuste da Apuração de ICMS e ICMS ST](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607654-Ajuste-da-Apura%C3%A7%C3%A3o-de-ICMS-e-ICMS-ST).

**Nota:** quando se tratar de Notas de Transferência, configure os ajustes abaixo para que as informações relacionadas à transferência sejam apresentadas nos registros C195/C197 e D195/D197 do SPED Fiscal:

**1.** Realize nesta tela, o ajuste de saída por transferência da Empresa que está emitindo a nota fiscal, e logo após, o ajuste de entrada para a Empresa que estará recebendo a nota fiscal de transferência.

**2.** Na tela [Geração ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045115953), efetue a geração do Livro Fiscal de Saída para a Empresa que está emitindo a nota de saída por transferência, e somente depois, realize a geração do Livro Fiscal de Entrada para a Empresa que receberá esta nota.

[\[voltar ao topo\]](#top)

## Apuração automática FECP Rio de Janeiro

No Estado do Rio de Janeiro, conforme prevê a Resolução SEFAZ nº 987/2016, a apuração do FECP é realizada tomando como referência a base de cálculo do ICMS e do ICMS ST. 

A seguir, trataremos das configurações que devem ser realizadas para efetuar um ajuste de apuração através da referência.

Primeiramente, no Painel Principal, selecione no campo **"Tipo de Configuração"** a opção **"Ajustes de Apuração de ICMS/ICMS ST"** e depois indique no campo **"Origem do Ajuste"** a opção **"Nota"**;

Em seguida, na aba [Ajustes de Apuração ICMS/ICMS ST](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110593-Configura%C3%A7%C3%B5es-de-Ajustes-de-Apura%C3%A7%C3%A3o#abaajustesdeapuraoicmsicmsst), realize as configurações abaixo:

*   No campo **"Tipo apuração"**  indique a opção **"Deduções do imposto apurado"**;
*   Informe no campo **"Tipo imposto"** a opção **"ICMS"**;
*   Efetue a marcação **"Agrupar registros em um único ajuste?"**;
*   Selecione no campo **"Inserir Ajuste por"** a opção **"Referência"**;
*   Por fim, informe a "**Fórmula Valor Ajuste"** conforme abaixo:  
    _CASE WHEN ((CASE WHEN ITE.CODCFO >=5000 AND ITE.CODCFO<6000 THEN ICMS.BASERED ELSE 0 END) -_  
    _(CASE WHEN ITE.CODCFO >=1000 AND ITE.CODCFO<2000 THEN ICMS.BASERED ELSE 0 END)) <> 0 THEN_  
    _((CASE WHEN ITE.CODCFO >=5000 AND ITE.CODCFO<6000 THEN ICMS.BASERED ELSE 0 END) -_  
    _(CASE WHEN ITE.CODCFO >=1000 AND ITE.CODCFO<2000 THEN ICMS.BASERED ELSE 0 END)) \* 0.02 ELSE 0 END_

Após criar o registro, valide a fórmula através do botão Valida Filtros/Fórmulas para que o campo **"Status"** seja alterado de **"Pendente"** para **"Liberado"**.

**Observação:** caso o campo Inserir Ajuste por esteja com a opção Referência selecionada, os campos abaixo não poderão ser utilizados em conjunto:

*   O campo Origem do Ajuste igual à **"Financeiro"**;
*   A marcação **"Utiliza doc. relacionado de outra referência"** efetuada.

Caso sejam utilizados em conjuntos, serão exibidas as seguintes mensagens:

**_"Inserir Ajuste Por 'Referência' não pode ser marcado em conjunto com a origem igual a 'Financeiro'"._**  
**_"Inserir Ajuste Por 'Referência' não pode ser marcado em conjunto 'Utiliza doc. relacionado de outra referência:' igual a 'Sim'"._**

Após a validação da configuração acima, realize a [Geração ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045115953-Gera%C3%A7%C3%A3o-ICMS-IPI) e verifique na tela [Ajuste da Apuração de ICMS e ICMS ST](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607654-Ajuste-da-Apura%C3%A7%C3%A3o-de-ICMS-e-ICMS-ST), a geração do ajuste.

[\[voltar ao topo\]](#top)