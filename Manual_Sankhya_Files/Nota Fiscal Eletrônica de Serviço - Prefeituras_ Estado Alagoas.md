# Nota Fiscal Eletrônica de Serviço - Prefeituras: Estado Alagoas

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/22531157152791-Nota-Fiscal-Eletr%C3%B4nica-de-Servi%C3%A7o-Prefeituras-Estado-Alagoas](https://ajuda.sankhya.com.br/hc/pt-br/articles/22531157152791-Nota-Fiscal-Eletr%C3%B4nica-de-Servi%C3%A7o-Prefeituras-Estado-Alagoas)

---

# Nota Fiscal Eletrônica de Serviço - Prefeituras: Estado Alagoas

Neste artigo serão apresentadas as especificações de emissão de NFS-e das cidades localizadas no estado de Alagoas, para conhecê-las acesse os links abaixo:

<table style="border-collapse: collapse;"><tbody><tr><td style="width: 100%;" colspan="2"><h4 class="wysiwyg-text-align-center" id="h_01HTJ1DMWGE480H6RYB8HF9D2Z"><span style="color: #4D4D4D;"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;"><strong>Cidades</strong></span><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif;"><strong>&nbsp;</strong></span></span></h4></td></tr><tr><td style="width: 50%;"><a href="#Arapiraca/AL"><span style="color: #4D4D4D;">Arapiraca/AL</span></a></td><td style="width: 50%;"><a href="#Macei%C3%B3/AL"><span style="color: #4D4D4D;">Maceió/AL</span></a></td></tr><tr><td><a href="#h_01KX3RHXQ3TDEGFCY1PG4JN3D8">São Sebastião/AL</a></td><td>&nbsp;</td></tr></tbody></table>

### **Arapiraca/AL**

O sistema encontra-se apto para emitir NFS-e para o município de Arapiraca.

**Observação:** a cidade não suporta o cancelamento de nota de serviço via webservice, este deverá ser feito diretamente na prefeitura.

[\[voltar ao topo\]](#top)

### **Maceió/AL**

O sistema encontra-se apto para emitir NFS-e para o município de Maceió.

**Observação:** a cidade não suporta o cancelamento de nota de serviço via webservice, este deverá ser feito diretamente na prefeitura.

[\[voltar ao topo\]](#top)

### **São Sebastião/AL**

O município de São Sebastião/AL utiliza um **Sistema Próprio Municipal** para as Notas Fiscais de Serviço (NFS-e), e a emissão foi homologada de forma automatizada por meio da integração via webservice.

Esta homologação já contempla a adequação aos novos impostos da Reforma Tributária (**IBS e CBS**). Para garantir que suas notas sejam emitidas e aprovadas sem erros, siga o passo a passo de configuração abaixo:

*   **Cadastros Básicos**
    *   [**Cidades**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades)**:** na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral),  preencha o **"Mun. domicílio fiscal"** com o código IBGE **2708305**.
    *   [**Empresa**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa)**:** confirme se a **"Inscrição Municipal"** da sua empresa está devidamente preenchida.
*   **Configurações do Serviço:** acesse o cadastro de  [Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o) (abas [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaimpostos) e [Alíquotas de ISS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o#abaalquotasdeiss)) e revise:
    *   **Código de Serviço Municipal:** preencha o campo **"Cód. Trib. Município"** com a formatação exigida pela prefeitura. Exemplo: **140101**.
    *   **Preenchimento obrigatório:** não esqueça de informar o **"Item da Lista de Serviços (LC 116)"** (ex: 1401), o **"Código CNAE"** (ex: 4520001) e o **"Código NBS"** (ex: 120024000, conforme a tabela oficial da Nomenclatura Brasileira de Serviços).
*   **Configuração para IBS e CBS (Reforma Tributária)** Para que os novos impostos sejam calculados e enviados corretamente ao portal da prefeitura:
    *   **Cadastro de** [Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o)**:** na [aba Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abaimpostos), [seção Reforma Tributária](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#01K56TN2K88BREGGCND4D6DBNF), preencha o campo **"Código Classificação Tributária Nacional"** (ex: 140101). Configure também as alíquotas de IBS e CBS pertinentes ao serviço.
    *   [**Tipos de Operação (TOP)**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP)**:** na [aba Reforma Tributária](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#01K56TN2K88BREGGCND4D6DBNF), certifique-se de ativar as marcações **"Tem CBS"** e **"Tem IBS"**.
*   **Regras de Emissão e Particularidades**
    *   **Reduções de Base:** a prefeitura só aceita notas com redução na base de cálculo do ISS (ex: 40%) caso exista um **benefício fiscal válido atrelado à operação**. Tentativas de redução sem amparo legal resultarão em rejeição do documento.

[\[voltar ao topo\]](#top)