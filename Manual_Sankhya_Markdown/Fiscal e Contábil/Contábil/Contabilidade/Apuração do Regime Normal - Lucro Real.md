# Apuração do Regime Normal - Lucro Real

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real)

---

# Apuração do Regime Normal - Lucro Real

 **![Módulo](https://ajuda.sankhya.com.br/hc/article_attachments/42312548261655) Módulo:** Contabilidade > Rotinas

---

Esta rotina permite aos optantes pelo regime de Lucro Real, a capacidade de controle e apuração do IRPJ e da CSLL de maneira efetiva e segura. Ela parte dos saldos das contas contábeis da entidade, deste modo, toda a memória de cálculo ficará registrada e evidenciada por meio das telas e dos relatórios nativos.

Para utilização desta rotina, deve-se inicialmente configurar na tela [Plano de Contas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116393) as seções **"Classificação IRPJ"** e **"Classificação CSLL"** que definirão a natureza de cada conta contábil dentro da rotina de apuração do IRPJ e da CSLL, conforme abaixo:

*   **(+) Adições:** essa opção classifica as contas Não dedutíveis;
*   **(-) Exclusões:** contas que serão deduzidas do lucro, reduzindo a base de cálculo;
*   **PAT 4%:** contas do PAT que irão deduzir da base de cálculo do lucro como benefício fiscal;
*   **Conta de Resultado:** são as contas que irão determinar o resultado do período apurado;
*   **Zeramento de Contas de Resultado:** conta responsável pela rotina de Zeramento e que será desconsiderada da rotina de Apuração.

Logo após, informe a **"Empresa"** e a **"Referência"** que deseja apurar, além de definir a **"Forma de Apuração"** conforme as opções:

*   **Mensal/Anual:** refere-se à rotina atual, onde os valores são acumulados de um mês para o outro com a sua conclusão na última competência do ano;
*   **Trimestral:** essa opção é referente à rotina que deve contemplar as informações dos trimestres com encerramentos em 31/03 a 30/06 e 30/09 a 31/12, desprezando, assim, os valores acumulados para a competência seguinte.

Dessa forma, ao final acione o botão ![botão-calcular-FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16994929487511) **"Calcular"**. 

A seguir, clique nos links abaixo para saber mais sobre as demais funcionalidades da tela.

<table style="border-collapse: collapse; width: 100%;" border="1"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 48.0476%;" colspan="2"><strong><span class="wysiwyg-color-black70">Funcionalidades da tela&nbsp;</span></strong></td></tr><tr><td class="wysiwyg-text-align-justify" style="width: 48.0476%;"><span class="wysiwyg-color-black70">&nbsp;<a class="topiclink" href="#detalhamentodasabasdeapura%C3%A7%C3%A3o" target="_self" rel="undefined">Detalhamento das abas de apuração</a></span></td><td style="width: 44.0476%;"><span class="wysiwyg-color-black70">&nbsp;<a href="#abaparteA" target="_self">Aba Parte A</a></span></td></tr><tr><td class="wysiwyg-text-align-justify" style="width: 48.0476%;"><span class="wysiwyg-color-black70">&nbsp;<a href="#abaparteB" target="_self">Aba Parte B</a></span></td><td style="width: 44.0476%;"><span class="wysiwyg-color-black70">&nbsp;<a class="topiclink" href="#bot%C3%B5esdatela" target="_self" rel="undefined">Botões da tela</a></span></td></tr></tbody></table>

---

## **Detalhamento das abas de apuração**

A rotina de apuração trata em abas distintas o IRPJ e a CSLL a serem apurados. As informações de cada imposto estarão disponíveis nas sub-abas [Apuração IRPJ](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real#apura%C3%A7%C3%A3oirpj) e [Apuração CSLL](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real#apuracaocsll), conforme exemplo abaixo:

![abas\_regime.gif](https://ajuda.sankhya.com.br/hc/article_attachments/6923088300439)

O sistema irá considerar os saldos das contas configuradas como Adições e Exclusões, que respectivamente trarão os saldos das contas configuradas no plano de contas da empresa e podendo ser incluídas, excluídas e editadas nas abas [(+) Adições](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real#\(+\)Adi%C3%A7%C3%B5es) e [(-) Exclusões](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real#\(-\)Exclus%C3%B5es).

![adicoes\_exclusoes.gif](https://ajuda.sankhya.com.br/hc/article_attachments/6923123152023)

[\[voltar ao topo\]](#L)

## **Aba Parte A**

![aba\_parte\_A.png](https://ajuda.sankhya.com.br/hc/article_attachments/10821260184343)

Nessa aba, quando habilitada a marcação **"Considerar CR’s específicos para Apuração"**, o sistema irá filtrar os Centros de Resultados cujo a marcação **"CR para calculo e-LALUR Parte A"** da aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044606754-Centros-de-Resultado#abageral) estiverem selecionadas. Sendo que, será considerado somente os saldos das Contas Contábeis e CR’s.

Ao habilitar a marcação **"Deduzir PAT sobre o Adicional IRPJ 10%"**, o cálculo do teto de 4% do PAT será realizado considerando o valor do **"Imposto Devido"**, presente na sub-aba Apuração IRPJ, seção Cálculo Imposto. Do contrário, será aplicado o percentual do teto de 4% somente sobre o valor contido no campo **"IRPJ 15%"**, desconsiderando o adicional de 10%. 

Além dos campos mencionados pode-se configurar as seguintes sub-abas:

<table style="border-collapse: collapse; height: 100px; width: 100%;" border="1" cellspacing="100px" cellpadding="100px"><tbody><tr style="height: 22px;"><td style="width: 47.3333%; height: 22px;"><span class="wysiwyg-color-black70">&nbsp;<a href="#apura%C3%A7%C3%A3oirpj" target="_self">Sub-aba Apuração IRPJ</a></span></td><td style="width: 47.9047%; height: 22px;"><span class="wysiwyg-color-black70">&nbsp;<a href="#apuracaocsll" target="_self">Sub-aba Apuração CSLL</a></span></td></tr><tr style="height: 22px;"><td style="width: 47.3333%; height: 22px;"><span class="wysiwyg-color-black70">&nbsp;<a href="#(+)Adi%C3%A7%C3%B5es" target="_self">Sub-aba (+)Adições</a></span></td><td style="width: 47.9047%; height: 22px;"><span class="wysiwyg-color-black70">&nbsp;<a href="#(-)Exclus%C3%B5es" target="_self">Sub-aba (-)Exclusões</a></span></td></tr><tr style="height: 22px;"><td style="width: 47.3333%; height: 22px;"><span class="wysiwyg-color-black70">&nbsp;<a href="#Incentivosfiscais" target="_self">Sub-aba Incentivos Fiscais</a></span></td><td style="width: 47.9047%; height: 22px;"><span class="wysiwyg-color-black70">&nbsp;<a href="#PER/DCOMP" target="_self">Sub-aba PER/DCOMP</a></span></td></tr><tr style="height: 22px;"><td style="width: 47.3333%; height: 22px;"><span class="wysiwyg-color-black70">&nbsp;<a class="topiclink" href="#recolhimentomesesanteriores" target="_self" rel="undefined">Sub-aba Recolhimento Meses Anteriores</a></span></td><td style="width: 47.9047%; height: 22px;"><span class="wysiwyg-color-black70">&nbsp;<a class="topiclink" href="#notasfiscaiscomretencoes" target="_self" rel="undefined">Sub-aba Notas Fiscais com Retenções</a></span></td></tr><tr style="height: 22px;"><td style="width: 47.3333%; height: 22px;"><span class="wysiwyg-color-black70">&nbsp;<a class="topiclink" href="#darf'srecolhidos" target="_self" rel="undefined">Sub-aba DARF's Recolhidos</a>&nbsp;</span></td><td style="width: 47.9047%; height: 22px;">&nbsp;</td></tr></tbody></table>

---

### **Sub-aba Apuração IRPJ**

![Aba](https://ajuda.sankhya.com.br/hc/article_attachments/15524987841559)

#### **Seção Base de Cálculo**

No campo **"Lucro Antes IRPJ"** será apresentado o valor acumulado por competência registrado mês a mês nos lançamentos contábeis referente as contas configuradas.

Nos campos **"Total das Adições"** e **"Total das Exclusões"** serão considerados os saldos das contas configuradas como Adições e Exclusões, que respectivamente trarão os saldos das contas configuradas no plano de contas da empresa e podendo ser incluídas, excluídas e editadas nas abas [(+) Adições](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real#\(+\)Adi%C3%A7%C3%B5es) e [(-) Exclusões](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real#\(-\)Exclus%C3%B5es).

O campo **"Resultado Liquido Ajustado"** representa o primeiro totalizador desta apuração onde serão considerados:

  ![Calculadora.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42312548262551) _**Lucro Antes IRPJ + Adições - Exclusões**_

Deve ser alimentado manualmente o campo **"Compensação de Prejuízos Fiscais"**, conforme controle do contador para aproveitamento de créditos. Os valores informados neste campo correspondem a seguinte regra:

 ![Calculadora.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42312548262551) **_Resultado Líquido Ajustado - Compensação de Prejuízos Fiscais = Base de Cálculo_**

#### **Seção Cálculo Imposto**

O **"IRPJ 15%"** representa 15% sobre o valor obtido na Base de Cálculo.

O campo **"Adicional de IRPJ 10%"** considera a condição “Se” o valor obtido na Base de Cálculo for maior 20.000,00 ao mês será aplicado 10% sobre o excedente. Sendo que:

 ![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/29119135653271) Quando apurado “mensal/anual” a parcela a deduzir deverá ser multiplicada pela quantidade de meses do ano já realizados até a data da apuração.

 ![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/29119135653271) Quando apurado “trimestral” essa parcela a deduzir será considerada a soma de 3 meses, ou seja, 60.000,00.

O campo **"Imposto devido"** representa a soma dos valores apurados nos campos IRPJ 15% e Adicional de IRPJ 10%.

O **"Valor do PAT"** é demostrativo e representa a movimentação contábil registrada nas contas configuradas.

O campo **"Dedução PAT"** corresponde a dedução do incentivo fiscal por refeição cedida, limitada a 4% do imposto calculado sobre os 15%. A regra contida nesse campo é:

 ![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/29119135653271) Se o valor registrado nas contas contábeis for inferior a 4% do IRPJ 15%, será ele o valor considerado.

 ![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/29119135653271) Se superior, registra-se o resultado de 4% do IRPJ 15%.

O campo **"Dedução Outros Incentivos"** será alimentado com os lançamentos registrados manualmente na sub-aba [Incentivos Fiscais](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real#Incentivosfiscais).

O **"Imposto Devido Liquido"** é igual a fórmula abaixo:

 ![Calculadora.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42312548262551) **_Imposto Devido - Dedução PAT - Dedução Outros Incentivos_**

O **"Total Recolhido Meses Ant."** é alimentado pelas informações contidas na sub-aba [Recolhimento Meses Anteriores](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal#recolhimentomesesanteriores).

#### **Seção Compensações**

O campo **"(-) Compensações"** contém as informações registradas na sub-aba [PER/DCOMP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real#PER/DCOMP).

Em **"Outras Compensações"** serão apresentadas as deduções lançadas manualmente direto no campo da apuração.

**Observação:** ao preencher o campo acima e acionar o botão ![botão-calcular-FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16994929487511) **"Calcular"**, e em seguida escolher a opção **"Cálculo Imposto Parte A"**, se o valor da Base de Cálculo ficar negativo, o campo Outras Compensações terá seu valor zerado; caso contrário, o valor inserido será considerado.

No campo **"Valores IRPJ retido a compensar"** serão exibidas as compensações lançadas na sub-aba [Notas Fiscais com Retenções](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal#notasfiscaiscomretencoes).

O campo **"(-) Compensação de Prejuízos"** irá deduzir do cálculo do Imposto a Recolher, sendo este exclusivo para apuração trimestral, ou seja, se o campo Forma de Apuração for definido com a opção Mensal/Anual o campo ( - ) Compensação de Prejuízos ficará indisponível para edição.

#### **Seção Imposto a Recolher**

É apresentado no campo **"Imposto a Recolher"** o resultado obtido no cálculo **"Saldo do Imposto a Recolher"** menos todas as compensações previstas no bloco de compensações.

Já o **"Recolhimento Avulso"** é um campo informativo e digitável. Não influencia a competência em que está sendo informado, porém na subsequente representa o valor recolhido dos meses anteriores.

[\[voltar ao subtítulo\]](#abaparteA)

### **Sub-aba Apuração CSLL**

**![Aba](https://ajuda.sankhya.com.br/hc/article_attachments/15525124130199)**

#### **Seção Base de Cálculo**

No campo **"Lucro Antes CSLL"** será apresentado o valor acumulado por competência registrado mês a mês nos lançamentos contábeis referente as contas configuradas.

Nos campos **"Total das Adições"** e **"Total das Exclusões"** serão considerados os saldos das contas configuradas como Adições e Exclusões, que respectivamente trarão os saldos das contas configuradas no plano de contas da empresa e podendo ser incluídas, excluídas e editadas nas abas [(+) Adições](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real#\(+\)Adi%C3%A7%C3%B5es) e [(-) Exclusões](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real#\(+\)Adi%C3%A7%C3%B5es).

**Observação:** caso o campo Forma de Tributação esteja definido com a opção Trimestral, os campos Lucro Antes CSLL, Total das Adições e Total das Exclusões apresentarão os valores registrados nas contas contábeis referentes ao movimento da competência, desprezando assim, o saldo acumulado do trimestre anterior ao da referência. Além disso, a informação do campo **"Total Recolhido Meses Ant."** será desconsiderada na apuração trimestral. 

O campo **"Resultado Liquido Ajustado"** representa o primeiro totalizador desta apuração onde serão considerados:

 _**![Calculadora.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42312548262551) Lucro Antes CSLL + Adições - Exclusões**_

O campo **"Compensação BC Negativa da CSLL"** deve ser alimentado manualmente conforme controle do contador para aproveitamento de créditos. Sendo que, os valores informados neste campo correspondem a seguinte regra:

 ![Calculadora.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42312548262551) **_Resultado Liquido Ajustado - Compensação BC Negativa da CSLL = Base de Cálculo_**

#### **Seção** **Cálculo do Imposto**

A **"Alíquota CSLL"** será preenchida com base no valor estipulado (9% ou 15%) no campo **"Alíquota de CSLL (Lei nº 11.727, de 2008, art. 17)"** da aba [Plano de Contas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607994-Empresa#abaplanodecontas) da tela [Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607994-Empresa), após o processamento do Cálculo Imposto Parte A.

O campo **"CSLL"** representa o resultado da conta Base de Cálculo x Aliquota CSLL.

O **"Total Recolhido Meses Ant."** é alimentado pelas informações contidas na sub-aba [Recolhimento Meses Anteriores](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal#recolhimentomesesanteriores).

#### **Seção** **Compensações**

O campo **"(-) Compensações"** contém as informações registradas na sub-aba [PER/DCOMP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real#PER/DCOMP).

Em **"Outras compensações"** serão apresentadas as deduções lançadas manualmente direto no campo da apuração.

No campo **"Valores IRPJ retido a compensar"** serão exibidas as compensações lançadas na sub-aba [Notas Fiscais com Retenções](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal#notasfiscaiscomretencoes).

O campo **"(-) Compensação de Prejuízos"** irá deduzir do cálculo do Imposto á Recolher, sendo este exclusivo para apuração trimestral, ou seja, se o campo Forma de Apuração for definido com a opção Mensal/Anual o campo ( - ) Compensação de Prejuízos ficará indisponível para edição.

#### **Seção** **Imposto a Recolher**

É apresentado no campo **"Imposto a Recolher"** o resultado obtido no cálculo **"Saldo do Imposto a Recolher"** menos todas as compensações previstas no bloco de compensações.

Já o **"Recolhimento Avulso"** é um campo informativo e digitável. Não influencia a competência em que está sendo informado, porém na subsequente representa o valor recolhido dos meses anteriores.

[\[voltar ao subtítulo](#abaparteA)[\]](#abaparteA)

### **Sub-aba (+) Adições**

Nessa sub-aba serão listadas analiticamente as movimentações contidas nas contas configuradas como Adições, podendo ser incluídas, excluídas e editadas. 

![Aba](https://ajuda.sankhya.com.br/hc/article_attachments/15525171665047)

[\[voltar ao subtítulo](#abaparteA)[\]](#abaparteA)

### **Sub-aba (-) Exclusões**

Nessa sub-aba serão listadas analiticamente as movimentações contidas nas contas configuradas como Exclusões, podendo ser incluídas, excluídas e editadas.

![Aba](https://ajuda.sankhya.com.br/hc/article_attachments/15525221463447)

[\[voltar ao subtítulo](#abaparteA)[\]](#abaparteA)

### **Sub-aba Incentivos Fiscais**

Aqui, serão lançados de forma manual os valores correspondentes aos Incentivos Fiscais e alimentará o campo de **"Deduções Outros Incentivos"** para Apuração de IRPJ.

![Aba](https://ajuda.sankhya.com.br/hc/article_attachments/15525238822423)

[\[voltar ao subtítulo](#abaparteA)[\]](#abaparteA)

### **Sub-aba PER/DCOMP**

Os valores correspondentes ao PER/DCOMP, devem ser lançados manualmente nessa sub-aba.

![Aba](https://ajuda.sankhya.com.br/hc/article_attachments/15525231294231)

[\[voltar ao subtítulo](#abaparteA)[\]](#abaparteA)

### **Sub-aba Recolhimento Meses Anteriores**

Essa sub-aba oferece uma visão dos valores apurados nos meses anteriores, propiciando, assim, uma visão geral dos valores apurados durante os meses do exercício contábil.

Para que os campos **"Valor Recolhimento IRPJ"** e **"Valor Recolhimento CSLL"** sejam alimentados, automaticamente, é necessário preencher manualmente a informação de Recolhimento Avulso nas abas de apuração de IRPJ e também de CSLL nas referências anteriores.

![Aba](https://ajuda.sankhya.com.br/hc/article_attachments/15525278511767)

**Importante:** conforme IN 1700/2017, art. 47, § 5°, o Recolhimento de Meses Anteriores só será considerado para a apuração "anual/mensal", pois essa modalidade tem reconhecimento por estimativas mensal, assim os valores são acumulados mensalmente, zerando ou reduzindo o valor à pagar. Já na apuração "trimestral", os valores são considerados de forma isolada, não impactando de forma cumulativa.

[\[voltar ao subtítulo\]](#abaparteA)

### **Sub-aba Notas Fiscais com Retenções**

Os registros contidos nessa sub-aba é de origem manual e tem como objetivo deixar registrado no período de apuração notas fiscais que possuem IRPJ ou CSLL retidos e que poderão influenciar na rotina de Apuração, ou seja, por meio de uma consulta rápida, você poderá selecionar o número único de um documento e apontar manualmente os valores. Essas informações ficarão registradas e disponíveis sempre que necessário, contribuindo no histórico dos valores apurados.

Ao acionar a marcação **"Compensar retenção no IRPJ e CSLL?"** os valores preenchidos nos campos **"Vlr. IRPJ"** e **"****Vlr. CSLL"** desta mesma aba, serão inseridos nos campos **"Valores IRPJ retido a compensar"** e **"Valor CSLL retido a compensar"** localizados nas sub-abas [Apuração IRPJ](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real#apura%C3%A7%C3%A3oirpj) e [Apuração CSLL](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607314-Apura%C3%A7%C3%A3o-do-Regime-Normal-Lucro-Real#apuracaocsll), respectivamente.

![Aba](https://ajuda.sankhya.com.br/hc/article_attachments/15525299987223)

[\[voltar ao subtítulo\]](#abaparteA)

---

### **Sub-aba DARF's Recolhidos**

Nessa sub-aba é possível registrar manualmente as informações sobre os DARF´s gerados, melhorando assim a rastreabilidade da origem dos documentos a serem pagos e da apuração que deu origem aos mesmos.

![Aba](https://ajuda.sankhya.com.br/hc/article_attachments/15525363330071)

[\[voltar ao subtítulo\]](#abaparteA) [\[voltar ao topo\]](#L)

## **Aba Parte B**

 ![versão FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42312559161623) **Esta aba estará disponível a partir da versão 4.18 do sistema.**

Nessa aba, serão adequados os lançamentos de compensações na Parte B do e-LALUR e e-LACS, ou seja, serão inclusos os valores que afetarão o Lucro Real de períodos-bases futuros, como, por exemplo, Prejuízos à Compensar, Depreciação Acelerada Incentivada, Lucro Inflacionário Acumulado até 31.12,1995, entre outros.

 ![Atenção FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16981016372631) Os lançamentos contidos nessa aba, são exclusivamente de origem manual.

![aba-parte-b.png](https://ajuda.sankhya.com.br/hc/article_attachments/12742080422167)

Assim, nessa aba tem-se disponível a sub-aba **"Compensações"**, que tratará dos registros M1410 e M500 da ECF que trata de prejuízos fiscais de períodos de apurações anteriores, sejam elas operacionais ou não, de períodos anuais ou trimestrais, conforme o respectivo regime.

**Nota:** por não ter impacto na Parte A, esse lançamento é um demonstrativo para controle do contador e deve ser alimentado manualmente.

[\[voltar ao topo\]](#top)

**Botões da tela**

O botão ![Botão Outras Opções.. FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16981062253591) **"Outras Opções..."** possui opções que influenciam diretamente no funcionamento da tela. Vejamos sobre elas:

*   **Cálculo Imposto:** essa opção dará início aos cálculos;
*   **Relatório IRPJ:** com esta opção, será gerado o relatório de resumo da apuração do IRPJ;
*   **Relatório CSLL:** ao acionar esta opção, gera-se o relatório de resumo da apuração da CSLL.
*   **Relatório Parte B:** quando essa opção for acionada, será visualizado um relatório contendo as páginas referentes aos impostos IRPJ e CSLL. Assim, será possível controlar o saldo da Parte B do LALUR e LACS que não são mencionadas na escrituração comercial, mas que influenciam a determinação do lucro real dos períodos futuros.

O botão ![botão-calcular-FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16994929487511) **"Calcular"** irá executar os cálculos da tela Apuração do Regime Normal. Além disso, na seta desse botão também há duas opções que poderão ser acionadas após informar a Empresa, Referência e o Tipo de Apuração. Observe:

*   **Cálculo Imposto Parte A:** ao acionar essa opção, o sistema efetuará um processamento com as informações preenchidas da aba Parte A;
*   **Cálculo Imposto Parte B:** assim como a opção acima, essa também irá realizar o processamento conforme os dados da aba Parte B. Esses dados são de cadastros e deverão se preenchidos manualmente.

---

 **![informações adicionais FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/29239787816599) Informações adicionais acerca do Cálculo Imposto Parte B:**

Ao apurar o resultado mensal ou trimestral para calcular o prejuízo do período, insira o valor do prejuízo na conta contábil correspondente na Parte B do LALUR e avance para a apuração do próximo período.

Dessa forma, sabe-se que, ao clicar no botão Calcular, o sistema registra a apuração com base nos saldos contábeis. No entanto, caso o saldo atual seja diferente do saldo da apuração anterior, o pop-up **"Seleção do Método de Recuperação de Saldos - Parte B do LALUR"** será apresentado com a seguinte mensagem:

_**"O saldo recuperado da contabilidade é diferente do saldo final da apuração anterior. Determine qual saldo será recuperado para esta apuração."**_

Pode-se selecionar uma das duas opções apresentadas:

*   **Recuperar saldos da contabilidade:** o sistema recupera o saldo da conta contábil indicada na contabilidade e registra esse valor no campo **"Saldo Inicial"** da Parte B do LALUR, utilizando a mesma conta contábil referente à apuração;
*   **Recuperar saldos da apuração anterior:** o sistema utiliza o valor do campo **"Saldo Final"** da Parte B do LALUR do trimestre anterior, referente à conta contábil indicada, e o registra no campo Saldo Inicial da Parte B do LALUR da mesma conta contábil referente à apuração. 

[\[voltar ao topo\]](#L)