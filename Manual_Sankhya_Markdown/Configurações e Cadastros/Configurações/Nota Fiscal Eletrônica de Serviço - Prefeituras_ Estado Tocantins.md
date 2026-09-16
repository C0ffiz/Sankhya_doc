# Nota Fiscal Eletrônica de Serviço - Prefeituras: Estado Tocantins

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/22602141163031-Nota-Fiscal-Eletr%C3%B4nica-de-Servi%C3%A7o-Prefeituras-Estado-Tocantins](https://ajuda.sankhya.com.br/hc/pt-br/articles/22602141163031-Nota-Fiscal-Eletr%C3%B4nica-de-Servi%C3%A7o-Prefeituras-Estado-Tocantins)

---

# Nota Fiscal Eletrônica de Serviço - Prefeituras: Estado Tocantins

Nesse artigo serão apresentadas as especificações de emissão de NFS-e das cidades localizadas no estado do Tocantins, para conhecê-las acesse os links abaixo:

<table class="wysiwyg-table-resized" style="margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 50%;"> <col style="width: 50%;"></colgroup><tbody><tr><td colspan="2"><p class="wysiwyg-text-align-center"><strong>Cidades</strong></p></td></tr><tr><td><a href="#araguanato">Araguaína/TO</a></td><td><a href="#palmasto">Palmas/TO</a></td></tr><tr><td><a href="#h_01H98JRWHQ4BCGBTVPNKC4B0ME">Araguatins/TO</a></td><td><a href="#parasodotocantinsto">Paraíso do Tocantins/TO</a></td></tr><tr><td><a href="#h_01KYHY4FF28YQABR033CVMEHR5">Bernardo Sayão/TO</a></td><td><a href="#tocantinsto">Tocantins/TO</a></td></tr></tbody></table>

### **Araguaína/TO**

A emissão de NFS-e pode ser realizada via API com serviço síncrono para o município de Araguaína. Para isso, basta configurar o parâmetro **"Utilizar emissão NFS-e WEB ISS Aguaraina pelo Broker? - NFSEISSARABROKE"** com o código IBGE de Araguaína **{disponível na versão ≥ 4.25b148 e 4.26b52}**. Com ele desconfigurado, a emissão será realizada via nativo (Sankhya) com serviço assíncrono.

Os seguintes cadastros estão envolvidos:

![1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22602097596311) Na tela [Cidades](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913), na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral), informe o **"Mun. domicílio fiscal"** de Araguaína, sendo este 1702109 e o **"Cód. município SIAFI"** 9241

![2 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22602141156375) Nos [**Tipos de Operação - TOP**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#top)**, acesse a aba**[**NFS-e**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abanfse) e configure no campo **"Cód. Natureza Oper. ISS (NFS-e)"** a natureza a ser utilizada na operação dentre as opções permitidas:

 
|  |  |
| --- | --- |
| **Código** | **Descrição** |
| 1 | Exigível |
| 2 | Não incidência |
| 3 | Isenção |
| 4 | Exportação |
| 5 | Imunidade |
| 6 | Exigibilidade suspensa por decisão judicial |
| 7 | Exigibilidade suspensa por procedimento administrativo |

![3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22602141159575) Acesse as [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa), aba [Documentos Fiscais Eletrônicos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaDocumentosFiscaisEletr%C3%B4nicos), sub-aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaNFS-e) > [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaGeralSub-abaNFS-e) e defina no campo **"Regime esp. tributação ISS (NFS-e)"** o regime especial de tributação ISS a ser utilizado pela empresa conforme as opções admitidas:

<table class="wysiwyg-table-resized" style="margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 21%;"> <col style="width: 79%;"></colgroup><tbody><tr><td><strong>Código</strong></td><td><strong>Descrição</strong></td></tr><tr><td>1</td><td>Microempresa municipal</td></tr><tr><td>2</td><td>Estimativa</td></tr><tr><td>3</td><td>Sociedade de profissionais</td></tr><tr><td>4</td><td>Cooperativa</td></tr><tr><td>5</td><td>Microempresário Individual (MEI)</td></tr><tr><td>6</td><td>Microempresário e Empresa de Pequeno Porte (ME EPP)</td></tr></tbody></table>

\*\*Nota:\*\*esta prefeitura permitirá a [Substituição de NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360046972414-Funcionalidades-relacionadas-%C3%A0-NFS-e#substituiodenfs-e) via webservice.

**Observação:** a cidade não suporta o cancelamento de nota de serviço via webservice.

[\[voltar ao topo\]](#top)

### **Araguatins/TO**

O município de Araguatins/TO utiliza um **Sistema Próprio Municipal** para as Notas Fiscais de Serviço (NFS-e), e a emissão foi homologada de forma automatizada por meio da integração via webservice.

Esta homologação já contempla a adequação aos novos impostos da Reforma Tributária (IBS e CBS). Para garantir que suas notas sejam emitidas e aprovadas sem erros, siga o passo a passo de configuração abaixo:

*   **Cadastros Básicos**
    *   [**Cidades**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades)**:** na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral), preencha o **"Mun. domicílio fiscal"** com o código IBGE **1702208**.
    *   [**Empresa**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa)**:** confirme se a **"Inscrição Municipal"** da sua empresa está devidamente preenchida.
*   **Configurações do Serviço:** acesse o cadastro de [Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o) (abas [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaimpostos) e [Alíquotas de ISS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaalquotasdeiss)) e revise:
    *   **Código de Serviço Municipal:** preencha o campo **"Cód. Trib. Município"** com a formatação exigida pela prefeitura. Exemplo: **140101**.
    *   **Preenchimento obrigatório:** não esqueça de informar o **"Item da Lista de Serviços (LC 116)"** (ex: 1401), o **"Código CNAE"** (ex: 4520001) e o **"Código NBS"** (ex: 120024000, conforme a tabela oficial da Nomenclatura Brasileira de Serviços).
*   **Configuração para IBS e CBS (Reforma Tributária)** Para que os novos impostos sejam calculados e enviados corretamente ao portal da prefeitura:
    *   **Cadastro de** [Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o)**:** na [aba Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abaimpostos), [seção Reforma Tributária](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#01K56TN2K88BREGGCND4D6DBNF), preencha o campo **"Código Classificação Tributária Nacional"** (ex: 140101). Configure também as alíquotas de IBS e CBS pertinentes ao serviço.
    *   [**Tipos de Operação (TOP)**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP)**:** na [aba Reforma Tributária](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#01K56TN2K88BREGGCND4D6DBNF) da TOP, certifique-se de ativar as marcações **"Tem CBS"** e **"Tem IBS"**.
*   **Regras de Emissão e Particularidades**
    *   **Tomador do Exterior:** o sistema permite a emissão para clientes do exterior normalmente (mediante preenchimento correto do endereço do tomador).
    *   **Múltiplos Itens e E-mails:** para incluir vários serviços na mesma nota ou enviar o documento para diversos e-mails, ative as opções "Enviar itens de NFSe separados no Json" e "Enviar múltiplos e-mails no Json" no cadastro da [Cidade](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral).
    *   **Reduções de Base:** a prefeitura só aceita notas com redução na base de cálculo do ISS (ex: 40%) caso exista um **benefício fiscal válido atrelado à operação**. Tentativas de redução sem amparo legal resultarão em rejeição do documento.

[\[voltar ao topo\]](#top)

### **Bernardo Sayão/TO**

O município de Bernardo Sayão/TO utiliza um **Sistema Próprio Municipal** para as Notas Fiscais de Serviço (NFS-e), e a emissão foi homologada de forma automatizada por meio da integração via webservice.

Esta homologação já contempla a adequação aos novos impostos da Reforma Tributária (**IBS e CBS**). Para garantir que suas notas sejam emitidas e aprovadas sem erros, siga o passo a passo de configuração abaixo:

*   **Cadastros Básicos**
    *   [**Cidades**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades)**:** na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral), preencha o "Mun. domicílio fiscal" com o código IBGE **1703206**.
    *   [**Empresa**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa)**:** confirme se a "Inscrição Municipal" da sua empresa está devidamente preenchida.
*   **Configurações do Serviço:** acesse o cadastro de [Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o) (abas [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaimpostos) e [Alíquotas de ISS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaalquotasdeiss)) e revise:
    *   **Código de Serviço Municipal:** preencha o campo "Cód. Trib. Município" com a formatação exigida pela prefeitura. Exemplo: **140101**.
    *   **Preenchimento obrigatório:** não esqueça de informar o "Item da Lista de Serviços (LC 116)" (ex: 1401), o "Código CNAE" (ex: 4520001) e o "Código NBS" (ex: 120024000, conforme a tabela oficial da Nomenclatura Brasileira de Serviços).
*   **Configuração para IBS e CBS (Reforma Tributária)** Para que os novos impostos sejam calculados e enviados corretamente ao portal da prefeitura:
    *   **Cadastro de** [Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o)**:** na [aba Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abaimpostos), [seção Reforma Tributária](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#01K56TN2K88BREGGCND4D6DBNF), preencha o campo **"Código Classificação Tributária Nacional"** (ex: 140101). Configure também as alíquotas de IBS e CBS pertinentes ao serviço.
    *   [**Tipos de Operação (TOP)**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP)**:** na [aba Reforma Tributária](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#01K56TN2K88BREGGCND4D6DBNF) da TOP, certifique-se de ativar as marcações **"Tem CBS"** e **"Tem IBS"**.
*   **Regras de Emissão e Particularidades**
    *   **Reduções de Base:** a prefeitura só aceita notas com redução na base de cálculo do ISS (ex: 40%) caso exista um **benefício fiscal válido atrelado à operação**. Tentativas de redução sem amparo legal resultarão em rejeição do documento.

[\[voltar ao topo\]](#top)

### **Palmas/TO**

Os seguintes cadastros estão envolvidos:

![1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22602097596311) Na tela [Cidades](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913), na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral), informe o **"Mun. domicílio fiscal"** de Palmas, sendo este 1721000 e o **"Cód. município SIAFI"** 9733

**![2 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22602141156375)** Acesse as [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893) na sub-aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaNFS-e) e defina no campo **"Regime esp. trib. ISS (NFS-e)"** o regime especial de tributação ISS a ser utilizado pela empresa conforme as opções admitidas:

<table class="wysiwyg-table-resized" style="margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 23%;"> <col style="width: 77%;"></colgroup><tbody><tr><td><strong>Código</strong></td><td><strong>Descrição</strong></td></tr><tr><td>1</td><td>Microempresa municipal</td></tr><tr><td>2</td><td>Estimativa</td></tr><tr><td>3</td><td>Sociedade de profissionais</td></tr><tr><td>4</td><td>Cooperativa</td></tr></tbody></table>

\*\*Nota:\*\*esta prefeitura permitirá a [Substituição de NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360046972414-Funcionalidades-relacionadas-%C3%A0-NFS-e#substituiodenfs-e) via webservice.

#### **Cancelamento**

Ao solicitar o cancelamento de uma NFS-e será aberto um pop-up para informar um dos motivos a seguir:

<table class="wysiwyg-table-resized" style="margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 23%;"> <col style="width: 77%;"></colgroup><tbody><tr><td><strong>Código</strong></td><td><strong>Descrição</strong></td></tr><tr><td>1</td><td>Erro na emissão</td></tr><tr><td>2</td><td>Serviço não prestado</td></tr><tr><td>4</td><td>Duplicidade na nota</td></tr></tbody></table>

**Importante:** os códigos **"3 - Erro de assinatura"** e **"5 - Erro de processamento"** são de uso restrito da Administração Tributária Municipal.

**Observação:** as notas fiscais de serviço emitidas nesta cidade podem conter o Código da Obra. Para realização das devidas configurações a respeito deste código, clique no link [Configuração para geração do Código da Obra](https://ajuda.sankhya.com.br/hc/pt-br/articles/360047599473-Configura%C3%A7%C3%B5es-gerais-para-NFS-e#configuraoparageraodocdigodaobra).

**Observação:** para que seja possível realizar o envio de NFS-e em modo síncrono para essa prefeitura é necessário habilitar o parâmetro **"Usa Serviço Síncrono para NFSe - USASINCRONOENV"**; assim, o envio de lote de NFS-e em modo síncrono possui um limite de 3 RPS por lote, de forma a não deixar o mesmo na fila de processamento.

[\[voltar ao topo\]](#top)

### **Paraíso do Tocantins/TO**

Os seguintes cadastros estão envolvidos:

![1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22602097596311) Na tela [Cidades](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913), na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral), informe o **"Mun. domicílio fiscal"** de Paraíso do Tocantins, sendo este 1721000 e o **"Cód. município SIAFI"** 973.

#### **Cancelamento**

Essa cidade possui apenas a descrição do motivo do cancelamento, ou seja, não há código. Além disso, deve-se informar um motivo até 250 caracteres.

[\[voltar ao topo\]](#top)

### **Tocantins/TO**

Os seguintes cadastros estão envolvidos:

![1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22602097596311) Na tela [Cidades](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913), na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral), informe o **"Mun. domicílio fiscal"** de Tocantins, sendo este 1716109 e o **"Cód. município SIAFI"** 9519.

![2 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22602141156375) Nos [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#top), acesse a aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abanfse) e configure no campo **"Cód. Natureza Oper. ISS (NFS-e)"** a natureza a ser utilizada na operação dentre as opções permitidas:

<table class="wysiwyg-table-resized" style="margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 17%;"> <col style="width: 83%;"></colgroup><tbody><tr><td><strong>Código</strong></td><td><strong>Descrição</strong></td></tr><tr><td>1</td><td>Microempresa municipal</td></tr><tr><td>2</td><td>Estimativa</td></tr><tr><td>3</td><td>Sociedade de profissionais</td></tr><tr><td>4</td><td>Cooperativa</td></tr><tr><td>5</td><td>Microempresário individual (MEI)</td></tr><tr><td>6</td><td>Microempresário e Empresa de Pequeno Porte (ME EPP)</td></tr></tbody></table>

**![3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22602141159575)** Acesse as [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa), aba [Documentos Fiscais Eletrônicos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaDocumentosFiscaisEletr%C3%B4nicos), sub-aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaNFS-e) > [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaGeralSub-abaNFS-e) e defina no campo **"Regime esp. trib. ISS (NFS-e)"** o regime especial de tributação ISS a ser utilizado pela empresa conforme as opções admitidas:

<table class="wysiwyg-table-resized" style="margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 18%;"> <col style="width: 82%;"></colgroup><tbody><tr><td><strong>Código</strong></td><td><strong>Descrição</strong></td></tr><tr><td>1</td><td>Microempresa municipal</td></tr><tr><td>2</td><td>Estimativa</td></tr><tr><td>3</td><td>Sociedade de profissionais</td></tr><tr><td>4</td><td>Cooperativa</td></tr><tr><td>5</td><td>Microempresário individual (MEI)</td></tr><tr><td>6</td><td>Microempresário e Empresa de Pequeno Porte (ME EPP)</td></tr></tbody></table>

A opção **"Considera valor líquido para NFS-e"** deve estar acionada para que o desconto informado nos itens seja considerado no valor do serviço enviado para prefeitura.

#### **Cancelamento**

Ao solicitar o cancelamento de uma NFS-e será aberto um pop-up para informar um dos motivos a seguir:

<table class="wysiwyg-table-resized" style="margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 19%;"> <col style="width: 81%;"></colgroup><tbody><tr><td><strong>Código</strong></td><td><strong>Descrição</strong></td></tr><tr><td>1</td><td>Erro na emissão</td></tr><tr><td>2</td><td>Serviço não prestado</td></tr><tr><td>4</td><td>Duplicidade na nota</td></tr></tbody></table>

**Importante:** os códigos **"3 - Erro de assinatura"** e **"5 - Erro de processamento"** são de uso restrito da Administração Tributária Municipal.

[\[voltar ao topo\]](#top)