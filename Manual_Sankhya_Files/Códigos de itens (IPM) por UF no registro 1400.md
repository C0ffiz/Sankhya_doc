# Códigos de itens (IPM) por UF no registro 1400

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116093-C%C3%B3digos-de-itens-IPM-por-UF-no-registro-1400](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116093-C%C3%B3digos-de-itens-IPM-por-UF-no-registro-1400)

---

# Códigos de itens (IPM) por UF no registro 1400

 **![Módulo 36x36 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42312578752151) Módulo:** Livros Fiscais > Avançado > Escrituração Fiscal Digital         

---

Diversas empresas, tem a obrigatoriedade de gerar no [EFD ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607614), o Registro 1400 - Informações sobre valores agregados; segundo o [Guia Prático EFD - ICMS/IPI - Versão 2.0.20](http://sped.rfb.gov.br/arquivo/show/1986), quando se trata do campo COD\_ITEM\_IPM\* (Campo 2 - Código do item) cada Unidade Federativa pode criar sua própria tabela onde listam quais códigos e operações devem ser apresentados no registro em questão.

\*Índice de Participação dos Municípios

Através das configurações realizadas por meio desta tela, será possível gerar o Registro 1400 do EFD ICMS/IPI conforme as especificações do Código do item e operações definidas por cada Estado.

<table style="border-collapse: collapse; width: 100%; height: 112px;" border="1"><tbody><tr style="height: 24px;"><td style="width: 100%; height: 24px;"><h4 id="h_01HYG0P7EK5B0NB4FR0RTE3JFE" class="wysiwyg-text-align-center"><strong>Funcionalidades da tela</strong></h4></td></tr><tr style="height: 22px;"><td style="width: 100%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;<a class="topiclink" href="#consideraesiniciais">Considerações iniciais</a>&nbsp; &nbsp;</span></td></tr><tr style="height: 22px;"><td style="width: 100%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;<a class="topiclink" href="#abageral">Aba Geral</a></span></td></tr><tr style="height: 22px;"><td style="width: 100%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;<a class="topiclink" href="#abasgrupodeprodutoprodutoetiposdeoperao">Abas Grupo de Produto, Produto e Tipos de Operação</a>&nbsp;</span></td></tr><tr><td style="width: 100%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;<a href="#F%C3%B3rmulaIPM">Fórmula IPM</a></span></td></tr><tr style="height: 22px;"><td style="width: 100%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;<a class="topiclink" href="#botoimportartabela">Botão Importar Tabela</a></span></td></tr></tbody></table>

![1400.png](https://ajuda.sankhya.com.br/hc/article_attachments/8493966390551)

### **Considerações iniciais**

O cadastro nesta tela, pode ser realizado de duas maneiras, inserção manual, ou por meio do botão ![Botão](/guide-media/01H3HF95F4QQ1GPWYH0JDKZX45)  localizado no alto da tela. Optando-se pela inclusão manual, preenche-se inicial e obrigatoriamente, o Código UF e Código Item, que se referem ao Estado ao qual os códigos de itens pertencem e o código de item para IPM, respectivamente.

![14002.png](https://ajuda.sankhya.com.br/hc/article_attachments/8493975682455)

Os demais preenchimentos serão explanados no decorrer desta documentação, assim como a alimentação da tela através do botão [Importar Tabela](#botoimportartabela).

[\[voltar ao topo\]](#top)

### **Aba Geral**

Nesta aba, são inseridas a Descrição do Código de Item para IPM, e as Datas Inicial e Final de vigência dos códigos. O preenchimento da Data Inicial de vigor dos códigos é obrigatório. A Data Final é opcional, porém quando inserida, o código em questão não será apresentado no arquivo depois que tal data for transposta, pois essa informação representa quando seu período de vigência será encerrado.

![14003.png](https://ajuda.sankhya.com.br/hc/article_attachments/8493976905111)

[\[voltar ao topo\]](#top)

### **Abas Grupo de Produto, Produto e Tipos de Operação**

Estas três abas possuem o mesmo propósito, que é de permitir a particularização dos critérios para uso dos códigos de itens; seguindo a nomenclatura de cada aba, pode-se definir [Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Produtos), [Grupos de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044598294-Grupos-de-Produtos-Servi%C3%A7os) ou [Tipos de Operação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP) específicos a serem utilizados com cada código de itens.

![14004.png](https://ajuda.sankhya.com.br/hc/article_attachments/8494031053719)

Para o registro 1400 será enviada a informação existente no campo Código Item (citado nas [Considerações iniciais](#consideraesiniciais)) para o **"Campo 2 - COD\_ITEM\_IPM"**. Estas informações serão vinculadas ao lançamento das notas no momento da geração do registro, de acordo com a seguinte ordenação/hierarquia:

Geral > Tipos de Operação > Grupo de Produto > Produto > Fórmula IPM

Ou seja, verifica-se primeiramente se existe algum Produto cadastrado, caso não tenha, será analisada a aba Grupo de Produtos, e em caso de insucesso, tem-se a busca pelos Tipos de Operação.

**Observação:** os parâmetros **"CFOPs que geram Não Dedutíveis no registro 1400 - CFOPNAODED1400"** e **"UFs que geram Não Dedutíveis no registro 1400 - UFSNAODED1400"** deverão estar configurados com as devidas UFs e CFOPs para que seja realizada a Geração do registro 1400.

É necessário que além da configuração dos parâmetros acima informados, esta tela também tenha seu devido registro para que o correto funcionamento do registro ocorra.

**Nota:** para que seja impresso no registro 1400 o **"Código do Item"**, deve-se realizar os cadastros das abas Grupo de Produto, Produto e Tipos de Operação desta tela.

[\[voltar ao topo\]](#top)

### **Fórmula IPM**

![versão FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42312578753559) **Esta aba estará disponível a partir da versão 4.33 do sistema.**

![Fórmula IPM.png](https://ajuda.sankhya.com.br/hc/article_attachments/24256959399447)

Nesta aba o sistema possibilitará a elaboração de uma fórmula para o preenchimento do registro 1400 da [EFD Fiscal ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/7267044122263-EFD-Fiscal-ICMS-IPI), exigindo do usuário a certificação da conformidade com a legislação estadual aplicável à empresa emissora.

Por meio do botão ![botão construtor.png](https://ajuda.sankhya.com.br/hc/article_attachments/24099504734231) **"Construtor"**, é possível criar fórmulas com vínculos nas tabelas: TGFCAB, TGFITE, TGFDIN e TGFLIV.

Os [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP) utilizadas na aba [Tipos de Operação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116093-C%C3%B3digos-de-itens-IPM-por-UF-no-registro-1400#abasgrupodeprodutoprodutoetiposdeoperao) desta tela, serão utilizadas para distinguir o **"Tipo de Movimento"** (Compra, Venda, Devoluções e Transferências).

![1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/24256972874647) Nesse contexto, o usuário deve possuir uma restrição por Grupo de Produto e/ou Produto;

![2 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/24256972892055) Se houver uma restrição por Grupo de Produto, o código IPM no registro 1400 será gerado apenas para os produtos pertencentes ao grupo cadastrado. Nesse caso, não é necessário que a aba Produto esteja preenchida.

Com as devidas configurações, na tela EFD - Fiscal ICMS/IPI. Ao inserir a referência de lançamento dos movimentos de entrada e clicar em ![processar FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/24257053230615)**"Processar"** e, em seguida, em ![botao-gerar-FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/24257053236503) **"Gerar"**, o arquivo TXT do registro 1400 incluirá o código criado.

Além disso, caso o campo Fórmula seja preenchido, o sistema Sankhya passará a desconsiderar os seguintes parâmetros:

*   **"CFOPs que geram Não Dedutíveis no registro 1400 - CFOPNAODED1400"**;
*   **"UFs com cd.IBGE parceiro fornecedor p/ reg.1400 - IBGEPARC1400"**;
*   **"UFs que geram NF-e de Venda no registro 1400 - UFSVENREG1400"**;
*   **"UFs que geram Não Dedutíveis no registro 14 - 00UFSNAODED1400"**;
*   **"UFs que geram CT-e Iniciados em Outro Estado no registro 1400 - UFSCTEOUTUF1400"**.

[\[voltar ao topo\]](#top)

### **Botão Importar Tabela**

Localizado na parte superior da tela, o botão ![importar.png](https://ajuda.sankhya.com.br/hc/article_attachments/8494246685335)  tem a função de carregar nesta própria rotina um arquivo previamente baixado do site do [SPED - Sistema Público de Escrituração Digital](http://sped.rfb.gov.br/) (seção [Sped Tabelas](http://www.sped.fazenda.gov.br/spedtabelas/AppConsulta/publico/aspx/ConsultaTabelasExternas.aspx?CodSistema=SpedFiscal)) no formato **".txt"**, que contenham os códigos e operações permitidos por cada estado, que devem ser apresentados no registro.

Uma vez de posse do arquivo correspondente a UF em questão, acionando-se o botão acim, será aberto o pop-up **"Informe os parâmetros"** que possibilita informar uma sigla de UF válida caso o arquivo não possua uma sigla:

![14005.png](https://ajuda.sankhya.com.br/hc/article_attachments/8494232263319)

Logo após, tem-se a exibição do pop-up para busca e escolha do documento.

Vejamos um exemplo de linha presente no arquivo:

SPDIPAM11|Compras escrituradas de mercadorias de produtores agropecuários paulistas por município de origem.|01012015|

**Observação:** ao realizar a importação de um arquivo, pode ser que os registros já existam no sistema, por esse motivo, através da marcação Manter Registros na Importação presente no botão Configuração da Tela (lado superior direito da tela), pode-se optar por preservar ou modificar os registros já importados, de modo a evitar-se algum tipo de duplicidade.

[\[voltar ao topo\]](#top)