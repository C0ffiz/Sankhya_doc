# Tela Fluxo de Caixa

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/41307193691927-Tela-Fluxo-de-Caixa](https://ajuda.sankhya.com.br/hc/pt-br/articles/41307193691927-Tela-Fluxo-de-Caixa)

---

# Tela Fluxo de Caixa

**Neste artigo**

*   [O que é e para que serve](#oque)
*   [Filtros principais](#filtros)
*   [Filtros avançados](#filtros-avancados)
*   [Indicadores (KPIs)](#kpis)
*   [Os sete gráficos](#graficos)
*   [Fluxo Projetado](#projetado)
*   [Análise de vencimentos (Aging)](#aging)
*   [Detalhe ao clicar nos gráficos](#detalhe)

**Módulo:** Financeiro  
**Caminho de acesso:** Menu Principal › Sankhya Finance › Fluxo de Caixa

---

## O que é e para que serve

Quando a pergunta é sobre a saúde do caixa — quanto há a receber, quanto há a pagar, qual banco concentra mais saldo e se há vencimentos se acumulando —, a tela **Fluxo de Caixa** é o lugar certo. Ela faz parte do **Sankhya Finance** e oferece uma visão integrada das entradas e saídas financeiras, reunindo sete gráficos com perspectivas diferentes sobre o fluxo financeiro: por período, por categoria, por prazo de vencimento e por banco. Ela não realiza lançamentos nem permite editar títulos.

Para ver como esta tela se conecta às demais telas do Sankhya Finance, consulte o [Guia Sankhya Finance](https://ajuda.sankhya.com.br/hc/pt-br/articles/41301087909655-Guia-Sankhya-Finance).

![](https://ajuda.sankhya.com.br/hc/article_attachments/41307193680791)

## Filtros principais

A barra no topo define o escopo da análise. Todos os gráficos e indicadores respondem simultaneamente a qualquer alteração feita aqui.

| Filtro | O que ele faz |
| --- | --- |
| **Período** | Intervalo de datas analisado |
| **Arquivo DRE** | Modelo de DRE usado para calcular os indicadores do topo da tela. Por padrão, o primeiro arquivo disponível  
![](https://ajuda.sankhya.com.br/hc/article_attachments/42315428804247) |
| **Contas bancárias** | Filtra por conta específica. Em branco = todas as contas ativas |
| **Empresa** | Filtra por empresa |
| **Naturezas** | Filtra por categoria financeira |
| **Centro de custo** | Filtra por área ou departamento |

## Filtros avançados

Para um controle mais preciso sobre o que entra na análise, o botão **Filtros avançados** abre opções adicionais divididas em dois grupos: o que incluir nos cálculos e como calcular.

### O que incluir

Defina quais tipos de lançamento devem aparecer nos gráficos e indicadores:

| Opção | O que inclui |
| --- | --- |
| **Recebidos** | Entradas já efetivadas |
| **Pagos** | Saídas já efetivadas |
| **A receber** | Entradas ainda não efetivadas |
| **A pagar** | Saídas ainda não efetivadas |
| **Previstos** | Lançamentos previstos, ainda não confirmados |
| **Saldo inicial** | Saldo das contas bancárias no início do período |

**⚠️ Atenção**

Ao menos uma opção precisa estar marcada para que os dados sejam exibidos.

### Opções de cálculo

Além de definir o que incluir, é possível ajustar como os valores são calculados:

| Opção | Efeito |
| --- | --- |
| **Incluir contas inativas** | Considera também contas bancárias desativadas |
| **Desconsiderar antecipação** | Exclui lançamentos que passaram por antecipação bancária |
| **Considerar float** | Aplica a carência em dias configurada no Tipo de Título: o sistema considera o vencimento do título somado aos dias de float. Ex.: tipo de título com float de 30 dias → vencimento + 30 dias |
| **Valores líquidos** | Usa o valor final (com acréscimos e deduções) no lugar do valor bruto |

## Indicadores (KPIs)

Quatro cards no topo da tela resumem o resultado do período filtrado. Os indicadores são os totalizadores do arquivo DRE selecionado no filtro — por isso os nomes e valores seguem o modelo de DRE da empresa. No modelo padrão são exibidos:

![](https://ajuda.sankhya.com.br/hc/article_attachments/41307181185815)

| Indicador | O que mostra |
| --- | --- |
| **Lucro Bruto** | Receitas menos despesas diretamente ligadas à operação no período |
| **Lucro Líquido** | Resultado final do período — todas as entradas menos todas as saídas |
| **EBITDA** | Resultado operacional antes de juros, impostos, depreciação e amortização |
| **Resultado Operacional** | Resultado das atividades operacionais da empresa no período |

**ℹ️ Nota**

Cada card mostra também a variação percentual em relação ao mesmo período do ano anterior. Os nomes dos indicadores podem variar conforme a estrutura de DRE configurada pelo administrador.

## Os sete gráficos

Abaixo dos indicadores, a tela exibe sete gráficos que cobrem diferentes ângulos do fluxo financeiro. Três deles — **Valor Líquido por Mês**, **Receitas × Despesas por Mês** e **Fluxo por Categoria** — permitem clicar nas barras para abrir o detalhe dos lançamentos. Os demais são apenas visuais.

**ℹ️ Nota**

Os gráficos desta tela independem do **Arquivo DRE** selecionado no filtro. Apenas os indicadores do topo (KPIs) seguem o modelo de DRE configurado.

| Gráfico | Tipo | Detalhe ao clicar | O que mostra |
| --- | --- | --- | --- |
| **Valor Líquido por Mês** | Barras | Sim | Saldo mensal (entradas menos saídas). Positivo = superávit; negativo = déficit |
| **Receitas × Despesas por Mês** | Barras duplas | Sim | Entradas e saídas comparadas lado a lado por mês |
| **Fluxo por Natureza** | Barras | Sim | Entradas e saídas por categoria financeira, com rateio aplicado |
| **Vencimentos (Aging)** | Barras duplas | Sim | Quanto há a receber e a pagar em cada faixa de prazo. Ver [Análise de vencimentos](#aging) |
| **Fluxo por Categoria Mensal** | Linhas | Não | Evolução mensal de cada categoria ao longo do período |
| **Saldo Mensal** | Barras + linha | Não | Barras de entradas/saídas com linha de saldo real das contas bancárias |
| **Distribuição por Banco** | Pizza | Sim | Participação de cada banco no saldo total de caixa |

Veja abaixo o que cada gráfico mostra, como lê-lo e que decisão ele apoia.

**Valor Líquido por Mês**

**O que mostra:** o resultado de cada mês (entradas menos saídas), em barras que sobem para o positivo e descem para o negativo.

**Como ler:** barra para cima é mês com resultado positivo (entrou mais do que saiu); barra para baixo é mês negativo (saiu mais do que entrou).

**Para que serve:** ver rapidamente em quais meses o caixa sobrou e em quais faltou, antes de entrar no detalhe.  
![Exibindo image.png](https://chat.google.com/u/0/api/get_attachment_url?url_type=FIFE_URL&content_type=image%2Fpng&attachment_token=AOo0EEWo7RDFBQs0FLDA6ahX4g5Io5OQ%2B9CtZYy9okMZO48tFyhLVSHBzhQptb31m613nhK3I3u3wiMQ1dp847SY11%2FQ0X6AF%2FdWksEsoD05NAM0lQ9hqQ50FKJ0BJltRz%2Fq8doUIybA91aaYyzDHxR5WagAIxWoS7b%2FEJLvoh2ZK97DcXJZjY0I8DKxosCSj9OVGt%2Fm8JfASP5yAd1ewn9d1Pvo2loamWdtVY89CVey87ismeum%2BXuVIgMO9dVh%2FJ1d7Kg2hJ1adeQCkfe%2BhGxlIsPn%2B5EOz0ER%2FJ292e1RhOe9hwqziKBmPEntzsES8vhYaoLa3Nl2y7F%2BMljUoCTYLY67IfsRikHXBy4LyKrDKjIeFYTkAmMDc9mQkwsUEWw9jKlKF%2FKuZ3WlLjDF559YeGaqDUTklzxoXaiA%2BsZYEIS%2FJkWgvsgdWwjBKsMUsscJ8ZhH8H8hrNL3ihSQhCoX3T6vaKpjoTSQCDlcy4BX0d4zmMDLsbCwSk8mLmBEkQK7qALTX%2B7n2CUqe9s8zN4dHOVUQw4Nlhz2QP6IsuFisCPjjqFfJYCUra43Wnjj2O4bXpnXIwyaLfWqD5l5%2Bcwa4jL43MzpMtGReOk4bTRZr7KhOiwGJIvVYlvdCYZs8eqZAKth&allow_caching=true&sz=w1920-h945-rw&auditContext=forDisplay)

**Receitas × Despesas por Mês**

**O que mostra:** as entradas e as saídas de cada mês, lado a lado (entradas em verde, saídas em vermelho).

**Como ler:** para cada mês há duas barras — uma de entradas e uma de saídas. A diferença visual entre elas mostra a folga ou o aperto do mês.

**Para que serve:** comparar o ritmo de recebimentos e pagamentos mês a mês e antecipar meses em que as saídas superam as entradas.  
  
![Exibindo image.png](https://chat.google.com/u/0/api/get_attachment_url?url_type=FIFE_URL&content_type=image%2Fpng&attachment_token=AOo0EEXiSYg%2FDQccdxV6q21HUn3kQitk7k%2FVgd9bthlb1GeJcxs1vNygalCfEmJwJQhy19FPd6di9gW8fbC%2B%2FbxkWNt6nHbsVmdJOVJuKxiXHmwAT%2F6YaclnVz3gqjhHY1MHcriIck0FxMFvqCjZOkYIlULuYpNvl9jOS2%2BuD0SgpJsSedPjYA6NtlsmNp3EuWxhTuziA%2FvXYv%2BgU1y2sy6uSzwCoV4V2QTL1Mn4KFN3PTYkOvjYr%2FzXuwpGlP%2FiU%2FRE8zKe%2BgSW3Ft5NCVxl9h2gZhnrhNPSEBhM0atWDkugHLyqBRMyYGHzASb2VAciEUlAVm5R9jZnSOJeGtoSfpih9aNboDhQ3kqQvZpTUZ7P8cxdXFJwHeHY9KKV9D10cgSE5NGhgbBy28MM3gh6UZxV%2B8KE%2F%2F1qeA76jzUJidUvNk9XzzIMBr6y%2BOvG5dlDlETsIvosSnCIq6zBxqd0wU3ODJhj5TPY1C6aLnszBPfyGUi2uwA9Y%2F2Zd9HF5e8%2BjDXfFXfxtpANfjy5CtZ3l20htnz4xXM6AwPG2QmZSvRYT4BRwpy5MO7XHopvYl03DDd54d14IpKKO4bEduw8EKrQoxdemt9vMSQxbs8E3DIbAvEQd7ldUb6kFWNyNhrQJ3L6IA%3D&allow_caching=true&sz=w1920-h945-rw&auditContext=forDisplay)

**Fluxo por Natureza**

**O que mostra:** o total movimentado por natureza no período, em barras horizontais (entradas e saídas por classificação).

**Como ler:** cada barra é uma natureza — o tamanho indica o volume movimentado naquela classificação.

**Para que serve:** identificar as naturezas que mais movimentam o caixa, tanto do lado das entradas quanto das saídas.  
  
![Exibindo image.png](https://chat.google.com/u/0/api/get_attachment_url?url_type=FIFE_URL&content_type=image%2Fpng&attachment_token=AOo0EEWNUFA6JReF%2BWrKM98DPuuyZl9EgVgQp1txFKJ%2F7MhiEmq2nq9pDI04Av64BUEi33kOvmdmQ2sNZWS2KYZ0DOUcSrTvIn%2Bsk775ZTE5LirT1POU62HCyb7U6G5JPBvWloVm1L68dMz8ZFv5YtNgt8JP27I1mFnQZeKmXLFsNNqCaPZ1489NZ8S6zDI6NIXECV62FOFxTUyGW31iJJXSk7s104pBVk6YwFgvu8VvbuxTg1GmkprC%2B8ppR6rS2atjpHO9ZN37NkBexC8vcbeykjEw6pgLCUDnP9YB4o78phREJMK8hMiFtok2bF1PGDewaBuwv5YKEuGS5qGZ%2Bfq5609lki63QPGFlFU1R5W91hXFey0WmkaSQkzchU1vZBMD7GIAuaJLkbjWhDKIj1gIDwz1D8sCWeeaqHqUP4snN42IQV%2BLn5j%2B4dAGFFhtMRqAM9R6bPFX6chG3yd5cw8hYHESgq8zDMIO1GbXxsKPvEyOuUXAgUr1Fo8EmFGUDRqH60t1IJIgVBcmtETtwMvmM4A2SK1zEbEF0cSQgq8OCDw2PHXI2NWS9C7AbxyeAJX9eggSkZodQpW0N4PHjXkDm3IGVFiUdYR3GuoiE75LbLzn0zuA%2FJeXe8BXUeXo%2F7gcbmM%3D&allow_caching=true&sz=w1920-h945-rw&auditContext=forDisplay)

**Vencimentos (Aging)**

**O que mostra:** os valores a receber e a pagar (títulos em aberto) distribuídos por faixa de vencimento.

**Como ler:** cada grupo de barras é uma faixa de prazo — em cada faixa, uma barra de recebimentos e uma de pagamentos. Quanto mais valor nas faixas vencidas (a partir de 1–30 dias), maior a atenção.

**Para que serve:** priorizar cobrança e programar pagamentos — ver o que está a vencer e, principalmente, o que já está vencido e há quanto tempo.  
  
![Exibindo image.png](https://chat.google.com/u/0/api/get_attachment_url?url_type=FIFE_URL&content_type=image%2Fpng&attachment_token=AOo0EEVbzFXmtaCm7CiACo%2B3KKJqa28EL5vYHMLrD%2B29AffM0gsWOytst1qfMnsUjzbJifD6VGDnaTGYYSXZWmi1wwhlOYNYT%2F6ky41ZThARt3PAn19t7DRqK11fKdqFZrxmjL7OwHtKrRdcyedpRDk22hg0dRcafXnIQnUTnUKsQXfVI6Zlxg5ZBNpJjCssDcNRiqDtcD%2FgbvBfJH3SeVWEDK1D9rdybk0MMHv%2FeEKpEyePI5vmSfILYU7ON3YS2rekxZU5xPpIMaSPtRjkc7KWjAqgxP%2F0kO6xBgQzrg3%2BxR%2Bnv6Fgy0yeFYYmne8h9ruZqfLqaw6lpQKCFSUm3wALXhTBbVmHq5RmUo20rTOw9BNgtmnQwpTyE3GzcStHXtGEXc09Pf%2B7TwoHGpi6Tgyt2ZJPXnrUlxdaKj%2F9ODGgy1RK35hTRU1Ag82gZwQe7s7sfFhgwkqmtFBIoLw2bDvulh7sGldp%2Bu6yBybtM%2BaSOlFKYSdtrseronV4zqlEIPLNN9sUzFtrmKetNA8GArXvaiW%2BWAeAsc5oJsqHNTa4g59aDUAD5eYKpHDLfop3dj4FOPh5UWdXUVyQxqgtrsaoZSOvNvrJ5N8ULoP0pJYVTQx5cIKJEd%2FoPqyWEE3mBE8w%2FtTl&allow_caching=true&sz=w1920-h945-rw&auditContext=forDisplay)

**ℹ️ Nota**

Este gráfico considera apenas títulos em aberto (ainda não recebidos nem pagos). Para entender cada faixa, consulte a seção [Análise de vencimentos](#aging) abaixo.

**Fluxo por Categoria Mensal**

**O que mostra:** a evolução mês a mês das principais naturezas, em linhas (uma linha por natureza).

**Como ler:** cada linha acompanha uma natureza ao longo dos meses — a posição acima ou abaixo de zero mostra se aquela natureza somou ou consumiu caixa no mês.

**Para que serve:** acompanhar a tendência de cada categoria ao longo do tempo e perceber qual natureza está puxando o resultado para cima ou para baixo.  
![Exibindo image.png](https://chat.google.com/u/0/api/get_attachment_url?url_type=FIFE_URL&content_type=image%2Fpng&attachment_token=AOo0EEWlWrT2s%2FnleosVPw6dVq4XO%2FIyj5Rkh%2BMmfKXCibyh6d39hLpA3aIZPTWWxlAYjrZKI%2BreuJVhnWzz%2FAi1oq9m3R5T%2BWHYf1MDvnsd7Bk5QAKdR4fmsUlBV56VJjulNWYpTRuVzq6r1MC%2F8DyCWXxHV0w325l05i0TDwN0zlAepkMpqSMDDXuTHBvUCptHLzDndq8%2FY0d48pPwtp64sgzH1Jp7UWaQcT0mJ0rmVWQ7261%2FABsi8%2Blypf4vEreBCHBmHGoiZQXclQLLg9hPGgIrRlYnB%2Ba7pUV9vtUCBtxwuKmHWd44%2F95Ce0gu2H3GoioGa278IjUDj%2BbtLdkraaU%2Fvg5o9MVMTSHvaNpm9nzjZMghGP5KHT%2FCTn7fsPgov3uAr5pVvZtWgtdMP6%2BJtzkQXGfU1t%2FmTzHP3C2NUsmeDjv7qyVqvfbjo8Alm06iuPn4L6x9iJhhJjkN6ptIApNRqtuQ1qWPvn3QWSsCHyb35Roakram44UeKIAC%2FRZih3DtcYvrjsMt%2F6ys1Iq53rG34gtqDr6s8B6BZoOwnlwoidQ%2Fff0W3v3DNcedH8C7sRZq2gF2aSBK7oLkKNbJ%2BKq0FhINyXvvGO5VI9GDuQZFTcxzHJno%2FQ%2FklJY6SbFws5xo&allow_caching=true&sz=w1920-h945-rw&auditContext=forDisplay)

**Saldo Mensal**

**O que mostra:** as entradas e as saídas de cada mês em barras, com uma linha de saldo acompanhando a evolução.

**Como ler:** as barras mostram entradas e saídas do mês; a linha mostra o saldo. A linha subindo indica caixa se recompondo; descendo, caixa se deteriorando.

**Para que serve:** ter, num só gráfico, a leitura do mês (barras) e a trajetória do saldo (linha) — útil para enxergar recuperação ou piora ao longo do período.  
  
![Exibindo image.png](https://chat.google.com/u/0/api/get_attachment_url?url_type=FIFE_URL&content_type=image%2Fpng&attachment_token=AOo0EEX6FkXYbdWDgWyRdG7X0c4AydwEfbgjDaI6U4TyktUC3husywev%2F7T7dKOBndLF94H6ax0IwNNfZfi8JuoZpu1%2FpAeJifAIji8K2%2FhKhNDyH26sXrLDrAwaKP0U5ZnK23xtENHCktLjpvIUqzP3sZ6Z%2FLwrjTXnPWs%2FDXG6aDxTdTsfpoNHN1k8sFOzuPVHLjnmSCptFOCESLzF9z4TvR08Qi40%2BTBL39LSAGuMoTZL8OiI7PxPTYsqO%2BKfEcA8%2FXTPZVMUOC2XeoeZvrYwgYX0e4JJLaXkWi6oeO0n3PMLiOwQ2jOnQ1%2FVIKldRmFUTt3KQzVoj14nFBC7i%2FjPE2yaaXkT3ij8xgZskaCL6KLuHRCuyssQvPD%2FOd8i0JjAdiK8Wukaun9XwQSlN4KyNtjSXosG19wUbI9g9BiCJDhGezij1bFBN0UEA5z62KhzeE%2BR2UkaOYBbofFmS3QCpKcThtaR1BGHd%2BqfBS3NlVIRyrQpabkr1ErBG6ImkKSAqppdegKOJO2D5ncrREJwmwFEQ3AhssLcH6I48ZPE62q7Tw5HsZNAHHNBOb3B8%2BKp3TxTYnPNeR0%2BR1hyVJrZaxstw%2B41QbFmX0YJuUOfkMNkHRzsfiUCsdFZDlV%2BvuQve4CQ&allow_caching=true&sz=w1920-h945-rw&auditContext=forDisplay)

**Distribuição por Banco**

**O que mostra:** como o saldo se distribui entre os bancos/contas, em um gráfico de rosca acompanhado de uma tabela (banco, nº de contas e saldo).

**Como ler:** cada fatia da rosca é um banco — ao lado, a tabela detalha quantas contas e qual o saldo de cada um. Saldos negativos aparecem na tabela com sinal de menos.

**Para que serve:** ter a posição consolidada por banco em um só lugar, apoiando decisões de transferência entre contas e a gestão de concentração bancária.  
  
![Exibindo image.png](https://chat.google.com/u/0/api/get_attachment_url?url_type=FIFE_URL&content_type=image%2Fpng&attachment_token=AOo0EEUWcTxenNlk%2BbjcFVrAI0lXCldykuas2fZZfJi3xKRfGLTSPRvsP%2B1h72DOa7zbriv3hxrQkiKzBZQYqWe5fOdP%2B1D%2FWBl7BlBU0zGKXADP%2FFlrvYZsBIglAZ%2BXdKO60GaSzUKYSpUHIayBCAcEtm2ZpoNf%2BxAhH3CIWtr6OvGf%2FTHUAVOCYRKO5QNcZmvjeYx6Ey1QXCREiK17F4pqComXveYs%2Ff45dzwPdQkYBn4%2Fe5i5BGfLZj4PFNznAHW%2Bq2TUyk7B3nrILgm4nHDreXmpwfuy%2FEqLBX72V9aL91TIXoG5Gfny3Uy5%2F1Wl453E6YINBYBPPz0eOMwVVg4DbGJPZ3TNdR4VpkXFTxxUY6xS8JOoLrsyifUPpRmwzI0mknC3C8yDnA2oOmoZLfK9xb0OYpJxKKI9nRI1LtbvvvAOBhvkTP%2Bv3j5RpSDurLlMtrVzDQIMQCLFkKt2lMRoV3rGzCVxeQNJg78olVsnJYwDloxmiUBtUO6oAOqcj4vLVrMvjMr6gK4cUGy0E0fGiwFcxZhFfndOgWOXu0pDC%2Fsw9Ll%2B2q5QVEUCM29GMG785OTunEeOREo09SuZKiDPsJgeZZVCkuBFTza54S95SEMyG7M3mYNwlv31qW03x8KVJhyy&allow_caching=true&sz=w1920-h945-rw&auditContext=forDisplay)  
 

## Fluxo Projetado

O gráfico **Fluxo Projetado** projeta o saldo de caixa dos próximos dias a partir dos títulos em aberto, ajudando você a antecipar se o caixa corre risco de ficar negativo. Diferente dos demais gráficos da tela, ele parte sempre da data de hoje e olha para frente.  
  
 

![](https://ajuda.sankhya.com.br/hc/article_attachments/41837818224279)

_Gráfico Fluxo Projetado com os toggles de regime e horizonte e a faixa de alerta de saldo negativo_ 

**⚠️ Atenção**

O **Fluxo Projetado** considera apenas os filtros de **Contas bancárias** e **Empresa**. Os filtros de **Arquivo DRE**, **Período**, **Naturezas**, **Centro de custo** e os **Filtros avançados** não afetam esta projeção.

### Como a projeção é calculada

A projeção parte do saldo atual das contas (o ponto de hoje) e soma, dia a dia, os títulos em aberto conforme o vencimento — os a receber aumentam o saldo projetado, os a pagar reduzem. O resultado é a curva de saldo esperado para o horizonte selecionado.

*   São considerados somente títulos em aberto — ainda não recebidos nem pagos.
*   A projeção começa sempre na data atual.

### Regime e horizonte

Dois controles no canto superior direito do card ajustam a projeção:

*   **Caixa** ou **Competência** — define o regime da projeção.
*   **7 dias**, **15 dias**, **30 dias** ou **90 dias** — define o horizonte projetado à frente.

### Alerta de saldo negativo

Quando a projeção indica que o saldo ficará negativo em algum dia do horizonte, o card exibe uma faixa de alerta com a data prevista da ruptura: _"Saldo projetado negativo em DD/MM — risco de ruptura de caixa"_. Use esse aviso para antecipar cobranças ou reprogramar pagamentos antes que o caixa fique negativo.

**ℹ️ Nota**

Se nenhum dia do horizonte projetado ficar negativo, a faixa de alerta não aparece.

## Análise de vencimentos (Aging)

O gráfico **Vencimentos** vai além do período filtrado: ele mostra o quanto há a receber e a pagar distribuído por faixas de atraso, calculadas sempre em relação à data atual. É o recurso certo para identificar rapidamente se títulos vencidos estão se acumulando.

| Faixa | O que representa |
| --- | --- |
| **A vencer** | Títulos cujo vencimento ainda não chegou — posição futura. |
| **1 a 30 dias** | Vencidos há até 30 dias — atraso recente. |
| **31 a 60 dias** | Vencidos entre 31 e 60 dias — atraso que merece atenção. |
| **61 a 90 dias** | Vencidos entre 61 e 90 dias — atraso relevante. |
| **Mais de 90 dias** | Vencidos há mais de 90 dias — maior risco; do lado de recebimentos, candidatos a inadimplência. |

**ℹ️ Nota**

As cinco faixas são sempre exibidas, mesmo sem lançamentos nelas — facilitando a comparação visual.

## Detalhe ao clicar nos gráficos

Nos gráficos que permitem drill-down, clicar em uma barra ou fatia abre uma janela com o contexto daquele ponto. O conteúdo da janela é sempre o mesmo: três cards de resumo — **Tipo** (Receitas ou Despesas), **Total de títulos** e **Valor total** — seguidos da lista de lançamentos paginada, com as colunas: título, parceiro, natureza, data de negociação, data de vencimento, valor líquido e situação.

**ℹ️ Nota**

O gráfico **Distribuição por Banco** é o único que exibe entradas e saídas juntas na mesma lista de detalhe.

![](https://ajuda.sankhya.com.br/hc/article_attachments/41307193686679)

![](https://ajuda.sankhya.com.br/hc/article_attachments/41307193687703)

Relativo a

*   [sankhyafinance](https://ajuda.sankhya.com.br/hc/pt-br/search?content_tags=01KVBPQS4F0A9FYX0DRX3B56B1&utf8=%E2%9C%93 "Resultados da pesquisa")