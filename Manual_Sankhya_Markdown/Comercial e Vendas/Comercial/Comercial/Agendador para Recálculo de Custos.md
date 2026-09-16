# Agendador para Recálculo de Custos

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594294-Agendador-para-Rec%C3%A1lculo-de-Custos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594294-Agendador-para-Rec%C3%A1lculo-de-Custos)

---

# Agendador para Recálculo de Custos

<table style="border-collapse: collapse; width: 100%; height: 35px;" cellspacing="0,5"><tbody><tr style="height: 58px;"><td class="wysiwyg-text-align-center" style="width: 100%; height: 35px;"><pre class="wysiwyg-text-align-justify"><span class="wysiwyg-font-size-medium"><strong><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42311676936343" alt="Módulo"> Módulo: </strong>Comercial &gt; Avançado &gt; Agendadores  </span></pre></td></tr></tbody></table>

---

Essa tela permite a criação de agendamentos para execução das rotinas de recálculo de custos. Para verificar sobre as informações importantes dessa tela de maneira mais fácil, acesse os links abaixo:

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td style="width: 43.4762%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#painelprincipal">Painel Principal</a>&nbsp;</span></td><td style="width: 10.9047%;">&nbsp;</td><td style="width: 45.619%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#abahorrios">Aba Horários</a></span></td></tr><tr><td style="width: 43.4762%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#abafrenqunciaagendamento">Aba Frequência Agendamento</a></span></td><td style="width: 10.9047%;">&nbsp;</td><td style="width: 45.619%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#abaconfiguraes">Aba Configurações</a></span></td></tr><tr><td style="width: 43.4762%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#parmetrosqueinfluenciamnestarotina">Parâmetros que influenciam esta rotina</a></span></td><td style="width: 10.9047%;">&nbsp;</td><td style="width: 45.619%;">&nbsp;</td></tr></tbody></table>

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/1500007036261)

Essas rotinas permitem a realização do Recálculo de Custos de Produtos a partir de movimentações de entrada, notas de compra, produção, etc. Tal funcionalidade será útil em casos de alterações em fórmulas de precificação (fórmulas de custo/preço) necessárias, devido às redefinições em políticas de custeio e precificação.

Nessa tela, inclua o agendamento por empresa e defina os seguintes parâmetros:

## Painel Principal

O campo **"Nro. agendamento"** é de numeração automática.

A **"Descrição agendamento"** refere-se ao nome da operação que será executada.

Informe a **"Empresa"** referente ao Agendamento.

**Observação:** com o parâmetro **"Custo por empresa? - CUSTOPOREMP"** habilitado, somente a Empresa informada no campo acima será calculada, porém, caso nenhuma seja configurada, a rotina será executada para todas as empresas. Com o parâmetro desativado, a rotina será executada para todas as empresas.

Através da marcação **"Ativo"** você determina se o Agendamento está ativo ou não.

[\[voltar ao topo\]](#top)

## Aba Horários

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/1500007036341)

Defina no campo **"Próxima execução em"** a próxima data em que a operação será executada.

No campo **"Data Final de Execução"** insira até quando a operação será executada.

[\[voltar ao topo\]](#top)

## Aba Frequência Agendamento

Defina nessa aba, o **"Horário"** e a frequência em que a rotina será executada, podendo ser **"Diária"**, **"Semanal"** ou **"Mensal"**.

![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/1500007036481)

[\[voltar ao topo\]](#top)

## Aba Configurações

![mceclip3.png](https://ajuda.sankhya.com.br/hc/article_attachments/1500007036541)

As marcações **"Excluir Custos?"**, **"Calcular Custos de Entrada?"** e **"Calcular Custo Médio?"** definirão quais tarefas de recálculo serão executadas, sendo que:

Se efetuada a marcação Excluir custos?, o sistema irá limpar a tabela de custos (TGFCUS) antes de executar o recálculo.

As marcações Calcular Custos de Entrada? e Calcular Custo Médio? serão utilizadas se o sistema for calcular somente os custos de entrada ou somente os custos médios.

No campo **"E-mail notificações"** informe o e-mail para qual serão enviadas as informações referentes aos recálculos. Assim, será encaminhado um e-mail com as ocorrências do processamento: quantas linhas foram atualizadas e se houve algum erro no Banco de Dados.

**Observação:** Caso as rotinas sejam executadas sem erro, o corpo do e-mail ficará da seguinte forma:

**_GERAÇÃO AUTOMÁTICA DE CUSTOS - Empresa: 00_**

**_Linhas afetadas (Excluir Custos): 0_**

**_Linhas afetadas (Custo Entrada): 0_**

**_Linhas afetadas (Custo Médio): 0_**

Porém, ocorrendo algum erro, será da seguinte forma:

**_GERAÇÃO AUTOMÁTICA DE CUSTOS - Empresa: 00_**

**_Ocorreu o seguinte erro: ORA-00904: PRODUTO.CDPROD: identificador inválido_**

Os **"Filtros"** deverão ser utilizados para determinar o período de movimento que será recalculado o custo.

A seção **"Data Inicial"** possui as seguintes opções:

*   **Ult. Execução:** refere-se a data da última execução;  
    
*   **Hoje:** compete a data atual;
*   **1º dia do mês:** ao selecioná-la considera o primeiro dia do mês;  
    
*   **Ult. dia do mês:** considera-se o último dia do mês.

Utiliza-se o campo **"Dias p/ somar na data inicial"** para adicionar uma determinada quantidade de dias a partir da Data inicial.

Já na seção **"Data Final"** existem os campos:

*   **Hoje:** compete a data atual;
*   **Ult. dia do mês:** considera-se o último dia do mês.  
    

Utiliza-se o campo **"Dias p/ somar na data final"** para adicionar uma determinada quantidade de dias a partir da Data final.  

[\[voltar ao topo\]](#top)

## Parâmetros que influenciam nesta rotina

O parâmetro **"Cálculo de Custo Assíncrono - CALCCUSTOASSINC"**, desativado por padrão, define como o sistema realizará o cálculo de custos. Ele pode ser configurado conforme as seguintes opções:

*   **Transação por Nota**: O cálculo de custos será processado por transação, considerando cada nota fiscal individualmente.
*   **Transação por Item**: O sistema calculará os custos item por item dentro de cada nota fiscal.
*   **Desabilitado**: O cálculo de custo não será realizado de forma assíncrona.

#### **Importante**

Esse parâmetro impacta diretamente a confirmação de notas e o Agendador de Recálculo de Custos. No entanto, **as rotinas de Recálculo de Custo e Atualização de Custo não são afetadas por essa configuração**.

Quando o parâmetro **CALCCUSTOASSINC** estiver definido como **"Transação por Nota"** ou **"Transação por Item"**, o cálculo de custo **não ocorrerá imediatamente**. Caso a base tenha sido recém-iniciada, o custo será processado apenas após a confirmação de uma segunda nota fiscal. O processo ocorre em duas etapas:

1.  Inicialmente, o Cálculo de Custo Assíncrono é preenchido com as informações da nota.
2.  O cálculo de custo é realizado posteriormente por um **JOB específico**, acionado somente após a confirmação de uma segunda nota.

[\[voltar ao topo\]](#top)