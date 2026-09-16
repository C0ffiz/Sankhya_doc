# Tela Tesouraria

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/41837442953239-Tela-Tesouraria](https://ajuda.sankhya.com.br/hc/pt-br/articles/41837442953239-Tela-Tesouraria)

---

# Tela Tesouraria

 **Módulo:** Sankhya Finance  
**Caminho de acesso:** Menu Principal › Sankhya Finance › Tesouraria

**ℹ️ Esta tela está disponível exclusivamente para clientes Sankhya Cloud.**

**Neste artigo**

*   [O que é e para que serve](#h_01KX3VYE869CD4X0JQ9WC1AP3A)
*   [Filtros](#h_01KX3VYE9KNMC8CWRPPPBF79ZR)
*   [Indicadores (KPIs)](#h_01KX3VYEAG763NY26YY5VT6BGB)
*   [Posição Bancária por Conta](#h_01KX3VYEBXQM7GM182FYHVN3QC)
*   [Modal de Conciliação Bancária](#h_01KX3VYEDSC8FPKSA47XZ9B1M1)
*   [Movimentação e Projeção](#h_01KX3VYENRD377T6Z8734T602S)
*   [Pontos de atenção](#h_01KX3VYEPT69DT41MQ0PS4JMPX)

## O que é e para que serve

A tela Tesouraria mostra a posição de caixa em tempo real, a conciliação por conta bancária e a projeção de curto prazo — é a resposta rápida para "qual é a minha posição de caixa agora e há algo errado na conciliação?". O público é o tesoureiro ou analista financeiro operacional, que acessa a tela várias vezes ao dia.

Esta tela não substitui a investigação de um título específico, feita na **Gestão Financeira**, nem a análise de resultado por natureza, feita nas telas de **Receitas**, **Despesas**, **Fluxo de Caixa** e **DRE**. Os dados são lidos direto do Sankhya Om, sem exportar para planilha.

Esta tela é uma das telas do Sankhya Finance; para ver como ela se encaixa no conjunto da solução, consulte o [Guia Sankhya Finance](https://ajuda.sankhya.com.br/hc/pt-br/articles/41301087909655-Guia-Sankhya-Finance).

![Tela Tesouraria com filtros, indicadores e posição bancária por conta](https://ajuda.sankhya.com.br/hc/article_attachments/41837442940567)

_Tela Tesouraria · 07/2026_

**ℹ️ Nota**

A tela é atualizada automaticamente. O topo direito mostra a data e a hora da última atualização e o botão Recarregar página, que força a releitura dos dados.

## Filtros

A tela tem quatro filtros, na barra logo abaixo do título.

*   **Data Negociação** — período (data inicial e final). Recorta os painéis pela data de negociação do título.
    
*   **Data da Baixa** — período (data inicial e final). Recorta os painéis pela data em que o título foi baixado no financeiro.
    
*   **Conta Bancária** — seleção de contas. Afeta todos os painéis da tela.
    
*   **Empresa** — seleção de empresas. Consolida os valores das empresas escolhidas.
    

## Indicadores (KPIs)

Três cards logo abaixo dos filtros resumem a posição consolidada. São a leitura de entrada da tela.

### Saldo Real

Posição consolidada considerando os títulos já baixados no financeiro. O rótulo do card é _"Títulos Baixados no Financeiro"_.

### Saldo do Banco

Posição consolidada considerando apenas os lançamentos já conciliados contra o extrato. O rótulo do card é _"Lançamentos Conciliados"_.

### Diferença

Saldo Real menos Saldo do Banco. Quando há divergência, o card fica em destaque e informa quantas contas divergem — por exemplo, _"4 conta(s) com divergência — verifique antes de conciliar"_. A diferença surge quando um título já foi baixado (entra no Saldo Real) mas ainda não foi conciliado (não entrou no Saldo do Banco).

![Cards de Saldo Real, Saldo do Banco e Diferença](https://ajuda.sankhya.com.br/hc/article_attachments/41837442941207)

_Indicadores — Saldo Real, Saldo do Banco e Diferença · 07/2026_

## Posição Bancária por Conta

Abaixo dos indicadores, a mesma posição é quebrada conta por conta. É onde você identifica em qual conta está a divergência.

Acima dos cards, uma linha-resumo mostra o total de contas, quantas divergem e o valor total em divergência — por exemplo, _"8 contas · 4 divergentes · R$ 1.283.252,02 em divergências"_. No canto direito, os filtros locais Todas, Só Divergentes e Só Conciliadas alternam a exibição dos cards.

### O que cada card mostra

*   Nome da conta / banco e a agência (Ag) com a descrição da conta.
    
*   Saldo Real da conta e Saldo do Banco da conta, lado a lado.
    
*   **Status Divergente** (badge vermelho) — os saldos não batem. O card exibe o valor da diferença e o link Ver Conciliação.
    
*   **Status Conciliado** (badge verde) — os saldos batem. O card exibe a marca _"Saldos conferem"_.
    

![Cards de posição bancária por conta, com status divergente ou conciliado](https://ajuda.sankhya.com.br/hc/article_attachments/41837442944023)

_Posição Bancária por Conta · 07/2026_

**ℹ️ Nota**

As contas divergentes aparecem antes das conciliadas. O link Ver Conciliação abre o modal de conciliação daquela conta — detalhado na seção seguinte.

## Modal de Conciliação Bancária

Abre ao clicar em Ver Conciliação em uma conta divergente. Mostra, no detalhe, os títulos que compõem a diferença daquela conta.

O cabeçalho traz o nome da conta e, abaixo, o período considerado, a agência e a descrição da conta — por exemplo, _"Período: 01/07/2026 a 31/07/2026 · Ag 10001 · TRANSITORIA"_. No topo, os mesmos três indicadores da tela principal, recalculados para a conta: Saldo Real, Saldo do Banco e Diferença.

### Títulos Gerados

A grade lista os títulos da conta. Acima dela há um campo de busca por histórico, número do documento ou número único bancário, e a paginação à direita (por exemplo, _"1-100 de 136"_). As colunas são:

 
| **Coluna** | **O que mostra** |
| --- | --- |
| Nº Único Bancário | Identificador do movimento bancário |
| Tipo de Movimento | Natureza do lançamento — por exemplo, Movimento Bancário |
| Dt. Lançamento | Data em que o lançamento entrou no Saldo Real |
| Nº Documento | Documento do lançamento |
| Vlr. Lançamento | Valor do movimento, com sinal (entrada positiva) |
| Histórico | Descrição do lançamento |
| Dt. Conciliação | Data em que o lançamento entrou no Saldo do Banco. Vazia = ainda não conciliado |
| Conciliado | Situação do lançamento — Pendente (não conciliado) ou conciliado |

### Rodapé de totais

Abaixo da grade, quatro totais consolidam a conta:

 
| **Total** | **O que soma** |
| --- | --- |
| Crédito | Soma das entradas do período |
| Débito | Soma das saídas do período |
| Líquido | Crédito menos Débito |
| Conciliado | Soma dos lançamentos já conciliados — é o que forma o Saldo do Banco |

Quando Líquido é diferente de Conciliado, há lançamento que já entrou no Saldo Real mas ainda não foi conciliado — exatamente a diferença apontada no card da conta.

![Modal de Conciliação Bancária com a grade de títulos gerados e rodapé de totais](https://ajuda.sankhya.com.br/hc/article_attachments/41837442944919)

_Modal de Conciliação Bancária · 07/2026_

## Movimentação e Projeção

Abaixo da posição, três painéis dão a leitura temporal do caixa.

### Evolução do Saldo

Linha do saldo consolidado dos últimos 365 dias. O painel destaca o saldo médio do período — por exemplo, _"Saldo médio R$ -12.498.411.710,76 em 365 dias"_.

![Gráfico de evolução do saldo consolidado nos últimos 365 dias](https://ajuda.sankhya.com.br/hc/article_attachments/41837452234903)

_Evolução do Saldo · 07/2026_

### Concentração Bancária

Distribuição do caixa por banco, em gráfico de rosca com o percentual de cada banco. O alternador Saldo Real / Saldo Banco troca a base do cálculo. No rodapé, o Total Consolidado indica quantos bancos entram e o valor somado — por exemplo, _"Total Consolidado (4 bancos)"_.

![Gráfico de rosca com a concentração bancária por banco](https://ajuda.sankhya.com.br/hc/article_attachments/41837442949015)

_Concentração Bancária · 07/2026_

### Movimentação de Caixa

Entradas e saídas por dia, pela data de baixa. As barras verdes são as Entradas (receitas baixadas no dia) e as vermelhas são as Saídas (despesas baixadas no dia).

![Gráfico de barras com entradas e saídas de caixa por dia](https://ajuda.sankhya.com.br/hc/article_attachments/41837442950039)

_Movimentação de Caixa · 07/2026_

## Pontos de atenção

**Posição em tempo real:** os indicadores (Saldo Real, Saldo do Banco e Diferença) e a Posição Bancária por Conta refletem o momento atual e são atualizados automaticamente. Use o botão Recarregar página para forçar a releitura.

**Tela personalizada:** o rodapé exibe o aviso _"Você está em uma tela personalizada"_, com o link Saiba mais.