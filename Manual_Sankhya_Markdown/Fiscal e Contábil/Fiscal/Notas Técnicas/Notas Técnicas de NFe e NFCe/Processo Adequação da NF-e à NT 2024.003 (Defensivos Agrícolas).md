# Processo Adequação da NF-e à NT 2024.003 (Defensivos Agrícolas)

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/42732990867479-Processo-Adequa%C3%A7%C3%A3o-da-NF-e-%C3%A0-NT-2024-003-Defensivos-Agr%C3%ADcolas](https://ajuda.sankhya.com.br/hc/pt-br/articles/42732990867479-Processo-Adequa%C3%A7%C3%A3o-da-NF-e-%C3%A0-NT-2024-003-Defensivos-Agr%C3%ADcolas)

---

# Processo Adequação da NF-e à NT 2024.003 (Defensivos Agrícolas)

**Módulo:** Fiscal e Contábil › Documentos Eletrônicos  
**Caminho de acesso:** Menu Principal › Preferências › Empresa › aba NF-e/NFC-e › sub-aba Nota Técnica NF-e

---

**Você encontra neste artigo:**

<table class="wysiwyg-table-resized"><colgroup><col style="width: 50%;"><col style="width: 50%;"></colgroup><tbody><tr><td><p>&nbsp;&nbsp;↳&nbsp;<a href="#h_01M00ZB3SKA7W4YHPM2M341Y1V"><span class="wysiwyg-underline">O que é e para que serve</span></a></p><p>&nbsp;&nbsp;↳&nbsp;<a href="#h_01M00ZB3SNHEYW17CW184WME3R"><span class="wysiwyg-underline">v1.01 — NCM de defensivos agrícolas e animais vivos</span></a></p></td><td><p>&nbsp;&nbsp;↳&nbsp;<a href="#h_01M00ZB3T3FA7BGP5X76M86SC7"><span class="wysiwyg-underline">v1.03 — Grade Defensivos Agrícolas no layout</span></a></p><p>&nbsp;&nbsp;↳&nbsp;<a href="#h_01M00ZBKS340BPBYQBHCC5R8V1"><span class="wysiwyg-underline">Pontos de atenção</span></a></p></td></tr></tbody></table>

## **O que é e para que serve**

A **Nota Técnica 2024.003** adequa a emissão de NF-e que envolvem itens classificados como defensivos agrícolas ou animais vivos, exigindo validações de NCM/CFOP e a inclusão de informações complementares no XML. Este artigo cobre as duas versões já disponíveis nas Preferências da Empresa — v1.01 e v1.03 — e não substitui a validação da classificação fiscal do produto, que continua sendo responsabilidade do cadastro de cada item.

## **v1.01 — NCM de defensivos agrícolas e animais vivos**

Ao emitir e validar notas fiscais com a versão v1.01 ativa, contendo itens classificados como defensivos agrícolas, você deve garantir que o **NCM** do item esteja de acordo com a regra estabelecida. Após a emissão, valide o XML gerado e confira se as tags referentes ao **Número da Receita** e ao **CPF do Responsável Técnico**, no Configurador de Layout da Nota, foram preenchidas corretamente.

Para produtos classificados como animais vivos, o NCM e o CFOP também precisam estar adequados às regras aplicáveis. Após gerar a nota, valide o XML e revise as tags de **Tipo de Guia**, **UF de Emissão**, **Série da Guia** e **Número da Guia**, também no Configurador de Layout da Nota, para evitar inconsistências ou rejeições.

<table style="background-color: #E6F4EE; border-color: #006B3F;"><tbody><tr><td style="background-color: #E6F4EE; border-color: #006B3F;"><p><span style="color: #0c447c;"><strong>ℹ️ Nota</strong></span></p><p>A quantidade de defensivos agrícolas enviada no XML depende de quais NTs estão ativas: com a NT 2024.003 v1.01 e a NT 2023.001 ativas juntas, o sistema envia até 20 defensivos agrícolas no XML. Com apenas a NT 2024.003 v1.01 ativa, é enviado apenas 1 defensivo agrícola, mesmo que o cadastro tenha mais de um item informado.</p></td></tr></tbody></table>

## **v1.03 — Grade Defensivos Agrícolas no layout**

Com a versão v1.03 ativa, você pode informar dados de defensivos agrícolas diretamente na NF-e. Para isso, ative a NT nesta tela e, no Configurador de Layout da Nota, adicione a grade **Defensivos Agrícolas** no rodapé do layout de Venda.

O preenchimento das tags segue esta correspondência: a tag <nRec> usa o valor do campo **Número da receita ou receituário do agrotóxico/defensivo agrícola** (até 30 caracteres), e a tag <CPF> usa o valor do campo **CPF do Responsável Técnico, emitente do receituário** (11 números válidos, com validação de CPF).

<table style="background-color: #E6F4EE; border-color: #006B3F; margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #E6F4EE; border-color: #006B3F;"><p><span style="color: #0c447c;"><strong>ℹ️ Nota</strong></span></p><p>A mesma regra de quantidade da v1.01 se aplica aqui: até 20 defensivos agrícolas com a NT 2023.001 também ativa, ou apenas 1 sem ela.</p></td></tr></tbody></table>

## **Pontos de atenção**

O limite de defensivos agrícolas enviados no XML (1 ou até 20) depende da combinação de NTs ativas nas Preferências da Empresa, e não apenas da versão da NT 2024.003 selecionada. Confira se a NT 2023.001 também precisa estar ativa para o seu cenário antes de cadastrar mais de um defensivo agrícola por item.