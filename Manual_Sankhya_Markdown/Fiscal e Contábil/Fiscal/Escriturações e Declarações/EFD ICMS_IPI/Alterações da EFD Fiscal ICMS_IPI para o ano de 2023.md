# Alterações da EFD Fiscal ICMS/IPI para o ano de 2023

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/11126560355991-Altera%C3%A7%C3%B5es-da-EFD-Fiscal-ICMS-IPI-para-o-ano-de-2023](https://ajuda.sankhya.com.br/hc/pt-br/articles/11126560355991-Altera%C3%A7%C3%B5es-da-EFD-Fiscal-ICMS-IPI-para-o-ano-de-2023)

---

# Alterações da EFD Fiscal ICMS/IPI para o ano de 2023

O layout do arquivo digital da [EFD Fiscal ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/7267044122263-EFD-Fiscal-ICMS-IPI) foi atualizado para o ano de 2023, assim, é necessário que o **Sankhya Om** esteja com as versões **4.15**, **4.16** ou superiores e/ou com o MGE - Livros Fiscais e Jiva - Livros Fiscais para as versões **4.46** ou superiores que contemplem as alterações de layout e atendam as versões **3.0.9** e **3.0.10** do [Guia Prático do EFD ICMS/IPI](http://sped.rfb.gov.br/pasta/show/1573).

Dessa forma, realize as seguintes configurações:

*   Na tela [EFD - Escrituração Fiscal Digital - ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607614-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI) a opção **"017 - Versão 116 - Início 01/01/2023"** do campo **"Versão do Layout do Arquivo"** estará configurada;
*   Em seguida, verifique se o preenchimento do campo **"Indicador de Layout (Registro K010)"** da aba [EFD - Escrituração Fiscal Digital](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaefdescrituraofiscaldigital) das [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa) está conforme o registro da empresa.

**Observações:**

A geração de documentos foram suspensas nas seguintes situações:

*   04 - NF-e, NFC-e ou CT-e - denegado;
*   05 - NF-e, NFC-e ou CT-e - Numeração inutilizada para os registro C100/C800/D100.

O tamanho de determinados campos foram alterados de 15 para 60 caracteres, sendo esses:

*   Campo 02 (NUM\_PROC) do registro C111;
*   Campo 03 (NUM\_PROC) dos registros E112, E230, E312 e 1922;
*   Campo 06 (NUM\_PROC) dos E116, E250, E316 e 1926.

**Nota:** no MGE - Livros Fiscais e Jiva - Livros Fiscais, a atualização da nova versão do layout se restringiu aos registros já atendidos de forma nativa, de forma que, os novos registros disponibilizados na versão 3.0.10 não foram implementados.

[\[Voltar ao topo\]](#top)