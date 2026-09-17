# Conferência de Cálculo Individual

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/39318926935191-Confer%C3%AAncia-de-C%C3%A1lculo-Individual](https://ajuda.sankhya.com.br/hc/pt-br/articles/39318926935191-Confer%C3%AAncia-de-C%C3%A1lculo-Individual)

---

# Conferência de Cálculo Individual

**Módulo:** Pessoal+  
**Caminho de Acesso:** Pessoal+ > Rotinas Folha  
**ID da Tela:** br.com.sankhya.rh.CalculoIndFolha

---

## **Sumário**

[Descrição e Usabilidade](#h_01KMNPN0XKFWTY01QMA1K2DNXQ)

[1\. Descrição da Funcionalidade](#h_01KMNPN0YBDF7ZJGJJ2AZM5VAG)  
[2\. Pré-requisitos](#h_01KMNPN0YHT7GC9MCSYW2VS9Z8)  
[3\. Jornada de Uso](#h_01KMNPN0YM2H9RZ4F5AGCGKJZ6)  
[4\. Pontos de Atenção](#h_01KMNPN105NYB7Z5TJEHC5AQVD)  
[5\. Dicas de Usabilidade](#h_01KMNPN10673T6V96Y5XS8ZS4Z)

[Perguntas Frequentes (FAQ)](#h_01KMNPN10BCF4DRACC1YHBTAJC)  
[Artigos Relacionados](#h_01KM0EQ552PB6F72T5Z2K7MMJ6)

---

## **Descrição e Usabilidade**

A conferência da folha de pagamento é a etapa onde você valida se os valores calculados estão corretos antes de confirmar a folha e seguir para integração e envio ao eSocial.

Essa etapa deve ser realizada sempre após o cálculo da folha, seja mensal, férias, rescisão ou 13º salário.

A conferência evita erros como:

*   Valores incorretos de salário;
*   Descontos indevidos;
*   Encargos calculados errado;
*   Problemas no envio ao eSocial.

### **1\. Descrição da Funcionalidade**

A rotina de conferência permite:

*   Validar proventos e descontos;
*   Conferir bases de cálculo (INSS, FGTS, IRRF, PIS);
*   Analisar encargos enviados ao eSocial;
*   Verificar avisos e inconsistências;
*   Entender como o cálculo foi feito (LOG).

A conferência pode ser feita:

*   Na própria tela de **Cálculos** quando se tratar de cálculo individual.
*   No **Gerenciador de Folhas** quando o cálculo for coletivo.

### **2\. Pré-requisitos**

Antes de conferir a folha:

*   A folha deve estar calculada;
*   As movimentações devem ter sido lançadas corretamente;
*   Os eventos devem estar configurados corretamente;
*   Os afastamentos (se houver) devem estar informados.

## **3\. Jornada de Uso**

![1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/39343912016023) A conferência deve ser feita analisando as abas disponíveis:

![conferenfolhacalc.gif](https://ajuda.sankhya.com.br/hc/article_attachments/39334663862423)

#### **![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42315206257687)Aba Folha**

Aqui são apresentados os principais valores de:

*   Dias trabalhados;
*   Salário base;
*   Proventos;
*   Descontos;
*   Salário líquido.

Você pode escolher visualizar em formato de **cards** ou **gráficos** clicando no ícone do canto superior direito da tela.

Para conferência dos detalhes do pagamento, clique nas linhas correspondentes:

✔️ **Proventos**

Esta seção apresenta todos os pagamentos de natureza salarial que serão feitos ao colaborador:

*   Salário base;
*   Horas extras;
*   Adicionais;
*   Férias;
*   Salário-família;
*   13º salário;
*   PLR.

**✔️ Descontos**

Nesta seção estão todos os valores deduzidos do salário base do colaborador, como:

*   INSS;
*   IRRF;
*   Vale transporte;
*   Plano de saúde;
*   Faltas e atrasos;
*   Pensão alimentícia.

**✔️ eSocial (encargos)**

![eSocial-base-de-cálculo.gif](https://ajuda.sankhya.com.br/hc/article_attachments/39338261850391)

Esta seção é destinada à [Conferência de Encargos](https://ajuda.sankhya.com.br/hc/pt-br/articles/25506992271255).

*   INSS
*   FGTS
*   IRRF
*   PIS/PASEP
*   Contribuição sindical

Os valores dos campos **INSS**, **FGTS**, **PIS/PASEP** e **Contribuição Sindical** serão apresentados ao lado do valor correspondente à sua base de cálculo, e, se houver, a diferença entre elas separadas pelo tipo de tributação.

⚠️ Os **valores dependem das incidências** configuradas na **aba eSocial do cadastro dos eventos**.

<table class="wysiwyg-table-resized" style="border-collapse: collapse; margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 18%;"> <col style="width: 57%;"> <col style="width: 25%;"></colgroup><tbody><tr style="height: 22px;"><td style="background-color: #90ee90; height: 22px; text-align: center; vertical-align: middle; width: 21.6191%;"><strong>Tipo de Tributação</strong></td><td style="background-color: #90ee90; height: 22px; text-align: center; vertical-align: middle; width: 38.9046%;"><strong>&nbsp; INSS, FGTS e Contribuição Sindical (eSocial)</strong></td><td style="background-color: #90ee90; height: 22px; text-align: center; vertical-align: middle; width: 59.6191%;"><strong>&nbsp; Base para INSS, FGTS e Contribuição Sindical</strong></td></tr><tr><td><span style="color: #4D4D4D;"><strong>INSS</strong></span></td><td style="vertical-align: top;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>Incidência p/ Previdência</strong> = <strong>11 (MENSAL)</strong>.</span></td><td><span style="color: #4D4D4D;">Soma dos valores das <strong>Bases de Cálculo</strong>: <strong>8 (INSS&nbsp;Trabalhador Assalariado)</strong> + <strong>18 (INSS Honorários&nbsp;Prestadores de Serviços)</strong> + <strong>19 (INSS Honorários do Transporte Rodoviário)</strong> + <strong>17 (INSS Pró Labore)</strong>.</span></td></tr><tr style="height: 22px;"><td style="height: 10px; width: 21.6191%;"><span style="color: #4D4D4D;"><strong>INSS 13</strong></span></td><td style="height: 10px; width: 38.9046%;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>Incidência p/ Previdência</strong> =<strong> 12 (13º Salário)</strong>.</span></td><td style="height: 10px; vertical-align: top; width: 59.6191%;"><span style="color: #4D4D4D;">Valor da <strong>Base de Cálculo</strong> com identificação <strong>9 (INSS 13º Sal. Trab. Assalariado)</strong>.</span></td></tr><tr style="height: 22px;"><td style="height: 11px; width: 21.6191%;"><span style="color: #4D4D4D;"><strong>FGTS</strong></span></td><td style="height: 11px; width: 38.9046%;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>FGTS&nbsp;</strong>=<strong> 11 (FGTS mensal)</strong>.</span></td><td style="height: 11px; vertical-align: top; width: 59.6191%;"><span style="color: #4D4D4D;">Valor da <strong>Base de Cálculo</strong> com identificação <strong>10 (FGTS)</strong>.</span></td></tr><tr style="height: 22px;"><td style="height: 10px; width: 21.6191%;"><span style="color: #4D4D4D;"><strong>FGTS 13</strong></span></td><td style="height: 10px; width: 38.9046%;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>FGTS</strong> = <strong>12 (Remuneração 13º salário)</strong>.</span></td><td style="height: 10px; vertical-align: top; width: 59.6191%;"><span style="color: #4D4D4D;">Valor da <strong>Base de Cálculo</strong> com identificação <strong>11 (FGTS 13º&nbsp;Sal)</strong>.</span></td></tr><tr style="height: 22px;"><td style="height: 10px; width: 21.6191%;"><span style="color: #4D4D4D;"><strong>FGTS Rescisório</strong></span></td><td style="height: 10px; width: 38.9046%;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>FGTS</strong> = <strong>21 (FGTS aviso prévio indenizado)</strong>.</span></td><td style="height: 10px; vertical-align: top; width: 59.6191%;"><span style="color: #4D4D4D;">Valor da <strong>Base de Cálculo</strong>&nbsp;identificada como <strong>31 (FGTS Rescisão)</strong>.</span></td></tr><tr><td><span style="color: #4D4D4D;"><strong>Contribuição Sindical</strong></span></td><td><span style="color: #4D4D4D;">Valor dos eventos que no cadastro de <strong>Eventos</strong>, aba&nbsp;<strong>Avançado</strong>, campo <strong>Outros</strong> tenha a opção <strong>Contribuição Sindical </strong>selecionada. E, na aba <strong>eSocial</strong>, o campo <strong>Incidência p/ Contrib. Sindical</strong> = <strong>11 (Base de cálculo)</strong>.</span></td><td>&nbsp;</td></tr></tbody></table>

Já, no campo **IRRF** será exibido os rendimentos tributáveis (sem as deduções legais):

<table class="wysiwyg-table-resized" style="border-collapse: collapse; margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 18%;"> <col style="width: 57%;"> <col style="width: 25%;"></colgroup><tbody><tr style="height: 22px;"><td style="background-color: #90ee90; height: 22px; text-align: center; vertical-align: middle; width: 21.6191%;"><strong>Tipo de Tributação</strong></td><td style="background-color: #90ee90; height: 22px; text-align: center; vertical-align: middle; width: 38.9046%;"><strong>&nbsp;IRRF eSocial</strong></td><td style="background-color: #90ee90; height: 22px; text-align: center; vertical-align: middle; width: 59.6191%;"><strong>&nbsp; Base para IRRF</strong></td></tr><tr><td><span style="color: #4D4D4D;"><strong>IRRF</strong></span></td><td style="vertical-align: top;"><span style="color: #4D4D4D;">Soma dos eventos com<strong> Incidência p/ IRRF </strong>=&nbsp;<strong>11 (RENDIMENTO TRIBUTÁVEL REMUNERAÇÃO MENSAL)</strong>.</span></td><td><span style="color: #4D4D4D;">O valor da <strong>Base de Cálculo</strong> com identificação <strong>12 (IRRF Trabalhador Assalariado)</strong> + <strong>15 (IRRF Honorários Prestador de Serviço)</strong> + <strong>14 (IRRF ProLabore)</strong> + <strong>16 (IRRF Honorários do Transporte Rodoviário)</strong> somado aos <strong>Eventos</strong> <strong>101 (INSS&nbsp;Empregados)</strong>, <strong>109 (INSS Honorários Prestação de&nbsp;Serviços)</strong>, <strong>111 (INSS Honorários Transporte Rodoviários)</strong>, <strong>107 (INSS Pró Labore)</strong>, <strong>176 (Dependentes - Remuneração Mensal)</strong>, <strong>166 (Pensão Alimentícia -&nbsp;Remuneração Mensal)</strong> e <strong>167 (Pensão Alimentícia -&nbsp;Rescisão)</strong>.</span></td></tr><tr style="height: 22px;"><td style="height: 10px; width: 21.6191%;"><span style="color: #4D4D4D;"><strong>IRRF Férias</strong></span></td><td style="height: 10px; vertical-align: top; width: 38.9046%;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>Incidência p/ IRRF</strong> = <strong>13 (RENDIMENTO TRIBUTÁVEL FERIAS)</strong>.</span></td><td style="height: 10px; vertical-align: top; width: 59.6191%;"><span style="color: #4D4D4D;">O valor da <strong>Base de Cálculo</strong> <strong>22 (IRRF Férias)</strong> + o valor dos&nbsp;<strong>Eventos</strong> <strong>201 (Provisão INSS Férias)</strong>, <strong>151 (Dependente Férias)</strong> e <strong>148 (Pensão Alimentícia Férias)</strong>.</span></td></tr><tr style="height: 22px;"><td style="height: 11px; width: 21.6191%;"><span style="color: #4D4D4D;"><strong>IRRF 13º. salário</strong></span></td><td style="height: 11px; vertical-align: top; width: 38.9046%;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>Incidência p/ IRRF</strong> = <strong>12 (RENDIMENTO TRIBUTÁVEL 13º SALARIO)</strong>.</span></td><td style="height: 11px; vertical-align: top; width: 59.6191%;"><span style="color: #4D4D4D;">O valor da <strong>Base de Cálculo</strong> <strong>13 (IRRF 13 Sal Trab. Assalariado)</strong>&nbsp;+ <strong>Eventos</strong> <strong>104 (INSS 13º Sal.&nbsp;Empregados)</strong>, <strong>177 (Dependentes - 13º salário) </strong>e <strong>168 (Pensão Alimentícia - 13 salário)</strong>.</span></td></tr><tr style="height: 22px;"><td style="height: 10px; width: 21.6191%;"><span style="color: #4D4D4D;"><strong>IRRF PLR</strong></span></td><td style="height: 10px; vertical-align: top; width: 38.9046%;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>Incidência p/ IRRF</strong> = <strong>15 (RENDIMENTOS RECEBIDOS ACUMULADAMENTE - RRA)</strong>.</span></td><td style="height: 10px; vertical-align: top; width: 59.6191%;"><span style="color: #4D4D4D;">O valor da <strong>Base de Cálculo</strong> <strong>55 (IRRF PLR)</strong> + <strong>Eventos</strong> com identificação <strong>176 (Dependentes - Remuneração Mensal)</strong> e <strong>149 (Pensão Alimentícia PLR)</strong>.</span></td></tr><tr style="height: 22px;"><td style="height: 10px; width: 21.6191%;"><span style="color: #4D4D4D;"><strong>IRRF RRA</strong></span></td><td style="height: 10px; vertical-align: top; width: 38.9046%;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>FGTS</strong> = <strong>21 (FGTS aviso prévio indenizado)</strong>.</span></td><td style="height: 10px; vertical-align: top; width: 59.6191%;"><span style="color: #4D4D4D;">O valor da <strong>Base de Cálculo</strong> <strong>29 (IRRF RRA)</strong> + <strong>Eventos</strong> <strong>176 (Dependentes - Remuneração Mensal)</strong> e <strong>150 (Pensão Alimentícia&nbsp;RRA)</strong>.</span></td></tr></tbody></table>

De forma semelhante, **as deduções de INSS e Pensão Alimentícia** também serão exibidas separadamente:

<table class="wysiwyg-table-resized" style="border-collapse: collapse; margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 10%;"> <col style="width: 42%;"> <col style="width: 48%;"></colgroup><tbody><tr style="height: 22px;"><td style="background-color: #90ee90; height: 22px; text-align: left; vertical-align: middle; width: 21.6191%;"><strong>Tipo de Tributação</strong></td><td style="background-color: #90ee90; height: 22px; text-align: left; vertical-align: middle; width: 38.9046%;" colspan="2"><strong>Valor</strong></td></tr><tr><td><span style="color: #4D4D4D;"><strong>Valor Dependentes</strong></span></td><td style="vertical-align: top;" colspan="2"><span style="color: #4D4D4D;">O valor apresentado nos Eventos: <strong>176 (Dependentes - Remuneração Mensal)</strong>, <strong>177 (Dependentes - 13º salário)</strong> e <strong>151 (Dependente Férias)</strong>.</span></td></tr><tr><td colspan="3"><span style="color: #990099;"><strong>Nota:</strong></span> <span style="color: #4D4D4D;">se houver mais de um evento na folha a ser conferida, apenas o evento <strong>176 </strong>será considerado. Se a folha contiver apenas os eventos <strong>177</strong> e <strong>151</strong>, no cálculo será&nbsp;considerado apenas o evento de código <strong>177</strong>.</span></td></tr><tr><td style="background-color: #90ee90; height: 22px; text-align: center; width: 24.6191%;"><strong>Tipo de Tributação</strong></td><td style="background-color: #90ee90; height: 22px; width: 36.7619%;"><strong>&nbsp; INSS e Pensão Alimentícia&nbsp;(eSocial)</strong></td><td style="background-color: #90ee90; height: 22px; width: 40.0476%;"><strong>&nbsp; Base para INSS e Pensão&nbsp;Alimentícia</strong></td></tr><tr style="height: 22px;"><td style="height: 10px; width: 21.6191%;"><span style="color: #4D4D4D;"><strong>INSS</strong></span></td><td style="height: 10px; vertical-align: top; width: 38.9046%;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>Incidência p/ IRRF</strong> = <strong>41 (DEDUÇÃO DO RENDIMENTO - PREVIDENCIA OFICIAL - REMUNERAÇÃO MENSAL)</strong>.</span></td><td style="height: 10px; vertical-align: top; width: 59.6191%;"><span style="color: #4D4D4D;">Soma dos valores dos <strong>Eventos</strong>&nbsp;<strong>101 (INSS Empregados)</strong> + <strong>109 (INSS Honorários&nbsp;Prestadores de Serviços)</strong> + <strong>111 (INSS Honorários do&nbsp;Transporte Rodoviário)</strong> + <strong>107 (INSS Pró Labore)</strong>.</span></td></tr><tr style="height: 22px;"><td style="height: 11px; width: 21.6191%;"><span style="color: #4D4D4D;"><strong>INSS13</strong></span></td><td style="height: 11px; vertical-align: top; width: 38.9046%;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>Incidência p/ IRRF</strong> = <strong>42 (DEDUÇÃO DO RENDIMENTO - PREVIDENCIA OFICIAL - 13º SALÁRIO)</strong>.</span></td><td style="height: 11px; vertical-align: top; width: 59.6191%;"><span style="color: #4D4D4D;">Valor do <strong>Evento 104 (INSS 13º Sal. Empregados)</strong>.</span></td></tr><tr style="height: 22px;"><td style="height: 10px; width: 21.6191%;"><span style="color: #4D4D4D;"><strong>INSSRRA</strong></span></td><td style="height: 10px; vertical-align: top; width: 38.9046%;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>Incidência p/ IRRF</strong> = <strong>44 (DEDUÇÕES PREVIDENCIA OFICIAL - RRA)</strong>.</span></td><td style="height: 10px; vertical-align: top; width: 59.6191%;"><span style="color: #4D4D4D;">Valor do <strong>Evento 146 (INSS RRA)</strong>.</span></td></tr><tr style="height: 22px;"><td style="height: 10px; width: 21.6191%;"><span style="color: #4D4D4D;"><strong>Provisão de Desconto INSS (férias)</strong></span></td><td style="height: 10px; vertical-align: top; width: 38.9046%;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>Incidência p/ IRRF</strong> = <strong>43 (DEDUÇÃO DO RENDIMENTO - PREVIDENCIA OFICIAL - FERIAS)</strong>.</span></td><td style="height: 10px; vertical-align: top; width: 59.6191%;"><span style="color: #4D4D4D;">Valor do <strong>Evento 201 (Provisão de INSS de Férias)</strong>.</span></td></tr><tr><td><span style="color: #4D4D4D;"><strong>Pensão Alimentícia</strong></span></td><td><span style="color: #4D4D4D;">Soma dos eventos com <strong>Incidência p/ IRRF</strong> = <strong>51 (DEDUÇÃO DO RENDIMENTO - PENSÃO ALIMENTICIA -&nbsp;REMUNERAÇÃO MENSAL)</strong>.</span></td><td style="vertical-align: top;"><span style="color: #4D4D4D;">Valor do <strong>Evento</strong> <strong>166 (Pensão Alimentícia -&nbsp;Remuneração Mensal)</strong>.</span></td></tr><tr><td><span style="color: #4D4D4D;"><strong>Pensão Alimentícia 13º</strong></span></td><td style="vertical-align: top;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>Incidência p/ IRRF</strong>&nbsp;= <strong>52 (DEDUÇÃO DO RENDIMENTO - PENSÃO ALIMENTICIA - 13º SALÁRIO)</strong>.</span></td><td style="vertical-align: top;"><span style="color: #4D4D4D;">Valor do <strong>Evento 168 (Pensão Alimentícia -&nbsp;Remuneração Mensal)</strong>.</span></td></tr><tr><td><span style="color: #4D4D4D;"><strong>Pensão Alimentícia Férias</strong></span></td><td style="vertical-align: top;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>Incidência p/ IRRF</strong> = <strong>53 (DEDUÇÃO DO RENDIMENTO - PENSÃO ALIMENTICIA - FERIAS)</strong>.</span></td><td style="vertical-align: top;"><span style="color: #4D4D4D;">Valor do <strong>Evento 148 (Pensão Alimentícia Férias)</strong>.</span></td></tr><tr><td><span style="color: #4D4D4D;"><strong>Pensão Alimentícia PLR</strong></span></td><td style="vertical-align: top;"><span style="color: #4D4D4D;">Soma dos eventos com <strong>Incidência p/ IRRF</strong>&nbsp;=<strong> 54 (DEDUÇÃO DO RENDIMENTO - PENSÃO ALIMENTICIA - PLR)</strong>.</span></td><td style="vertical-align: top;"><span style="color: #4D4D4D;">Valor do <strong>Evento 149 (Pensão Alimentícia PLR)</strong>.</span></td></tr><tr><td><span style="color: #4D4D4D;"><strong>Pensão Alimentícia RRA</strong></span></td><td><span style="color: #4D4D4D;">Soma dos eventos <strong>Incidência p/ IRRF</strong> = <strong>55 (DEDUÇÕES PENSÃO&nbsp;ALIMENTICIA - RRA)</strong>.</span></td><td style="vertical-align: top;"><span style="color: #4D4D4D;">Valor do <strong>Evento 150 (Pensão Alimentícia RRA)</strong>.</span></td></tr></tbody></table>

Além disso, se a empresa for [contribuinte do PIS](https://ajuda.sankhya.com.br/hc/pt-br/articles/28240000315543), é possível comparar a base de cálculo do PIS calculada pelo sistema com a enviada ao eSocial. Essa comparação ajuda a identificar diferenças entre a base vinculada ao evento e as configurações de incidência do eSocial.

Caso existam divergências, é importante verificar as configurações do evento nas abas **eSocial** e **Bases de Cálculo** da tela **Eventos**, além da tela [Processos](https://ajuda.sankhya.com.br/hc/pt-br/articles/4405166245655), onde podem estar vinculados eventos que suspendem a incidência do PIS/PASEP.

O pop-up **Eventos que compõem a base** mostra os eventos excluídos por estarem ligados a processos que suspendem a incidência, indicando que a ausência é por medida judicial.

![confpisprocesso.gif](https://ajuda.sankhya.com.br/hc/article_attachments/39338491904023)

**✔️ Bases de cálculo**

Utilize o botão **Eventos que compõem** para identificar quais eventos formaram a base apresentada e validar a origem dos valores.

Se precisar fazer algum ajuste no Evento, é só clicar no botão ![botão Direcionar.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/39338622961559) **Ir para cadastro da base...** que vai levar você para a tela de cadastro da base correspondente.

**Observação:** quando um trabalhador tem vínculos com mais de uma empresa no mesmo período, é necessário considerar o IRRF já retido em outra fonte para que a retenção na empresa atual seja correta.

Informe neste evento a base líquida do IRRF, não a base bruta, pois o sistema não identifica o modelo de cálculo usado pela outra empresa (simplificado ou completo).

**Exemplo:**

Colaborador com vínculo em duas empresas:

*   **Empresa A (outra fonte):**
    *   Base líquida do IRRF: R$ 3.200,00
    *   IRRF retido: R$ 134,86
*   **Empresa B (atual):**
    *   Registrar R$ 3.200,00 no evento **Base de IRRF de Outra Fonte**
    *   Registrar R$ 134,86 no evento **IRRF Retido de Outra Fonte**

**✔️ Ocorrências**

Nesta seção serão apresentadas as **ocorrências** lançadas para o colaborador na competência vigente.

**✔️ Informações do Cálculo**

Aqui, são exibidas as principais informações desse cálculo, sendo elas: **Código da Empresa**, **Código do Funcionário**, **Referência** e **Data de Pagamento**.

**✔️ Demonstrativos**

Nos Demonstrativos constarão os tipos e valores das rubricas pagas ao colaborador.

#### ![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42315206257687)**Aba Movimentações**

![confmovimcalculo.png](https://ajuda.sankhya.com.br/hc/article_attachments/39339266852119)

Verifique se todos os lançamentos de movimento estão corretos.

*   Confirme:
    *   Eventos lançados;
    *   Valores;
    *   Referência correta.

⚠️ Para incluir novos movimentos, a folha precisa estar confirmada. 

Clique no botão **Adicionar Movimento**, selecionar o **Evento** e preencha o **Índice** ou o **Valor** correspondente e salve as informações e confirme o recálculo.

Para lançar um movimento complementar, ative a opção **Verba de Meses Anteriores**. Então, informe no campo **Referência de Origem** uma referência anterior ao cálculo atual.

![maislançmov-calculo.gif](https://ajuda.sankhya.com.br/hc/article_attachments/39341763978007)

#### ![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42315206257687)**Aba Avisos**

![confaviso-calculo.gif](https://ajuda.sankhya.com.br/hc/article_attachments/39342913902999)

Analise as mensagens de inconsistências ou alertas clicando na linha para visualizar os detalhes. 

Depois de confirmar a folha, você pode arquivar os avisos usando o botão **Arquivar** para seguir com a integração contábil e financeira. Se precisar fazer algum ajuste, basta acessar a rotina e recalcular a folha.

⚠️ A partir da **versão 5.53**, se houver eventos calculados na folha para o eSocial ainda não enviados no S-1010, aparecerá a mensagem:

_**"Existem eventos calculados na folha que devem ser enviados no evento S-1010 antes do envio do evento S-1200/S-2299."**_

Clicando no aviso, o sistema mostra os eventos pendentes de envio no S-1010 para que sejam enviados antes dos eventos periódicos S-1200 e S-2299.

#### ![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42315206257687)**Aba Regras**

![confregras-calculo.png](https://ajuda.sankhya.com.br/hc/article_attachments/39343055930135)

Apresenta as configurações do **Registro Fiscal**, **Sindicato** e **Regras de Cálculo** utilizadas no cálculo.

#### ![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42315206257687)**Aba LOG**

![conflog-calculo.gif](https://ajuda.sankhya.com.br/hc/article_attachments/39343571620759)

Exibe como o cálculo foi realizado. Ao clicar em cada linha do LOG, é apresentado os dados das fórmulas principais e suas auxiliares, as variáveis usadas no cálculo e, logo abaixo, os valores das funções presentes em cada uma delas.

💡 Use essa aba para investigar diferenças ou erros.

**Observação:** se a fórmula incluir a chamada de algum Evento por meio das variáveis &E ou &F, ele será exibido como um link para visualização dentro do próprio LOG. Caso o Evento não tenha fórmula associada, aparecerá uma mensagem informando que a fórmula está vazia. Você pode acessar quantos LOGs forem necessários e voltar ao LOG inicial da consulta.

![conflogform-calculo.gif](https://ajuda.sankhya.com.br/hc/article_attachments/39343571621911)

Para facilitar a conferência dos valores, também é possível exportar o LOG de cálculo das fórmulas para um arquivo TXT usando o botão ![botão-download-envio-holerite-P+.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/39343571623063) **Download do log**. Esse arquivo será salvo com o nome **LOGCALC\_MESEANOREF\_TIPO DE FOLHA.txt**.

Exemplo: LOGCALC\_112025\_N.txt

No caso de **Folha Complementar**, o arquivo será compactado em um zip contendo um arquivo para cada referência calculada.

#### ![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42315206257687)**Aba Provisões**

![confprov-calculo.png](https://ajuda.sankhya.com.br/hc/article_attachments/39343623152791)

Apresenta os os valores provisionados para:

*   **13º Salário** (Décimo Terceiro);
*   **Férias**.

Vale lembrar que as configurações contábeis devem estar corretamente ajustadas.

Para saber mais sobre como o sistema calcula essa aba, acesse o artigo: [Como o sistema calcula a aba Provisões na tela de Cálculos](https://ajuda.sankhya.com.br/hc/pt-br/articles/40078646183319).

#### ![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42315206257687)**Aba Médias**

![confmedias-calculo.gif](https://ajuda.sankhya.com.br/hc/article_attachments/39343758733719)

Esta aba apresenta os eventos que formam as médias segundo as Regras de Cálculo definidas. Essas médias aparecem também em férias, rescisão e 13º salário. Clique na linha para ver o detalhamento do cálculo.

![2 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/39343955687703)Após a conferência, se estiver tudo correto:

![confirma-calculo.gif](https://ajuda.sankhya.com.br/hc/article_attachments/39344172725911)

1.  Clique em **Confirmar Folha**.
2.  Você pode emitir os relatórios do cálculo (holerite, relatórios) no menu **Documentos** à esquerda da tela.
3.  Siga para:
    *   Integração contábil;
    *   Integração financeira;
    *   Envio ao eSocial.
4.  Se houver erro:
    *   Ajuste o cadastro ou movimentação
    *   Clique em ![botão-recalcular-P+FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/39344196155799) **Recalcular.**
    *   Ou ![botão-remover-P+.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/39344172728343)**Excluir** e refazer o cálculo.

### **4\. Pontos de Atenção**

*   Nunca confirme a folha sem conferir.
*   Bases de cálculo incorretas geram erro no eSocial.
*   Eventos com incidência errada impactam encargos.
*   Avisos do sistema devem ser analisados.
*   Diferenças entre cálculo e eSocial indicam erro de configuração.

### **5\. Dicas de Usabilidade**

*   Sempre comece conferindo proventos e descontos.
*   Use o LOG para entender diferenças de valores.
*   Padronize um checklist de conferência mensal.
*   Revise eventos em caso de erro recorrente.
*   Valide encargos antes do envio ao eSocial.

## **Perguntas Frequentes (FAQ)**

**1\. Preciso conferir a folha antes de confirmar?**

Sim, essa etapa é obrigatória para evitar erros no pagamento e no eSocial.

**2\. Onde faço a conferência da folha coletiva?**

Na tela Gerenciador de Folhas.

**3\. Posso corrigir a folha depois de confirmar?**

Depende do parâmetro **FPALTCALCULO** que define se o usuário pode alterar a folha após confirmar.

*   **Desligado**: bloqueia alterações manuais.
*   **Ligado**: permite ajustes após confirmação.

**4\. O que fazer se encontrar erro na folha?**

Corrija o cadastro ou movimentação e realize o recálculo.

**5\. Para que serve o LOG do cálculo?**

Para entender como o sistema chegou aos valores calculados.

## **Artigos Relacionados**

*   [Cálculos da Folha de Pagamento](https://ajuda.sankhya.com.br/hc/pt-br/articles/39309113368599)
*   [Cálculo da Folha Mensal](https://ajuda.sankhya.com.br/hc/pt-br/articles/39311261533335)
*   [Gerenciador de Folhas](https://ajuda.sankhya.com.br/hc/pt-br/articles/4424800696599)
*   [Integração Financeira](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044610374)
*   [Central do eSocial](https://ajuda.sankhya.com.br/hc/pt-br/articles/7064222145175)