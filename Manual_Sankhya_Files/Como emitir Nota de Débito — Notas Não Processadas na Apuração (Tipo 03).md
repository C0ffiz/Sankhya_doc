# Como emitir Nota de Débito — Notas Não Processadas na Apuração (Tipo 03)

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/40099828273687-Como-emitir-Nota-de-D%C3%A9bito-Notas-N%C3%A3o-Processadas-na-Apura%C3%A7%C3%A3o-Tipo-03](https://ajuda.sankhya.com.br/hc/pt-br/articles/40099828273687-Como-emitir-Nota-de-D%C3%A9bito-Notas-N%C3%A3o-Processadas-na-Apura%C3%A7%C3%A3o-Tipo-03)

---

# Como emitir Nota de Débito — Notas Não Processadas na Apuração (Tipo 03)

**Módulo:** Comercial › Rotinas

**Caminho de acesso:** `Menu Principal › Comercial › Rotinas › Portal de Vendas`

---

## O que é e para que serve

Use a Nota Fiscal de Débito (Tipo 03) quando identificar, após a prévia da apuração assistida pelo Comitê Gestor do IBS (CG-IBS), que documentos fiscais que você emitiu não foram reconhecidos pelo sistema. Emitir esta nota garante que o saldo final do período reflita os débitos corretos, evitando que você sofra multas e juros futuros.

Esta nota produz efeitos apenas na sua apuração e não gera créditos automáticos para os clientes.

## Antes de começar

Verifique a integridade das informações na prévia da apuração assistida e configure o [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP) e a tributação.

### Configuração do Tipo de Operação (TOP)

Acesse o Cadastro de [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP) e configure:

*   **Tipo de Movimento:** selecione V (Venda).
*   [**Aba Financeiro**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abafinanceiro) **e** [**Aba Estoque**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abaestoque)**:** selecione Não atualizar e Nenhum, respectivamente.
*   [**Aba Livro Fiscal**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abalivrofiscal)**:** no campo **Atualização de Livro ICMS**, selecione Livro de Saída. Informe os CFOPs `5949` ou `6949`.
*   [**Aba Impostos**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abaimpostos)**:** marque as opções **Tem CBS** e **Tem IBS na seção** [**Reforma Tributária**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#01K56TN2K88BREGGCND4D6DBNF).
*   [**Aba NF-e / NFC-e / CF-e**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abanfe/nfce/cfe)**:** em **NF-e**, selecione 6 - Nota de Débito. Em **Tipo de Nota de Débito**, selecione 03 - Débitos de notas fiscais não processadas na apuração. Marque a opção **Buscar NF de origem p/referenciar na NFe** para que os documentos relacionados sejam gerados corretamente no XML do DFe.

### Configuração da Tributação (IBS e CBS)

Acesse as telas de [Alíquotas de IBS](https://ajuda.sankhya.com.br/hc/pt-br/articles/33820442146199-Cadastro-de-Al%C3%ADquotas-IBS-Reforma-Tribut%C3%A1ria) e [Alíquotas CBS](https://ajuda.sankhya.com.br/hc/pt-br/articles/33822014543895-Cadastro-de-Al%C3%ADquotas-CBS-Reforma-Tribut%C3%A1ria) e configure a exceção de imposto com os seguintes parâmetros:

*   **CST:** 811
*   **Classificação Tributária (cClassTrib):** 811002
*   **Alíquotas:** informe as vigentes.

## Como emitir a nota

1.  Acesse o [**Portal de Vendas**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612654-Portal-de-Vendas).
2.  Utilize os filtros para localizar as notas não processadas pela apuração.
3.  Selecione as notas que receberão o ajuste.
4.  Clique Grade de Itens > [**Outras Opções**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612374-Central-de-Vendas-Grade-Itens-Bot%C3%A3o-Outras-Op%C3%A7%C3%B5es) › **Emissão de notas de ajuste e Complemento** › **Emitir nota de Débito**.
5.  No pop-up, selecione a TOP configurada.
6.  Selecione os itens a serem considerados (cada item corresponderá a um documento fiscal não processado).
7.  Confirme se a sua empresa e o destinatário estão exatamente iguais à nota original.
8.  Salve a nota.

<table style="background-color: #E6F4EE; border-color: #006B3F; margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #E6F4EE; border-color: #006B3F;"><p><strong>Dica</strong></p><p>O sistema recupera os impostos do documento de origem automaticamente. A data do documento referenciado é utilizada para informar o ajuste de competência de forma automática.</p></td></tr></tbody></table>

<table style="background-color: #E6F1FB; border-color: #185FA5; margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #E6F1FB; border-color: #185FA5;"><p><strong>Nota</strong></p><p>O crédito do cliente só será liberado após o efetivo processamento da nota original pelo sistema do Comitê Gestor.</p></td></tr></tbody></table>

## Pontos de atenção

### Estrutura do XML

Para validação correta, o XML conterá obrigatoriamente os grupos Ajuste de Competência (`gAjusteCompet`) e Documento Fiscal Eletrônico Referenciado (`DFeReferenciado`):

```auto

<ide>
    <finNFe>6</finNFe>
    <tpNFDebito>03</tpNFDebito>
</ide>
<det nItem="1">
    <imposto>
        <IBSCBS>
            <CST>811</CST>
            <cClassTrib>811002</cClassTrib>
            <gAjusteCompet>
                <competApur>xxxx-xx</competApur>
                <vIBS>x.xx</vIBS>
                <vCBS>x.xx</vCBS>
            </gAjusteCompet>
        </IBSCBS>
    </imposto>
    <DFeReferenciado>
        <chaveAcesso>44-CHAVE-DA-NOTA-ORIGINAL-NAO-PROCESSADA-44</chaveAcesso>
    </DFeReferenciado>
</det>
```