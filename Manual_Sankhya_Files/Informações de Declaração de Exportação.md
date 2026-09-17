# Informações de Declaração de Exportação

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116413-Informa%C3%A7%C3%B5es-de-Declara%C3%A7%C3%A3o-de-Exporta%C3%A7%C3%A3o](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116413-Informa%C3%A7%C3%B5es-de-Declara%C3%A7%C3%A3o-de-Exporta%C3%A7%C3%A3o)

---

# Informações de Declaração de Exportação

![Módulo 36x36 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313089595799) **Módulo:** Livros Fiscais > Avançado

---

Quando uma empresa efetua vendas para fora do país, torna-se necessário emitir documentos de cunho fundamental para que a exportação ocorra. Um desses documentos é a Declaração de Exportação - DE que engloba o Registro de Exportação - RE, sendo esse o conjunto de informações de natureza comercial, financeira, cambial e fiscal, que caracteriza a operação de exportação de uma mercadoria. Esses documentos são utilizados pela Receita Federal pois dão início ao despacho aduaneiro e também apoiam na geração de obrigações fiscais, como o [EFD - Escrituração Fiscal Digital - ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607614) onde gera-se os registros 1100 e 1105 do arquivo e o [Sintegra](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607534) sendo gerados os registros 85 e 86.

Deste modo, esta tela possibilitará o preenchimento dos referidos documentos.

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td style="width: 43.1904%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#painelprincipal">Painel Principal</a>&nbsp;</span></td><td style="width: 13.3333%;">&nbsp;</td><td style="width: 43.4762%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#abainformaesderegistroexportao">Aba Informações de Registro Exportação</a></span></td></tr><tr><td style="width: 43.1904%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#abainformaesdenotaexportao">Aba Informações de Nota Exportação</a></span></td><td style="width: 13.3333%;">&nbsp;</td><td style="width: 43.4762%;">&nbsp;</td></tr></tbody></table>

## Painel Principal

Localizado no alto da tela, o Painel Principal reúne as informações pertinentes a Declaração de Exportação.

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4638406960023)

O campo **"Nro Declaração"** comportará a numeração responsável por identificar a declaração que foi realizada.

A categoria desta declaração será descrita através do campo **"Tipo Declaração"**, que contém as seguintes opções:

*   Declaração Única de Exportação;
*   Declaração Simplificada;
*   Declaração de Exportação.

**Observação:** quando o campo Tipo Declaração estiver com a opção Declaração de Exportação selecionada, o campo **"Nro Registro"** (aba **"Informações de Registro Exportação"**) deverá ter um valor diferente de zero.

**Nota:** se a opção Declaração Única de Exportação (DU-E) estiver selecionada no campo Tipo de Declaração, será necessário que você preencha o campo **"Natureza"** da sub-aba Informações de Nota Exportação, caso contrário, será exibida a seguinte mensagem:

_**"Não foi possível atualizar o registro!**_  
_**É necessário informar o campo NATUREZA da nota para declaração D10, pois possui tipo de declaração única".**_

Por meio do campo **"Data Declaração"**, informe o período ao qual a declaração foi composta.

O período em que ocorreu a concretização da operação, será apontado no campo **"Data Averbação"**.

Informe também a **"Natureza"** da declaração, de acordo com as seguintes opções:

*   Direta;
*   Indireta;
*   Não - antes de 01/07/2005;
*   Sim - antes de 01/07/2005.

O campo **"Código do País de Destino"**, permitirá informar qual será o país destinatário da exportação.

[\[voltar ao topo\]](#top)

## Aba Informações de Registro Exportação

Esta aba compreenderá os dados que dizem respeito ao Registro de Exportação. Informe o número do registro e o período em que o mesmo foi realizado.

Por padrão, o sistema irá inserir o número 0 (zero) no campo **"Nro Registro"**. Assim, utilize um valor diferente apenas se a opção **"Declaração de Exportação"** do campo **"Tipo Declaração"** estiver selecionada. Caso as informações estejam incompatíveis, será apresentado a mensagem abaixo:

**_"Se o campo Tipo Declaração for igual a Declaração de Exportação, o Nro Registro deve ser informado e ser diferente de 0"._**

[\[voltar ao topo\]](#top)

## Aba Informações de Nota Exportação

Nesta aba serão apontados os documentos que irão compor o Registro de Exportação.

O campo **"Nro Único Nota"** é responsável pelo preenchimento e busca dos respectivos documentos, quando acionado, será exibido o pop-up **"Filtro por Notas"** que permite refinar a busca, tornando-a mais simples e rápida. Ressaltando, que os documentos a serem pesquisados pertencem à modalidade de venda.

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4638402978455)

Ao informar os dados necessários para a pesquisa, é possível realizar a seleção de um ou vários documentos a serem inseridos no Registro de Exportação.

**Observação:** ao informar uma nota cujos itens possuam CFOP's diferentes, será apresentada a mensagem abaixo:

**_"O documento vinculado possui mais de um CFOP e não foi possível determinar qual a natureza da exportação será adotada"._**

Se a nota informada possuir em seus itens todos os CFOP's iguais, porém este CFOP não seja o 7501, será apresentado o valor do campo **"CFOP"** no campo calculado de igual nome e será sugerido à você no campo **"Natureza"**, a opção **"Direta"**.

Caso a nota informada possua em seus itens todos os CFOP's iguais e este seja igual a 7501, será apresentado o valor do campo CFOP no campo calculado de nome igual, e sugerido a você o campo Natureza com a opção **"Indireta"** selecionada.

Assim, ao gerar o arquivo sped fiscal, o registro 1100 será gerado para cada nota e terá a informação Natureza (campo 5), conforme foi informado na aba Informações de Nota Exportação. Se o campo Natureza desta aba não for preenchido, será considerado o campo Natureza do Cabeçalho da tela.

Ao final, teremos a indicação da data, número e do tipo de conhecimento para cada documento selecionado.

**Observação:** quando o parâmetro **"Validar dt. conhecimento de declaração Exportação? - VALDTDECDTCTEXP"** estiver desligado, o sistema permitirá que você informe a Data do Conhecimento maior do que a Data de Declaração.

**Nota:** a Data do Conhecimento poderá ser maior que a Data de Declaração, desde não ultrapasse o último dia de referência desta última. Por exemplo: se a Data de Declaração for igual à 21/09/2021, a Data do Conhecimento não pode ser superior à 30/09/2021.

Na sub-aba **"Exportação Direta/Indireta"**, você poderá consultar os registros referentes à **"Natureza"** e o **"CFOP"**, dado que, estes estarão associados à nota cadastrada. 

[\[voltar ao topo\]](#top)