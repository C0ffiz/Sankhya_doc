# Saiba como gerar o registro 1980 no EFD ICMS/IPI

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/12267173392919-Saiba-como-gerar-o-registro-1980-no-EFD-ICMS-IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/12267173392919-Saiba-como-gerar-o-registro-1980-no-EFD-ICMS-IPI)

---

# Saiba como gerar o registro 1980 no EFD ICMS/IPI

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><span style="font-weight: 400;"><strong><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42312550936855" alt="versão FINAL.png"> </strong></span><span style="font-weight: 400;">Esta funcionalidade está disponível <strong>somente em HTML5</strong><br>e a partir da <strong>versão 4.18</strong>.</span></pre></td></tr></tbody></table>

Conheça nesse artigo como gerar o Registro 1980 - GIAF 3 - Guia de informação e apuração de incentivos fiscais e financeiros: central de distribuição (entradas/saídas).

#### **Configurações iniciais**

Primeiramente, acesse a tela [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893), aba [Livros Fiscais](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abalivrosfiscais) e acione a marcação **"Beneficiário de Incentivo PRODEPE/FUNCRESCE?"**.

![Aba\_Livros\_Fiscais\_Marca\_\_o\_\_Benefici\_rio\_de\_Incentivo\_PRODEPE\_FUNCRESCE\_acionada.png](https://ajuda.sankhya.com.br/hc/article_attachments/12267171528215)

Ainda nessa tela, na aba [EFD-Escrituração Fiscal Digital](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaefdescrituraofiscaldigital), sub-aba **"Blocos e Registros"**, os registros abaixo devem estar com a marcação **"Gerar Registro"** acionada:

*   Registro 1001 -  Abertura do Bloco 1;
*   Registro 1980 - GIAF 3 - Guia de informação e apuração de incentivos fiscais e financeiros: central de distribuição (entradas/saídas);
*   Registro 1990 - Encerramento do Bloco 1.

![aba\_EFD-Escritura\_\_o\_Fiscal\_Digital\_\_2\_.png](https://ajuda.sankhya.com.br/hc/article_attachments/12271185225495)

Agora, na tela [CFOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044600714), selecione o CFOP utilizado e no campo **"Tipo de Operação PRODEPE"** informe se possui incentivo ou não.

![Tela\_CFOP\_aba\_Geral.png](https://ajuda.sankhya.com.br/hc/article_attachments/12267271229591)

Feito isso, acesse a tela de [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113), aba [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113#abaimpostos), seção **"Prodepe"** e informe a opção **"Com incentivo"** no campo **"Cód. Apur. Inc. PRODEPE/FUNCRESCE?"**. Configure também o campo **"Indicador Esp. Inc. PRODEPE/FUNCRESCE"** com a opção **"Com incentivo"** ou **"Sem incentivo"**.

![Cadastros\_de\_Produtos\_campo\_Indicador\_Esp.\_Inc.\_PRODEPE\_FUNCRESCE\_com\_a\_op\_\_o\_Com\_incentivo.png](https://ajuda.sankhya.com.br/hc/article_attachments/12267351937815)

Em seguida, acesse a tela [Cadastro Incentivos Fiscais/Financeiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360052979134) e configure o campo **"Indicador de Enquadramento"** com a opção **"4-Central de distribuição (entradas/saídas)"**. Preencha também o campo **"****Índice de recolhimento da central de distribuição"**, com o índice de recolhimento estabelecido pelo respectivo decreto concessivo.

![Tela\_Cadastro\_Incentivos\_Fiscais\_Financeiros\_2.png](https://ajuda.sankhya.com.br/hc/article_attachments/12271891218071)

Na aba **"Produtos"**, informe o **"Produto"** cadastrado anteriormente na tela Cadastro de Produtos.

#### **Geração do Registro 1980**

Realizadas as configurações acima, acesse a tela [EFD - Fiscal ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/7267044122263-EFD-Fiscal-ICMS-IPI-) e informe no **"Painel Principal"** a **"Empresa"** e a **"Data Referência"**.

Em seguida, preencha na aba [Configurações](https://ajuda.sankhya.com.br/hc/pt-br/articles/7267044122263-EFD-Fiscal-ICMS-IPI-#abaconfigura%C3%A7%C3%B5es), o **"Período"** da geração do relatório, selecione a **"UF"** a ser considerada para a geração do arquivo e, por fim, defina a **"Finalidade de Apresentação do Arquivo"**.

![EFD\_-\_Fiscal\_ICMSIPI\_2.png](https://ajuda.sankhya.com.br/hc/article_attachments/12272915832215)

Agora, clique em **"Processar"** para que o sistema realize a geração e preenchimento da aba **"1001"** e sub-aba **"1980"** referentes aos registros do arquivo de Escrituração, conforme as condições estabelecidas nas configurações.

![EFD\_-\_Fiscal\_ICMSIPI\_3.png](https://ajuda.sankhya.com.br/hc/article_attachments/12289732785175)

Caso os registros sejam gerados com sucesso, será apresentado no pop-up a mensagem:

_**"Registros processados com sucesso!"**_

Para gerar o aquivo TXT para o Registro 1980, basta clicar no botão **"Gerar"**. Veja abaixo um exemplo do arquivo: 

|1001|0|  
  
|1010|N|N|N|N|N|N|N|N|N|N|N|S|N|  
  
|**1980**|02|3,00|600,00|4000,00|2,00|1800,00|6000,00|676,00|120,00|120,00|240,00|436,00|40,00|  
  
|1990|4|