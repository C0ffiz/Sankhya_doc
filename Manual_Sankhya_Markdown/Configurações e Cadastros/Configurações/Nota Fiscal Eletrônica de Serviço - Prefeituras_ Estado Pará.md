# Nota Fiscal Eletrônica de Serviço - Prefeituras: Estado Pará

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/22600243711511-Nota-Fiscal-Eletr%C3%B4nica-de-Servi%C3%A7o-Prefeituras-Estado-Par%C3%A1](https://ajuda.sankhya.com.br/hc/pt-br/articles/22600243711511-Nota-Fiscal-Eletr%C3%B4nica-de-Servi%C3%A7o-Prefeituras-Estado-Par%C3%A1)

---

# Nota Fiscal Eletrônica de Serviço - Prefeituras: Estado Pará

Neste artigo serão apresentadas as especificações de emissão de NFS-e das cidades localizadas no estado do Pará, para conhecê-las acesse os links abaixo:

<table style="border-collapse: collapse; margin-left: 0px; margin-right: auto;"><tbody><tr><td style="text-align: center; width: 72.9524%;" colspan="2"><h4 id="h_01HTQPZR8H99GNYC2JA45NNTJE"><span style="color: #4D4D4D;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><strong>Cidades</strong></span></span></h4></td></tr><tr><td style="width: 34.1905%;"><a href="#barcarena/pa" target="_self"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Barcarena/PA</span></a><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;</span></td><td style="width: 38.7619%;"><a class="topiclink" href="#parauapebaspa"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Parauapebas/PA</span></a></td></tr><tr><td style="width: 34.1905%;"><a class="topiclink" href="#belmpa"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Belém/PA</span></a></td><td style="width: 38.7619%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"></span><a href="#Reden%C3%A7%C3%A3o/PA"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Redenção/PA</span></a></td></tr><tr><td><a href="#h_01KKH4THE5Y8ZYCAH27KGJ65QS">Itaituba/PA</a></td><td style="width: 38.7619%;"><a href="#01JXA9YW692JNTXEJYAD0055T3">Pau D'Arco/PA</a></td></tr><tr><td><a href="#h_01KKH4THE5Y8ZYCAH27KGJ65QS">Marabá/PA</a></td><td><a href="#h_01KTS0JFW3H7DRZH00Z357SN05">Santarém/PA</a></td></tr><tr><td style="width: 34.1905%;"><a class="topiclink" href="#paragominaspa"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Paragominas/PA</span></a></td><td><span style="font-family: Verdana,Geneva,Arial,sans-serif;"></span><a href="#Xinguara/PA"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Xinguara/PA</span></a></td></tr></tbody></table>

### **Barcarena/PA**

O sistema encontra-se apto para emitir NFS-e para o município de Barcarena.

**Observação:** a cidade suporta o cancelamento de nota de serviço via webservice.

[\[voltar ao topo\]](#top)

### **Belém/PA**

A emissão de NFS-e para o município de Belém poderá ser realizada via **API**, desde que seja ativado o parâmetro **“Utilizar emissor NFS-e em Curitiba pelo Broker? – NFSECURITBROKER”**.

Este parâmetro é **indispensável** para garantir a conformidade das emissões.

O sistema encontra-se apto para emitir NFS-e para o município de Belém.

**Observação:** a cidade suporta o cancelamento de nota de serviço via webservice.

[\[voltar ao topo\]](#top)

### **Itaituba/PA**

O município de Itaituba/PA utiliza um **Sistema Próprio Municipal** para as Notas Fiscais de Serviço (NFS-e), e a emissão foi homologada de forma automatizada por meio da integração via webservice.

Para que suas notas sejam emitidas e aprovadas sem erros, siga o passo a passo de configuração abaixo:

*   **Cadastros Básicos**
    *   [**Cidades**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades)**:** na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral), preencha o **"Mun. domicílio fiscal"** com o código IBGE **1503606**.
    *   [**Empresas**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa)**:** confirme se a **"Inscrição Municipal"** e o **"Cód. Regime Tribut."** (ex: Lucro Real) da sua empresa estão devidamente preenchidos.
*   **Configurações do Serviço:**  acesse o cadastro de [Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o) (abas [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaimpostos) e [Alíquotas de ISS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaalquotasdeiss)) e revise:
    *   **Código de Serviço Municipal:** preencha o campo **"Cód. Trib. Município"** com a formatação exigida pela prefeitura (ex: **0000110000004**).
    *   **Preenchimento obrigatório:** não esqueça de informar o **"Item da Lista de Serviços (LC 116)"** (ex: 11.04), o **"Código CNAE"** (ex: 4930204) e o **"Código NBS"** (ex: 1.0601.90.00, conforme a tabela oficial da Nomenclatura Brasileira de Serviços).
*   **Regras de Emissão e Particularidades**
    *   **Múltiplos Itens e E-mails:** para incluir vários serviços na mesma nota ou enviar o documento para diversos e-mails, ative as opções **"Enviar itens de NFSe separados no Json"** e **"Enviar múltiplos e-mails no Json"** no cadastro da  [Cidade](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades).
    *   **ISS Retido e Exterior:** o sistema permite a emissão de notas com ISS retido e para clientes do exterior normalmente (mediante preenchimento correto do endereço do tomador).
    *   **Cancelamento e Substituição:** o **Cancelamento** via sistema está homologado e funcional. No entanto, a operação de **Substituição** pode não ser suportada pelo webservice da prefeitura (cenário em análise). Caso ocorra rejeição ao tentar substituir, a recomendação é cancelar a nota original e emitir um novo documento.
    *   **Atenção às Reduções de Base:** o sistema está preparado para calcular deduções na base do ISS. Porém, a prefeitura bloqueia a emissão caso a atividade prestada não permita essa redução. Consulte o regulamento do município para confirmar quais serviços autorizam a dedução da base de cálculo antes de emitir a nota.

[\[voltar ao topo\]](#top)

### **Marabá/PA**

O município de Marabá/PA utiliza o **Emissor Nacional** para as Notas Fiscais de Serviço (NFS-e), e a emissão foi homologada de forma automatizada por meio da integração via webservice.

Esta homologação já contempla a adequação aos novos impostos da Reforma Tributária (**IBS e CBS**). Para que suas notas sejam emitidas e aprovadas sem erros, siga o passo a passo de configuração abaixo:

*   **Cadastros Básicos**
    *   [**Cidades**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades)**:** na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral), preencha o **"Mun. domicílio fiscal"** com o código IBGE **1504208**.
    *   **Empresas:** confirme se a **"Inscrição Municipal"** e o **"Cód. Regime Tribut."** (ex: Lucro Real) da sua empresa estão devidamente preenchidos.
*   **Série e Numeração (Exigência de 5 dígitos):** por utilizar o Portal Nacional, a prefeitura exige que a série da nota tenha exatamente 5 caracteres. Configure da seguinte forma:
    *   **Preferências da Empresa:** (Caminho: [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa), aba [Documentos Fiscais Eletrônicos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaDocumentosFiscaisEletr%C3%B4nicos), sub-aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaNFS-e) > [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaGeralSub-abaNFS-e)) preencha o **"Prefixo Série NFS-e Padrão Nacional"** com 2 dígitos, usando números de **00 a 49**.
    *   **TOP (Tipos de Operação):** (Caminho: botão [Outras Opções](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#botooutrasopes...) > [Controle de Numeração](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#controledenumeracao)) configure a **"Série Padrão Nacional"** com 3 dígitos (ex: de **001 a 999**) e ative a numeração automática.
*   **Configurações do Serviço:** acesse o cadastro de [Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o) (abas [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaimpostos) e [Alíquotas de ISS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaalquotasdeiss)) e revise:
    *   **Código de Serviço Municipal:** o Portal Nacional exige um formato específico. Adicione o dígito **"01"** ao final do código original do serviço. Exemplo: preencha como **140101001**.
    *   **Preenchimento obrigatório:** não esqueça de informar o **"Item da Lista de Serviços (LC 116)"** (ex: 140101), e o **"Código CNAE"** (ex: 45.30-7-05).
*   **Configuração para IBS e CBS (Reforma Tributária)** Para que os novos impostos sejam calculados e enviados corretamente ao portal da prefeitura:
    *   **Cadastro de Serviço:** na [Seção Reforma Tributária](https://xn--seo%20reforma%20tributria-ycc7a5i/), na aba [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaimpostos), configure as alíquotas de IBS e CBS pertinentes ao serviço.
    *   [**Tipos de Operação (TOP)**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP)**:** na aba [Reforma Tributária](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#01K56TN2K88BREGGCND4D6DBNF) da TOP, certifique-se de ativar as marcações referentes ao cálculo de CBS e IBS.
*   **Regras de Emissão e Particularidades**
    *   **Ative o Padrão Nacional:** lembre-se de ativar a marcação **"Emitir NFS-e Padrão Nacional"** nas [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa).
    *   **Cancelamento e Substituição:** o município suporta tanto o **Cancelamento** quanto a **Substituição** de notas via webservice. Ambas as operações podem ser realizadas diretamente pelo sistema Sankhya sem erros, com atualização automática do status.
    *   **Tomador do Exterior e ISS Retido:** o sistema permite a emissão de notas com retenção de ISS e para clientes do exterior normalmente (mediante preenchimento do endereço estrangeiro sem obrigatoriedade de CEP/UF brasileiro).
    *   **Múltiplos Itens e E-mails:** para incluir vários serviços na mesma nota ou enviar o documento para diversos e-mails, ative as opções **"Enviar itens de NFSe separados no Json"** e **"Enviar múltiplos e-mails no Json"** no [cadastro da Cidade](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades).
    *   **Atenção às Reduções de Base:** a prefeitura de Marabá/PA **não aceita** dedução na base de cálculo do ISS. Tentar emitir notas com base reduzida resultará em rejeição do documento.

[\[voltar ao topo\]](#top)

### **Paragominas/PA**

Os seguintes cadastros estão envolvidos:

 **![1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22600647921687)**Na tela [Cidades](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913), aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral), informe o **"Mun. domicílio fiscal"** de Paragominas, sendo este 1505502 e o **"Cód. município SIAFI"** 0509.

 ![2 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22600647938967)Nos [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#top), acesse a aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abanfse) e configure no campo **"Cód. Natureza Oper. ISS (NFS-e)"** a natureza a ser utilizada na operação. São permitidas as seguintes opções:

<table style="border-collapse: collapse; margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #ffffff; width: 14.5714%;"><span style="color: #4D4D4D;"><strong>Código</strong></span></td><td style="background-color: #ffffff; width: 85.4286%;"><span style="color: #4D4D4D;"><strong>&nbsp;Descrição</strong></span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;1</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Tributação no Município</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;2</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Tributação fora do Município</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;3</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Isenção</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;4</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Imune</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;5</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Exigibilidade suspensa por decisão judicial</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;6</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Exigibilidade suspensa por procedimento administrativo</span></td></tr></tbody></table>

 ![3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22600672446103)**Acesse as** [**Preferências da Empresa**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa)**, aba** [**Documentos Fiscais Eletrônicos**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaDocumentosFiscaisEletr%C3%B4nicos)**, sub-aba** [**NFS-e**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaNFS-e) **>** [**Geral**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaGeralSub-abaNFS-e) **e**  **defina no campo "Regime esp. tributação ISS (NFS-e)" o regime especial de tributação ISS a ser utilizado pela empresa conforme as opções admitidas:** 

<table style="border-collapse: collapse; margin-left: 0px; margin-right: auto;"><tbody><tr style="background-color: #ffffff; height: 22px;"><td style="height: 33px; width: 12.4286%;"><span style="color: #4D4D4D;"><strong>&nbsp;Código</strong></span></td><td style="height: 33px; width: 87.5714%;"><span style="color: #4D4D4D;"><strong>&nbsp;Descrição</strong></span></td></tr><tr style="height: 22px;"><td style="height: 33px; width: 12.4286%;"><span style="color: #4D4D4D;">&nbsp;1</span></td><td style="height: 33px; width: 87.5714%;"><span style="color: #4D4D4D;">&nbsp;Microempresa municipal</span></td></tr><tr style="height: 22px;"><td style="height: 33px; width: 12.4286%;"><span style="color: #4D4D4D;">&nbsp;2</span></td><td style="height: 33px; width: 87.5714%;"><span style="color: #4D4D4D;">&nbsp;Estimativa</span></td></tr><tr style="height: 22px;"><td style="height: 33px; width: 12.4286%;"><span style="color: #4D4D4D;">&nbsp;3</span></td><td style="height: 33px; width: 87.5714%;"><span style="color: #4D4D4D;">&nbsp;Sociedade de profissionais&nbsp;</span></td></tr><tr style="height: 22px;"><td style="height: 33px; width: 12.4286%;"><span style="color: #4D4D4D;">&nbsp;4</span></td><td style="height: 33px; width: 87.5714%;"><span style="color: #4D4D4D;">&nbsp;Cooperativa</span></td></tr><tr style="height: 22px;"><td style="height: 33px; width: 12.4286%;"><span style="color: #4D4D4D;">&nbsp;5&nbsp;</span></td><td style="height: 33px; width: 87.5714%;"><span style="color: #4D4D4D;">&nbsp;Microempresário Individual (MEI)</span></td></tr><tr style="height: 22px;"><td style="height: 33px; width: 12.4286%;"><span style="color: #4D4D4D;">&nbsp;6</span></td><td style="height: 33px; width: 87.5714%;"><span style="color: #4D4D4D;">&nbsp;Microempresário e Empresa de Pequeno Porte (ME EPP)</span></td></tr></tbody></table>

#### **Cancelamento**

Ao solicitar o cancelamento de uma NFS-e será aberto um pop-up para informar um dos motivos a seguir:

<table style="border-collapse: collapse; margin-left: 0px; margin-right: auto;"><tbody><tr style="background-color: #ffffff; height: 22px;"><td style="height: 22px; width: 12.4286%;"><span style="color: #4D4D4D;"><strong>&nbsp;Código</strong></span></td><td style="height: 22px; width: 87.5714%;"><span style="color: #4D4D4D;"><strong>&nbsp;Descrição</strong></span></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 12.4286%;"><span style="color: #4D4D4D;">&nbsp;1</span></td><td style="height: 22px; width: 87.5714%;"><span style="color: #4D4D4D;">&nbsp;Erro na emissão</span></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 12.4286%;"><span style="color: #4D4D4D;">&nbsp;2</span></td><td style="height: 22px; width: 87.5714%;"><span style="color: #4D4D4D;">&nbsp;Serviço não prestado</span></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 12.4286%;"><span style="color: #4D4D4D;">&nbsp;4</span></td><td style="height: 22px; width: 87.5714%;"><span style="color: #4D4D4D;">&nbsp;Duplicidade na nota</span></td></tr></tbody></table>

**Importante:** os códigos **"3 - Erro de assinatura"** e **"5 - Erro de processamento"** são de uso restrito da Administração Tributária Municipal.

[\[voltar ao topo\]](#top)

### **Parauapebas/PA**

Os seguintes cadastros estão envolvidos:

 **![1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22600647921687)**Na tela [Cidades](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913), aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral), informe o **"Mun. domicílio fiscal"** de Parauapebas, sendo este 1505536 e o **"Cód. município SIAFI"** 0595.

**Observação:** para obter a chave de acesso é necessário que a empresa acesse o [Portal Governa](https://governa.presidencia.gov.br/) com seu usuário e senha, entre no menu **"Gerenciamento > Configurar Padrão"** e configure o módulo webservice. Neste momento será gerada a chave de acesso para a empresa, podendo esta alterá-la sempre que desejado.

 **![2 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22600647938967)**Nos [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114), aba [Livro Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abalivrofiscal), defina no campo **"Forma de Recolhimento ISS"** a forma de recolhimento da operação realizada.

Já, na aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abanfse), configure no campo **"Cód. Natureza Oper. ISS (NFS-e)"** a natureza a ser utilizada na operação. São permitidas as seguintes opções:

<table style="border-collapse: collapse; margin-left: 0px; margin-right: auto;"><tbody><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;"><strong>Código</strong></span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;"><strong>&nbsp;Descrição</strong></span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;1</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Tributação no Município</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;2</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Tributação fora do Município</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;3</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Isenção</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;4</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Imune</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;5</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Exigibilidade suspensa por decisão judicial</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;6</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Exigibilidade suspensa por procedimento administrativo</span></td></tr></tbody></table>

Para configurar o campo acima, deve-se atentar aos seguintes pontos:

*   Para flexibilizar o cadastro de novas naturezas de operação no momento da implantação de novos provedores de NFS-e e novos municípios, foi criada a aba [Natureza da Operação ISS/Município](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abanaturezadaoperaoissmunicpio) no cadastro de [Tipos de Operação-TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#top);
    
*   Esta aba somente estará disponível se o parâmetro **"Utilizar Cód. Nat. Operação ISS por Top/Empresa - NATOPEISSTOPEMP"** estiver habilitado;
    
*   Deve-se incluir a empresa relacionada a emissão das notas e a natureza da operação relacionada ao município de domicílio fiscal da cidade em que a empresa se encontra.
    

**Nota:** com o parâmetro NATOPEISSTOPEMP ativado, o campo Cód. Natureza Oper. ISS (NFS-e) da aba NFS-e será retirado do cadastro de Tipos de Operação - TOP. A configuração desta aba evita a criação de uma TOP para cada empresa que tenha uma natureza de operação diferente; com este formato a mesma TOP pode ser utilizada por empresas que tenham naturezas diferentes.

**Observação:** para o cadastro de natureza da operação, os registros deverão ser incluídos via script ('SCRIPT\_NATUREZAS\_OPERACAO\_ISS') do banco de dados na tabela TGFNAS.

#### **XML's na Emissão de Notas**

Os XML's gerados para as notas desse município possuem algumas particularidades quanto a algumas TAG's. Observe:

**Forma de Recolhimento**

Serão aceitos os seguintes códigos:

<table style="border-collapse: collapse; margin-left: 0px; margin-right: auto;"><tbody><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;"><strong>Código</strong></span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;"><strong>&nbsp;Descrição</strong></span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;00</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;A Recolher</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;01</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Retido na Fonte</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;03</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Devido a Outro Município</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;04</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Sem Recolhimento</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;05</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Fixo/Anual</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;06</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Fixo/Mensal</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;07</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Simples Nacional</span></td></tr></tbody></table>

**Regime de Recolhimento**

Serão aceitos os seguintes códigos:

<table style="border-collapse: collapse; margin-left: 0px; margin-right: auto;"><tbody><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;"><strong>Código</strong></span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;"><strong>&nbsp;Descrição</strong></span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;00</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Normal</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;03</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Isento</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;04</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Imune</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;07</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Não Incidência</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;08</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Estimado</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;09</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Autônomo</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;11</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Simples Nacional</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;14</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;MEI</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4D4D4D;">&nbsp;15</span></td><td style="width: 85.4286%;"><span style="color: #4D4D4D;">&nbsp;Uniprofissional</span></td></tr></tbody></table>

 **![3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22600672446103)**Acesse as [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa), aba [Documentos Fiscais Eletrônicos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaDocumentosFiscaisEletr%C3%B4nicos), sub-aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaNFS-e) > [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaGeralSub-abaNFS-e) e defina no campo **"Chave de Acesso da NFS-e"** a chave de acesso que foi vinculada à empresa juntamente a prefeitura. 

**Defina no campo "Regime esp. tributação ISS (NFS-e)" o regime especial de tributação ISS a ser utilizado pela empresa conforme as opções admitidas:**

<table style="border-collapse: collapse; margin-left: 0px; margin-right: auto;"><tbody><tr style="height: 22px;"><td style="height: 22px; width: 12.8571%;"><span style="color: #4D4D4D;"><strong>&nbsp;Código</strong></span></td><td style="height: 22px; width: 87.1429%;"><span style="color: #4D4D4D;"><strong>&nbsp;Descrição</strong></span></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 12.8571%;"><span style="color: #4D4D4D;">&nbsp;1</span></td><td style="height: 22px; width: 87.1429%;"><span style="color: #4D4D4D;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;Microempresa municipal</span></span></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 12.8571%;"><span style="color: #4D4D4D;">&nbsp;2</span></td><td style="height: 22px; width: 87.1429%;"><span style="color: #4D4D4D;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;Estimativa</span></span></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 12.8571%;"><span style="color: #4D4D4D;">&nbsp;3</span></td><td style="height: 22px; width: 87.1429%;"><span style="color: #4D4D4D;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;Sociedade de profissionais</span></span></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 12.8571%;"><span style="color: #4D4D4D;">&nbsp;4</span></td><td style="height: 22px; width: 87.1429%;"><span style="color: #4D4D4D;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;Cooperativa</span></span></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 12.8571%;"><span style="color: #4D4D4D;">&nbsp;5&nbsp;</span></td><td style="height: 22px; width: 87.1429%;"><span style="color: #4D4D4D;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;Microempresário Individual(MEI)</span></span></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 12.8571%;"><span style="color: #4D4D4D;">&nbsp;6</span></td><td style="height: 22px; width: 87.1429%;"><span style="color: #4D4D4D;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;Microempresário e Empresa de Pequeno Porte (ME EPP)</span></span></td></tr></tbody></table>

#### **Cancelamento**

Ao solicitar o cancelamento de uma NFS-e será aberto um pop-up para informar um dos motivos a seguir:

<table style="border-collapse: collapse; margin-left: 0px; margin-right: auto;"><tbody><tr style="height: 22px;"><td style="height: 22px; width: 12.4286%;"><span style="color: #4D4D4D;"><strong>&nbsp;Código</strong></span></td><td style="height: 22px; width: 87.5714%;"><span style="color: #4D4D4D;"><strong>&nbsp;Descrição</strong></span></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 12.4286%;"><span style="color: #4D4D4D;">&nbsp;1</span></td><td style="height: 22px; width: 87.5714%;"><span style="color: #4D4D4D;">&nbsp;Erro na emissão</span></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 12.4286%;"><span style="color: #4D4D4D;">&nbsp;2</span></td><td style="height: 22px; width: 87.5714%;"><span style="color: #4D4D4D;">&nbsp;Serviço não prestado</span></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 12.4286%;"><span style="color: #4D4D4D;">&nbsp;4</span></td><td style="height: 22px; width: 87.5714%;"><span style="color: #4D4D4D;">&nbsp;Duplicidade na nota</span></td></tr></tbody></table>

**Importante:** os códigos **"3 - Erro de assinatura"** e **"5 - Erro de processamento"** são de uso restrito da Administração Tributária Municipal.

A prefeitura de Parauapebas/PA **não aceita a substituição de NFS-e via Webservice (eNotas)**. A operação de substituição deve ser realizada **diretamente no portal da prefeitura**.

---

 **![informações adicionais FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28923297237527) Informações adicionais acerca da Emissão de NFS-e no município de Parauapebas/PA:**

*   Nesta prefeitura, ao realizar a emissão de NFSe com tomador do exterior ou ISS retido, o sistema emitirá a nota sem erros;
    
*   Para emitir uma nota fiscal com variados cadastros de serviços, habilite a marcação **"Enviar itens de NFSe separados no JSON"** no cadastro de [Cidades](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades), aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abanfs-e);
*   Caso queira cadastrar o envio da nota para mais de um e-mail, preencha o campo **"E-mail específico p/ envio NFSe"** na aba [NF-e/NFS-e/CT-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros#abanf-enfs-ect-e), no cadastro de [Parceiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros) e habilite a marcação **"Envia múltiplos e-mails no JSON"** no cadastro de Cidades, aba NFS-e;
*   Será possível, ainda, calcular a redução do imposto no cálculo automaticamente, basta que o campo **"Tipo de dedução de base do ISS"** da aba [Alíquota de ISS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaalquotasdeiss), do cadastro de [Serviço](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o), esteja definida com a opção **"Materiais"** e o campo **"Percentual de ISS"** possua o valor a ser deduzido.

[\[voltar ao topo\]](#top)

### **Redenção/PA**

Os seguintes cadastros estão envolvidos:

 ![1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22600647921687) Na tela [Cidades](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades), aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral), informe o **"Mun. domicílio fiscal"** de Redenção, sendo este 1506138 e o **"Cód. município SIAFI"** 0567.

 ![2 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22600647938967) Acesse as [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893), aba [Documentos Fiscais Eletrônicos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaDocumentosFiscaisEletr%C3%B4nicos), sub-aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaNFS-e) > [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaGeralSub-abaNFS-e) e defina no campo **"Regime esp. trib. ISS (NFS-e)"** o regime especial de tributação ISS a ser utilizado pela empresa conforme as opções admitidas:

<table class="wysiwyg-table-resized" style="margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 15%;"> <col style="width: 85%;"></colgroup><tbody><tr><td style="width: 14.5714%;"><span style="color: #4d4d4d;"><strong>&nbsp;Código</strong></span></td><td style="width: 85.2857%;"><span style="color: #4d4d4d;"><strong>&nbsp;Descrição</strong></span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4d4d4d;">&nbsp;1</span></td><td style="width: 85.2857%;"><span style="color: #4d4d4d;">&nbsp;Simples Nacional</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4d4d4d;">&nbsp;2</span></td><td style="width: 85.2857%;"><span style="color: #4d4d4d;">&nbsp;Normal</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4d4d4d;">&nbsp;3</span></td><td style="width: 85.2857%;"><span style="color: #4d4d4d;">&nbsp;Especial</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4d4d4d;">&nbsp;4</span></td><td style="width: 85.2857%;"><span style="color: #4d4d4d;">&nbsp;Estimativa</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4d4d4d;">&nbsp;5</span></td><td style="width: 85.2857%;"><span style="color: #4d4d4d;">&nbsp;Microempresário Individual (MEI)</span></td></tr><tr><td style="width: 14.5714%;"><span style="color: #4d4d4d;">&nbsp;6&nbsp;</span></td><td style="width: 85.2857%;"><span style="color: #4d4d4d;">&nbsp;Profissional Autônomo</span></td></tr></tbody></table>

 ![3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/22600672446103) Nos [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#top), acesse a aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abanfse) e configure no campo **"Cód. Natureza Oper. ISS (NFS-e)"** a natureza a ser utilizada na operação. São permitidas as seguintes opções:

<table class="wysiwyg-table-resized" style="margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 15%;"> <col style="width: 85%;"></colgroup><tbody><tr><td><span style="color: #4d4d4d;"><strong>&nbsp;Código</strong></span></td><td><span style="color: #4d4d4d;"><strong>&nbsp;Descrição</strong></span></td></tr><tr><td><span style="color: #4d4d4d;">&nbsp;1</span></td><td><span style="color: #4d4d4d;">&nbsp;Tributável</span></td></tr><tr><td><span style="color: #4d4d4d;">&nbsp;2</span></td><td><span style="color: #4d4d4d;">&nbsp;Imune</span></td></tr><tr><td><span style="color: #4d4d4d;">&nbsp;3</span></td><td><span style="color: #4d4d4d;">&nbsp;Isento</span></td></tr><tr><td><span style="color: #4d4d4d;">&nbsp;4</span></td><td><span style="color: #4d4d4d;">&nbsp;Exigibilidade suspensa por decisão judicial</span></td></tr><tr><td><span style="color: #4d4d4d;">&nbsp;5</span></td><td><span style="color: #4d4d4d;">&nbsp;Exigibilidade suspensa por procedimento administrativo</span></td></tr></tbody></table>

#### **Cancelamento**

Ao solicitar o cancelamento de uma NFS-e será aberto um pop-up para informar um dos motivos a seguir:

<table class="wysiwyg-table-resized" style="margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 12%;"> <col style="width: 88%;"></colgroup><tbody><tr><td><span style="color: #4d4d4d;"><strong>&nbsp;Código</strong></span></td><td><span style="color: #4d4d4d;"><strong>&nbsp;Descrição</strong></span></td></tr><tr><td><span style="color: #4d4d4d;">&nbsp;1</span></td><td><span style="color: #4d4d4d;">&nbsp;Erro na emissão</span></td></tr><tr><td><span style="color: #4d4d4d;">&nbsp;2</span></td><td><span style="color: #4d4d4d;">&nbsp;Serviço não prestado</span></td></tr><tr><td><span style="color: #4d4d4d;">&nbsp;3</span></td><td><span style="color: #4d4d4d;">&nbsp;Duplicidade na nota</span></td></tr></tbody></table>

**Essa prefeitura não permite substituição via webservice.**

---

 **![informações adicionais FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28923297237527) Informações adicionais acerca da Emissão de NFS-e no município de Redenção:**

*   Nesta prefeitura, ao realizar a emissão de NFSe com tomador do exterior ou ISS retido, o sistema emitirá a nota sem erros;
*   Para emitir uma nota fiscal com variados cadastros de serviços, habilite a marcação **"Enviar itens de NFSe separados no JSON"** no cadastro de [Cidades](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades), aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abanfs-e);
*   Caso queira cadastrar o envio da nota para mais de um e-mail, preencha o campo **"E-mail específico p/ envio NFSe"** na aba [NF-e/NFS-e/CT-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros#abanf-enfs-ect-e), no cadastro de [Parceiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros) e habilite a marcação **"Envia múltiplos e-mails no JSON"** no cadastro de [Cidades](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades), aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abanfs-e);
*   Será possível ainda, calcular a redução do imposto no cálculo automaticamente, basta que o campo **"Tipo de dedução de base do ISS"** da aba [Alíquota de ISS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaalquotasdeiss), do cadastro de [Serviço](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o), esteja definida com a opção **"Materiais"** e o campo **"Percentual de ISS"** possua o valor a ser deduzido.

[\[voltar ao topo\]](#top)

### **Pau D'Arco/PA**

O município de Pau D'Arco/PA utiliza o **Sistema Próprio Municipal** para as Notas Fiscais de Serviço (NFS-e), e a emissão foi homologada de forma automatizada por meio da integração via webservice.

Para que suas notas sejam emitidas e aprovadas sem erros, siga o passo a passo de configuração abaixo:

*   **Cadastros Básicos**
    *   [**Cidades**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades)**:** na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral), preencha o "Mun. domicílio fiscal" com o código IBGE **1505551**.
    *   [**Empresa**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa)**:** confirme se a **"Inscrição Municipal"** da sua empresa está devidamente preenchida.
*   **Configurações do Serviço:** acesse o cadastro de [Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o) (abas [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaimpostos) e [Alíquotas de ISS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaalquotasdeiss)) e revise:
    *   **Código de Serviço Municipal:** preencha o campo **"Cód. Trib. Município"** com a formatação exigida pela prefeitura. Exemplo: **140101**.
    *   **Preenchimento obrigatório:** não esqueça de informar o **"Item da Lista de Serviços (LC 116)"** (ex: 1401), o **"Código CNAE"** (ex: 4520001) e o **"Código NBS"** (ex: 120024000, conforme a tabela oficial da Nomenclatura Brasileira de Serviços).
*   **Regras de Emissão e Particularidades**
    *   **Múltiplos Itens e E-mails:** para incluir vários serviços na mesma nota ou enviar o documento para diversos e-mails, ative as opções **"Enviar itens de NFSe separados no Json"** e **"Enviar múltiplos e-mails no Json"** no cadastro da [Cidade](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral).

[\[voltar ao topo\]](#top)

### 

### **Santarém/PA**

O município de Santarém/PA utiliza o **Emissor Nacional** (Portal Nacional) para as Notas Fiscais de Serviço (NFS-e), e a emissão foi homologada de forma automatizada por meio da integração via webservice.

Esta homologação já contempla a adequação aos novos impostos da Reforma Tributária (**IBS e CBS**). Para que suas notas sejam emitidas e aprovadas sem erros, siga o passo a passo de configuração abaixo:

*   **Cadastros Básicos**
    *   [**Cidades**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades)**:** na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral), preencha o **"Mun. domicílio fiscal"** com o código IBGE **1506807**.
    *   [**Empresa**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa)**:** confirme se a **"Inscrição Municipal"** e o **"Cód. Regime Tribut."** da sua empresa estão devidamente preenchidos.
*   **Série e Numeração (Exigência de 5 dígitos)** Por utilizar o Portal Nacional, a prefeitura exige que a série da nota tenha exatamente 5 caracteres. Configure da seguinte forma:
    *   **Preferências da Empresa:** (Caminho: [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa), aba [Documentos Fiscais Eletrônicos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaDocumentosFiscaisEletr%C3%B4nicos), sub-aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaNFS-e) > [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#Sub-abaGeralSub-abaNFS-e)) preencha o **"Prefixo Série NFS-e Padrão Nacional"** com 2 dígitos, usando números de **00 a 49**.
    *   **TOP (Tipos de Operação):** (Caminho: [Outras Opções](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#botooutrasopes...) > [Controle de Numeração](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#controledenumeracao)) configure a **"Série Padrão Nacional"** com 3 dígitos (ex: de **001 a 999**) e ative a numeração automática.
*   **Configurações do Serviço:** acesse o cadastro de [Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o) (abas [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaimpostos) e [Alíquotas de ISS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaalquotasdeiss)) e revise:
    *   **Código de Serviço Municipal:** preencha o campo **"Cód. Trib. Município"** com a formatação exigida pelo portal nacional. Exemplo: **07.13.01.118**.
    *   **Preenchimento obrigatório:** não esqueça de informar o **"Item da Lista de Serviços (LC 116)"** (ex: 07.13), o **"Código CNAE"** (ex: 7119799) e o **"Código NBS"** (ex: 114031000, conforme a tabela oficial da Nomenclatura Brasileira de Serviços).
*   **Configuração para IBS e CBS (Reforma Tributária)** Para que os novos impostos sejam calculados e enviados corretamente ao portal:
    *   **Cadastro de** [Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o)**:** na [aba Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abaimpostos), [seção Reforma Tributária](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#01K56TN2K88BREGGCND4D6DBNF), preencha o campo **"Código Classificação Tributária Nacional"** (ex: 140101). Configure também as alíquotas de IBS e CBS pertinentes ao serviço.
    *   [**Tipos de Operação (TOP)**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP)**:** na [aba Reforma Tributária](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#01K56TN2K88BREGGCND4D6DBNF) da TOP, certifique-se de ativar as marcações **"Tem CBS"** e **"Tem IBS"**.
*   **Regras de Emissão e Particularidades**
    *   **Ative o Padrão Nacional:** lembre-se de ativar a marcação **"Emitir NFS-e Padrão Nacional"** nas [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa).
    *   **Cancelamento e Substituição:** o município suporta tanto o **Cancelamento** quanto a **Substituição** de notas via webservice. Ambas as operações podem ser realizadas diretamente pelo sistema Sankhya sem erros.
    *   **Tomador do Exterior e ISS Retido:** o sistema permite a emissão de notas com retenção de ISS e para clientes do exterior normalmente (mediante preenchimento correto do endereço estrangeiro do tomador).
    *   **Múltiplos Itens e E-mails:** para incluir vários serviços na mesma nota ou enviar o documento para diversos e-mails, ative as opções **"Enviar itens de NFSe separados no Json"** e **"Enviar múltiplos e-mails no Json"** no [cadastro da Cidade](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades).
    *   **Reduções de Base Não Permitidas:** a prefeitura de Santarém/PA **não permite** deduções/reduções na base de cálculo do ISS via integração (Erro E0440 - "O tipo de dedução/redução informado na DPS não é permitida pelo município..."). Tentativas de emitir notas com dedução resultarão em rejeição pelo portal.

[\[voltar ao topo\]](#top)

### 

### **Xinguara/PA**

O sistema encontra-se apto para emitir NFS-e para o município de Xinguara.

**Observação:** a cidade suporta o cancelamento e a [Substituição](https://ajuda.sankhya.com.br/hc/pt-br/articles/360046972414-Funcionalidades-relacionadas-%C3%A0-NFS-e#substituiodenfs-e) de nota de serviço via webservice.

---

**![informações adicionais FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28923297237527)** **Informações adicionais acerca da Emissão de NFS-e no município de Xinguara:**

*   Para emitir uma nota fiscal com variados cadastros de serviços, habilite a marcação **"Enviar itens de NFSe separados no JSON"** no cadastro de [Cidades](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades), aba [NFS-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abanfs-e);
    
*   Caso queira cadastrar o envio da nota para mais de um e-mail, preencha o campo **"E-mail específico p/ envio NFSe"** na aba [NF-e/NFS-e/CT-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros#abanf-enfs-ect-e), no cadastro de [Parceiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros) e habilite a marcação **"Envia múltiplos e-mails no JSON"** no cadastro de Cidades, aba NFS-e;
    
*   Será possível ainda, calcular a redução do imposto no cálculo automaticamente, basta que o campo **"Tipo de dedução de base do ISS"** da aba [Alíquota de ISS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaalquotasdeiss), do cadastro de [Serviço](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o), esteja definida com a opção **"Materiais"** e o campo **"Percentual de ISS"** possua o valor a ser deduzido.
    

[\[voltar ao topo\]](#top)