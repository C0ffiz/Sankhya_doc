# Tela Gestão Financeira

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/41307904983575-Tela-Gest%C3%A3o-Financeira](https://ajuda.sankhya.com.br/hc/pt-br/articles/41307904983575-Tela-Gest%C3%A3o-Financeira)

---

# Tela Gestão Financeira

**Módulo:** Financeiro  
**Caminho de acesso:** Menu Principal › Sankhya Finance › Gestão Financeira

**Você encontra neste artigo:**

<table class="wysiwyg-table-resized" style="border-collapse: collapse;"><colgroup><col style="width: 50%;"> <col style="width: 50%;"></colgroup><tbody><tr><td style="border-color: #999; padding: 8px; text-align: left; vertical-align: top;"><a href="#oque">O que é e para que serve</a><br><a href="#filtros">Filtros disponíveis</a><br><a href="#cards">Cards de resumo</a><br><a href="#lista">Lista de títulos</a><br>&nbsp;&nbsp;&nbsp;↳ <a href="#botoes">Botões</a><br>&nbsp;&nbsp;&nbsp;↳ <a href="#colunas">Colunas</a></td><td style="border-color: #999; padding: 8px; text-align: left; vertical-align: top;"><a href="#situacoes">Situação dos títulos</a><br><a href="#detalhes">Detalhes do título</a><br><a href="#rateio">Rateio</a></td></tr></tbody></table>

---

## O que é e para que serve

Quando a pergunta é sobre um título específico — qual é a situação, houve renegociação, o valor foi antecipado, como está distribuído entre áreas —, a tela **Gestão Financeira** é o lugar certo. Ela faz parte do **Sankhya Finance** e exibe a lista completa de todos os títulos financeiros da empresa, tanto entradas quanto saídas, com acesso ao detalhe de cada lançamento. É a tela operacional da solução: ideal para consultar, auditar e acompanhar contas a pagar e a receber.

Para ver como esta tela se conecta às demais telas do Sankhya Finance, consulte o [Guia Sankhya Finance](https://ajuda.sankhya.com.br/hc/pt-br/articles/41301087909655-Guia-Sankhya-Finance).

![](https://ajuda.sankhya.com.br/hc/article_attachments/41307904981911)

## Filtros disponíveis

Use os filtros para localizar títulos por empresa, parceiro, situação ou período. Eles podem ser combinados livremente.

| Filtro | O que ele faz |
| --- | --- |
| **Real ou provisão** | Alterna entre títulos reais e provisões |
| **Empresa** | Filtra por empresa |
| **Situação** | Filtra pela situação do título: Aberto, Vencido, Renegociado, Compensado, Baixado, Baixa parcial e Antecipado. Aceita múltipla seleção |
| **Parceiro** | Filtra por cliente ou fornecedor |
| **Data de vencimento** | Período de vencimento dos títulos |
| **Data de negociação** | Período de negociação (lançamento) dos títulos |
| **Data da baixa** | Período da baixa (quitação) dos títulos |

## Cards de resumo

Quatro cards no topo da tela mostram a posição financeira atual e funcionam também como filtros rápidos: clicar em um card filtra a lista para aquela categoria. Clicar novamente volta a exibir todos os títulos.

| Card | Cor | O que mostra | Ao clicar, a lista mostra... |
| --- | --- | --- | --- |
| **Total a Receber** | Verde | Soma das entradas em aberto no período | Todas as receitas em aberto |
| **Recebimentos em Atraso** | Amarelo | Entradas vencidas e ainda não recebidas, com o total de juros acumulados | Todas as receitas vencidas em aberto |
| **Total a Pagar** | Vermelho | Soma das saídas em aberto no período | Todas as despesas em aberto |
| **Pagamentos em Atraso** | Vermelho | Saídas vencidas e ainda não pagas, com o total de juros acumulados | Todas as despesas em aberto atrasadas |

## Lista de títulos

Abaixo dos cards, a lista exibe todos os títulos que atendem aos filtros aplicados. Títulos com rateio exibem um ícone na linha — clicar nesse ícone abre o detalhamento do rateio diretamente, sem precisar abrir o painel de detalhes.

### Botões

| Botão | O que faz |
| --- | --- |
| **Atualizar** | Recarrega os títulos com os filtros atuais |
| **Abrir detalhes** | Abre o painel lateral com os detalhes do título selecionado. Aparece ao selecionar uma linha |

### Colunas da lista

| Coluna | O que mostra |
| --- | --- |
| **Número** | Identificador único do título |
| **Parceiro** | Nome do cliente (entrada) ou fornecedor (saída) |
| **Empresa** | Empresa do lançamento |
| **Categoria** | Categoria financeira do lançamento (ex: Vendas, Energia, Folha de Pagamento) |
| **Tipo de título** | Forma do lançamento: Boleto, Cheque, Pix, TED, Dinheiro, Cartão, Crédito, etc. |
| **Data de negociação** | Data em que o lançamento foi registrado |
| **Data de vencimento** | Data de vencimento do título |
| **Valor original** | Valor bruto do lançamento, sem acréscimos ou deduções |
| **Valor líquido** | Valor final — com juros, multas e descontos aplicados |
| **Situação** | Situação atual do título. Ver [Situação dos títulos](#situacoes) |
| **Conciliado** | Indica se o lançamento foi conferido com o extrato bancário |

## Situação dos títulos

Cada título exibe um indicador colorido com sua situação atual, calculada automaticamente pelo sistema. Entender o significado de cada situação ajuda a interpretar a lista e priorizar ações.

| Situação | O que significa |
| --- | --- |
| **Antecipado** | O título foi antecipado junto a um banco antes do vencimento |
| **Renegociado** | O título original foi substituído por um novo acordo de prazo ou valor |
| **Compensado** | O título foi quitado por compensação com outro lançamento de natureza oposta |
| **Baixa parcial** | Parte do valor foi paga ou recebida — ainda há saldo pendente |
| **Pago / Recebido** | Valor integralmente quitado |
| **Vencido** | O prazo passou e o título ainda não foi baixado |
| **Aberto** | Dentro do prazo, aguardando pagamento ou recebimento |
| **Baixado** | Título com baixa registrada no financeiro |
| **Provisão** | Lançamento provisionado, ainda não confirmado como título real |

## Detalhes do título

O detalhe do título não é uma janela modal: é um painel lateral que abre à direita da tela ao selecionar uma linha e clicar em **Abrir detalhes**. O painel exibe todas as informações do lançamento — e o conteúdo varia conforme a situação do título: somente as seções aplicáveis são exibidas.

![](https://ajuda.sankhya.com.br/hc/article_attachments/41307872640407)

**Renegociação**  `Título renegociado`

Exibe a cadeia completa de renegociação: o título original e os títulos que foram gerados a partir daquela renegociação.

**Antecipação**  `Título antecipado`

Exibe o número do acerto, a data e o usuário responsável, os encargos da antecipação bancária (juros e encargos, IOF, obrigação com banco) e os cards de **Valor total**, **Valor líquido recebido** e **Desconto total**. Inclui também a tabela **Títulos gerados**, que lista cada título criado na operação — tipo de referência (título original, antecipação, obrigação, juros e encargos, IOF), número, valor e data de negociação.

**Compensação**  `Título compensado`

Exibe o registro de compensação com as entradas e saídas envolvidas. Quando há diferença entre os totais, aparece também o saldo pendente.

**Baixa Parcial**  `Título com pagamento parcial`

Exibe as parcelas já quitadas e o saldo que ainda está em aberto.

**Baixado**  `Título totalmente quitado`

Exibe os dados da quitação: data do acerto, usuário responsável, valor baixado, descontos aplicados e valor atualizado.

## Rateio

Títulos com rateio exibem um ícone diretamente na linha da lista. Clicar nesse ícone abre uma janela com a divisão proporcional do lançamento — sem precisar abrir o painel de detalhes. Para cada parte do rateio são exibidos: valor, percentual, Centro de Resultado, categoria, projeto, parceiro e data de alteração.

Relativo a

*   [sankhyafinance](https://ajuda.sankhya.com.br/hc/pt-br/search?content_tags=01KVBPQS4F0A9FYX0DRX3B56B1&utf8=%E2%9C%93 "Resultados da pesquisa")