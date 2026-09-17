# Saiba como gerar o registro 1970 no EFD ICMS/IPI

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/12262170274711-Saiba-como-gerar-o-registro-1970-no-EFD-ICMS-IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/12262170274711-Saiba-como-gerar-o-registro-1970-no-EFD-ICMS-IPI)

---

# Saiba como gerar o registro 1970 no EFD ICMS/IPI

<table class=" wysiwyg-text-align-center" style="width: 98.8772%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42312504365847" alt="versão FINAL.png"> Esta funcionalidade está disponível <strong>somente em HTML5</strong> <br>e a partir da <strong>versão 4.18</strong>.</pre></td></tr></tbody></table>

Conheça nesse artigo como gerar o Registro 1970 - GIAF 3 - Guia de informação e apuração de incentivos fiscais e financeiros: importação (diferimento na entrada e crédito presumido na saída subsequente).

#### **Configurações iniciais**

Primeiramente, acesse a tela [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893), aba [Livros Fiscais](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abalivrosfiscais) e acione a marcação **"Beneficiário de Incentivo PRODEPE/FUNCRESCE?"**.

![Aba\_Livros\_Fiscais\_Marca\_\_o\_\_Benefici\_rio\_de\_Incentivo\_PRODEPE\_FUNCRESCE\_acionada.png](https://ajuda.sankhya.com.br/hc/article_attachments/12264686650519)

Ainda nessa tela, na aba [EFD-Escrituração Fiscal Digital](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaefdescrituraofiscaldigital), sub-aba **"Blocos e Registros"**, os registros abaixo devem estar com a marcação **"Gerar Registro"** acionada:

*   Registro 1001 - Abertura do Bloco 1;
*   Registro 1970 - GIAF 3 - Guia de informação e apuração de incentivos fiscais e financeiros: importação (diferimento na entrada e crédito presumido na saída subsequente);
*   Registro 1975 - GIAF 3 - Guia de informação e apuração de incentivos fiscais e financeiros: importação (saídas internas por faixa de alíquota);
*   Registro 1990 - Encerramento do Bloco 1.

![aba\_EFD-Escritura\_\_o\_Fiscal\_Digital.png](https://ajuda.sankhya.com.br/hc/article_attachments/12264686686231)

**Observação:** o registro 1975 é obrigatório sempre que houver um registro 1970. 

Agora, na tela [CFOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044600714), selecione o CFOP utilizado e no campo **"Tipo de Operação PRODEPE"** informe se possui incentivo ou não.

![Tela\_CFOP\_aba\_Geral.png](https://ajuda.sankhya.com.br/hc/article_attachments/12264709485335)

Feito isso, acesse a tela de [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113), aba [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113#abaimpostos), seção **"Prodepe"** e informe a opção **"Com incentivo"** no campo **"Cód. Apur. Inc. PRODEPE/FUNCRESCE?"**. Configure também o campo **"Indicador Esp. Inc. PRODEPE/FUNCRESCE"** com a opção **"Com incentivo"** ou **"Sem incentivo"**.

![Cadastros\_de\_Produtos\_campo\_Indicador\_Esp.\_Inc.\_PRODEPE\_FUNCRESCE\_com\_a\_op\_\_o\_Com\_incentivo.png](https://ajuda.sankhya.com.br/hc/article_attachments/12265114184087)

Em seguida, acesse a tela [Cadastro Incentivos Fiscais/Financeiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360052979134) e configure o campo **"Indicador de Enquadramento"** com a opção **"3-Importação (diferimento/crédito presumido)"**. Já no campo **"C****usto para Importações-base"**, selecione o tipo de custo que será utilizado para a composição do registro 1975.

![Tela\_Cadastro\_Incentivos\_Fiscais\_Financeiros.png](https://ajuda.sankhya.com.br/hc/article_attachments/12265598536727)

Na aba **"Produtos"**, informe o **"Produto"** cadastrado anteriormente na tela Cadastro de Produtos e indique o percentual de alíquota incidente sobre importações-base para a composição do registro 1975, no campo **"Alíquota incidente s/ Importações-base"**.  

![aba\_Produtos.png](https://ajuda.sankhya.com.br/hc/article_attachments/12265849762071)

#### **Geração do Registro 1970**

Realizadas as configurações acima, acesse a tela [EFD - Fiscal ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/7267044122263-EFD-Fiscal-ICMS-IPI-) e informe no **"Painel Principal"** a **"Empresa"** e a **"Data Referência"**.

Em seguida, preencha na aba [Configurações](https://ajuda.sankhya.com.br/hc/pt-br/articles/7267044122263-EFD-Fiscal-ICMS-IPI-#abaconfigura%C3%A7%C3%B5es), o **"Período"** da geração do relatório, selecione a **"UF"** a ser considerada para a geração do arquivo e, por fim, defina a **"Finalidade de Apresentação do Arquivo"**.

![Imagens\_ksnip\_7\_.png](https://ajuda.sankhya.com.br/hc/article_attachments/12289683489303)

Agora, clique em **"Processar"** para que o sistema realize a geração e preenchimento da aba **"1001"** e sub-abas **"1970"** e **"1975"** referentes aos registros do arquivo de Escrituração, conforme as condições estabelecidas nas configurações.

![EFD\_-\_Fiscal\_ICMSIPI.png](https://ajuda.sankhya.com.br/hc/article_attachments/12266014634007)

Casos os registros sejam gerados com sucesso, será apresentado no pop-up a mensagem:

_**"Registros processados com sucesso!"**_

Para gerar o aquivo TXT para o Registro 1970, basta clicar no botão **"Gerar"**. Veja abaixo um exemplo do arquivo: 

|1001|0|  
  
|1010|N|N|N|N|N|N|N|N|N|N|S|N|N|  
  
|**1970**|02|3050,50|468,50|1300,00|90,00|1300,00|156,00|140,40|161,83|374,50|212,67|  
  
|1975|3,50|1000,00|206,67|7,23|  
  
|1975|6,00|800,00|50,00|3,00|  
  
|1975|8,00|500,00|140,00|11,20|  
  
|1975|10,00|0,00|0,00|0,00|  
  
|1990|9|  
  
|9001|0|