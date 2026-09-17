# Crédito do Trabalhador: Novas Regras para Desconto em Rescisões Contratuais (Portaria MTE nº 1.115/2026)

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/42166107959319-Cr%C3%A9dito-do-Trabalhador-Novas-Regras-para-Desconto-em-Rescis%C3%B5es-Contratuais-Portaria-MTE-n%C2%BA-1-115-2026](https://ajuda.sankhya.com.br/hc/pt-br/articles/42166107959319-Cr%C3%A9dito-do-Trabalhador-Novas-Regras-para-Desconto-em-Rescis%C3%B5es-Contratuais-Portaria-MTE-n%C2%BA-1-115-2026)

---

# Crédito do Trabalhador: Novas Regras para Desconto em Rescisões Contratuais (Portaria MTE nº 1.115/2026)

**Módulo:** Pessoal+  
**Versão mínima:** 5.113

**Caminhos de acesso:**

*   Pessoal+ > Rotinas Folha > Lançamento de Movimento > Por Funcionário > Importação Automática Crédito do Trabalhador (Webservice)
*   Pessoal+ > Rotinas Folha > Cálculos > Rescisão

---

### **Sumário**

[Descrição e Usabilidade](#h_01KY7KDSKBP1NZ37Q3NX1119KD)

[1\. Descrição da Funcionalidade](#h_01KY7NF473WEWK962GSQWA4FA9)  
[2\. Pré-requisitos](#h_01KY7KDSKT9QQKHAJTSHWYF525)  
[3\. Jornada de Uso](#h_01KY7N6PE0FT0WW48XQVCX825M)

[3.1 Importar os dados do contrato](#h_01KY7KDSMBN9M92TTM0N4RT6KY)  
[3.2 Conferir os dados importados](#h_01KY7M7XQN9ZBKDMDWYJVN0JXB)  
[3.3 Calcular a rescisão](#h_01KY7KDSMHBS5Y0303C1AM53FS)  
[3.4 Emitir o TRCT](#h_01KY7KDSMMJ8WGJJ4YG1APM3DA)

[4\. Pontos de Atenção](#h_01KY7KDSMW09BRYJYV9BY1W5TY)

[Perguntas Frequentes (FAQ)](#h_01KY7KDSMYHFRCXHKC2NZ9QC6C)  
[Artigos Relacionados](#h_01KY7KDSN4TGNFXMGGRW28P4TB)

---

## **Descrição e Usabilidade**

A [**Portaria MTE nº 1.115/2026**](https://www.in.gov.br/web/dou/-/portaria-mte-n-1.115-de-25-de-junho-de-2026-714711070) alterou as regras para desconto do Crédito do Trabalhador (eConsignado) nas rescisões contratuais. As novas regras são aplicadas às rescisões com **data de desligamento a partir de 23/07/2026**. Para desligamento ocorridos até 22/07/2026, o sistema continua utilizando as regras anteriores.

📚 Para saber mais, acesse [Desconto do Crédito do Trabalhador em Caso de Rescisão Contratual](https://ajuda.sankhya.com.br/hc/pt-br/articles/36028895710871).

### **1\. Descrição da Funcionalidade**

A partir das atualizações das regras do **Crédito do Trabalhador** para rescisões contratuais pela **Portaria MTE nº 1.115/2026**, o sistema passou a automatizar todo o processo de consulta, cálculo, lançamento e demonstração do desconto do empréstimo consignado nas verbas rescisórias, reduzindo parametrizações manuais e garantindo que o cálculo da margem consignável considere as verbas rescisórias previstas na legislação.

📚 Acesse o [**Manual do Crédito do Trabalhador**](https://www.gov.br/trabalho-e-emprego/pt-br/assuntos/credito-do-trabalhador/empregador/manual-operacional-do-empregador) e confira todo o fluxo operacional para desligamento do trabalhador (item 5.7).

Durante o processo de rescisão, o sistema:

*   consulta automaticamente os dados atualizados do contrato junto à Dataprev;
*   importa saldo devedor e percentual de garantia;
*   realiza o lançamento automático do saldo devedor e percentual de garantia;
*   calcula o desconto considerando os limites legais;
*   considera as verbas rescisórias na base da margem consignável;
*   apresenta no TRCT todas as informações utilizadas no cálculo.

<table style="margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #FAEEDA; border-color: #854F0B;"><p><strong style="color: #633806;">⚠️ </strong><span style="color: hsl(32,89%,21%);"><strong style="color: #633806;">Atenção</strong></span></p><p><strong>Data de corte da legislação</strong></p><p data-start="1658" data-end="1736">Todo o processamento do Crédito do Trabalhador na rescisão é definido pela <strong data-start="1263" data-end="1302">data de desligamento do colaborador</strong>.</p><ul><li data-list-item-id="e116a9a7fcca6a23ba25e6473c9448215"><p data-start="1658" data-end="1736">Até <strong data-start="1828" data-end="1842">22/07/2026: regras anteriores</strong> do Crédito do Trabalhador;</p></li><li data-list-item-id="e096fdfdfa442f5b73120a12b0d63a29b"><p data-start="1658" data-end="1736">A partir de <strong data-start="1905" data-end="1919">23/07/2026</strong>:<strong data-start="1905" data-end="1919"> novas regras da Portaria MTE nº 1.115/2026</strong>.</p></li></ul><p data-start="1968" data-end="1985">Essa data define:</p><ul data-start="1987" data-end="2201"><li data-section-id="h7vy6k" data-start="1987" data-end="2024" data-list-item-id="e05b2e90f8215a327673a9ed02b1dfaf4">qual serviço da API será utilizado;</li><li data-section-id="1p5kddm" data-start="2025" data-end="2062" data-list-item-id="e70c178afb0eef3f194347b8b04d909c5">quais informações serão importadas;</li><li data-section-id="114yyst" data-start="2063" data-end="2107" data-list-item-id="ecb9f84e25e2707594ae7308d7d4b4210">quais verbas entram na margem consignável;</li><li data-section-id="wewr9y" data-start="2108" data-end="2153" data-list-item-id="ed75227d2aba04844c661292463173559">como será calculado o desconto da rescisão;</li><li data-section-id="1jlc0x4" data-start="2154" data-end="2201" data-list-item-id="eea609c6d8b77829153f9b0694237dfaa">quais informações serão apresentadas no TRCT.</li></ul></td></tr></tbody></table>

### **2\. Pré-requisitos**

Antes de realizar a rescisão, verifique se:

*   a empresa possui integração configurada com a API do Crédito do Trabalhador;
*   o certificado digital utilizado para comunicação com a Dataprev está válido;
*   o colaborador possui contrato ativo do Crédito do Trabalhador registrado junto ao governo;
*   o cálculo da rescisão ainda não foi processado.

### **3\. Jornada de Uso**

#### **3.1 Importar os dados do contrato**

1.  Acesse a tela **Lançamento de Movimento** (Pessoal+ > Rotinas Folha);
2.  Selecione **Por Funcionário**;
3.  Acione o botão **Importação automática Crédito Trabalhador**;
4.  Informe: **Empresa** e **Referência**;
5.  Marque o tipo de importação **Rescisão**;
6.  Informe o **Código do Funcionário**;
7.  Clique em **Importar** e confirme para prosseguir com a importação automática.
    
    Ao iniciar uma importação do tipo **Rescisão**, o sistema consulta a API da Dataprev utilizando o CPF do colaborador.
    
    Após a consulta, o lançamento de movimento é preenchido automaticamente com:
    
    *   Tipo de Movimento: Rescisão;
    *   evento de desconto do Crédito do Trabalhador;
    *   número do contrato;
    *   saldo residual;
    *   percentual de garantia;
    *   instituição financeira.
    
    Se existirem vários contratos ativos, todos serão importados e o cálculo será realizado individualmente para cada contrato. 
    
    Caso o governo não retorne saldo ou percentual de garantia, esses campos serão preenchidos com valor **0**, mantendo a importação disponível para conferência.
    
    <table style="margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #FAEEDA; border-color: #854F0B;"><p><strong style="color: #633806;">⚠️ </strong><span style="color: hsl(32,89%,21%);"><strong style="color: #633806;">Atenção</strong></span></p><p>A rescisão não pode ser calculada enquanto essas informações não forem disponibilizadas pela Dataprev, conforme as <a href="https://www.gov.br/trabalho-e-emprego/pt-br/assuntos/credito-do-trabalhador/empregador/comunicado-aos-empregadores/orientacoes-adicionais-sobre-a-funcionalidade-de-garantias-no-credito-do-trabalhador.pdf" target="_blank" rel="noopener noreferrer">Orientações adicionais sobre a funcionalidade de garantias no crédito do trabalhador</a>.</p></td></tr></tbody></table>
    

#### **3.2 Conferir os dados importados**

1.  Após a importação, confira os dados preenchidos automaticamente pelo sistema.
    
    Para desligamentos ocorridos a partir de **23/07/2026**, passam a integrar automaticamente a base da margem consignável as verbas rescisórias previstas na Portaria MTE nº 1.115/2026, quando existentes no cálculo.
    
    Entre elas:
    
    *   6003 - Aviso prévio indenizado;
        
    *   6004 - Férias em dobro indenizadas na rescisão;
        
    *   6006 - Férias proporcionais;
        
    *   6007 - Férias vencidas.
        
    
    Essas verbas são consideradas apenas nas rescisões. Elas **não são utilizadas na folha mensal**.
    

#### **3.3 Calcular a rescisão**

*   Acesse a tela **Cálculos** (Pessoal+ > Rotinas Folha) e execute normalmente o cálculo da rescisão.
    
    <table style="background-color: #f4fdff; border-style: none; margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #f4fdff; border-color: #185FA5;"><p><span data-markdown-start-index="1971">ℹ️</span><span data-markdown-start-index="1971">&nbsp;</span><span style="color: hsl(210,75%,37%);"><span data-markdown-start-index="1971"><strong>Atualização automática do Crédito do Trabalhador (versão &gt; 5.116)</strong></span></span></p><p data-start="5586" data-end="5628">Após preencher dos dados da <strong>Etapa 1 do cálculo da rescisão</strong>, o sistema consulta automaticamente os dados mais atualizados do Crédito do Trabalhador junto à Dataprev, considerando:<span aria-hidden="true"></span></p><ul><li data-section-id="12er30a" data-start="1634" data-end="1647" data-list-item-id="eabafa34628f2e261af07e30df3592802">Referência;</li><li data-section-id="1s6dciw" data-start="1650" data-end="1670" data-list-item-id="eb5240eab0fa366528c78a8135189c045">Data de Pagamento;</li><li data-section-id="h93626" data-start="1673" data-end="1683" data-list-item-id="e154b26a537145e2d157133fbc282471b">Empresa;</li><li data-section-id="176sv68" data-start="1686" data-end="1700" data-list-item-id="e7f1e0264510377ffd7a50868add9097b">Funcionário;</li><li data-section-id="1dm1ee6" data-start="1703" data-end="1722" data-list-item-id="e43348dc5a252ab26fc524e35831d5928">Data de Demissão.</li></ul><p>Assim, mesmo se a importação (<a href="#h_01KY7KDSMBN9M92TTM0N4RT6KY">etapa 3.1</a>) não tenha sido realizada ou que os dados importados estejam desatualizados, o sistema atualiza as informações antes de calcular a rescisão, garantindo que o cálculo use os dados mais recentes disponíveis no momento do processamento.</p><p>Se a consulta ao governo não for concluída, o cálculo da rescisão <strong data-start="2236" data-end="2258">não é interrompido</strong>. A ocorrência é apresentada na aba <strong data-start="2297" data-end="2318">Avisos </strong>do Cálculo, com a orientação correspondente.</p><p>Se o funcionário, a empresa ou a data de demissão forem alterados, uma nova verificação será realizada no próximo cálculo da rescisão.</p></td></tr></tbody></table>
    
    O sistema calcula automaticamente:
    
    *   a base de margem consignável;
        
    *   as verbas rescisórias elegíveis;
        
    
    Para determinar o valor do desconto, o sistema considera a base de cálculo da margem consignável de garantia limitado ao saldo devedor. Dessa forma, o desconto aplicado corresponde ao menor valor entre:
    
    *   o limite calculado pela garantia rescisória;
    *   o saldo devedor atualizado do contrato.
    
    Caso o limite da garantia seja inferior ao saldo devedor, o sistema realiza um **desconto parcial** e registra o saldo não descontado, que deverá ser tratado entre o trabalhador e a instituição financeira.
    
    Não é necessário informar esses valores manualmente.
    
         
    | Exemplo | Situação | Limite da garantia | Saldo devedor | Desconto aplicado | Resultado |
    | --- | --- | --- | --- | --- | --- |
    | **1** | 
    Base da margem consignável: **R$ 10.000,00**
    
    Garantia: **10%**
    
     | R$ 10.000,00 × 10% = **R$ 1.000,00** | **R$ 1.000,00** | **R$ 1.000,00** | O desconto corresponde exatamente ao saldo devedor. O contrato é quitado integralmente. |
    | **2** | 
    
    Base da margem consignável: **R$ 10.000,00**
    
    Garantia: **10%**
    
     | R$ 10.000,00 × 10% = **R$ 1.000,00** | **R$ 500,00** | **R$ 500,00** | Como o saldo devedor é menor que o limite da garantia, o sistema desconta apenas R$ 500,00 e quita o contrato. |
    | **3** | 
    
    Base da margem consignável: **R$ 10.000,00**
    
    Garantia: **10%**
    
     | R$ 10.000,00 × 10% = **R$ 1.000,00** | **R$ 2.000,00** | **R$ 1.000,00** | Como o limite da garantia é menor que o saldo devedor, o sistema desconta R$ 1.000,00. O saldo restante deverá ser negociado diretamente entre o trabalhador e a instituição financeira. |
    
    <table style="margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #FAEEDA; border-color: #854F0B;"><p><strong style="color: #633806;">⚠️ </strong><span style="color: hsl(32,89%,21%);"><strong style="color: #633806;">Atenção</strong></span></p><p>O sistema sempre aplica o menor valor entre o limite calculado pela garantia rescisória e o saldo devedor atualizado do contrato, conforme previsto na Portaria MTE nº 1.115/2026.</p></td></tr></tbody></table>
    

#### **3.4 Emitir o TRCT**

1.  Após concluir o cálculo da rescisão, gere o TRCT.
    
    O relatório apresentará as informações utilizadas para composição do desconto do Crédito do Trabalhador.
    
    São apresentados:
    
    *   instituição financeira;
        
    *   número do contrato;
        
    *   saldo devedor;
        
    *   percentual de garantia;
        
    *   valor efetivamente descontado;
        
    *   saldo não descontado;
        
    *   mensagem explicativa conforme a situação do contrato:
        
        *   Desconto integral: quando todo o saldo devedor puder ser descontado;
            
        *   Desconto parcial: quando o percentual de garantia limitar o desconto;
            
        *   Sem desconto: quando não existir garantia rescisória vinculada ao contrato.
            
        
        Caso o colaborador possua mais de um contrato ativo, cada contrato será apresentado separadamente.
        

### **4\. Pontos de Atenção**

*   A data de desligamento é o único critério utilizado para definir se serão aplicadas as regras anteriores ou as novas regras da Portaria MTE nº 1.115/2026: 
    *   A regra antiga permanece válida para desligamentos ocorridos até **22/07/2026**;
    *   As novas regras são aplicadas apenas para desligamentos ocorridos a partir de **23/07/2026**.
*   A consulta da API utiliza os dados mais recentes disponibilizados pelo governo.
*   Os eventos de férias e aviso prévio passam a compor automaticamente a margem consignável nas rescisões enquadradas na nova legislação.
*   A inclusão dessas verbas ocorre apenas em rescisões e não altera o comportamento da folha mensal.
*   Se o saldo residual ou o percentual de garantia não forem retornados pela API, os respectivos campos serão preenchidos com **0,00** e será apresentado um aviso para conferência dos dados no Portal Emprega Brasil.
*   Caso a consulta ao governo não seja concluída por indisponibilidade do serviço, o sistema registra a ocorrência e lhe informa.

## **Perguntas Frequentes (FAQ)**

**1\. A partir de quando as novas regras passam a valer?**

Para desligamentos ocorridos a partir de **23/07/2026**.

**2\. O que muda para rescisões anteriores a** **23/07/2026****?**

O sistema continua utilizando as regras anteriores do Crédito do Trabalhador.

**3\. Preciso preencher manualmente os dados do contrato?**

Não.

O sistema consulta automaticamente a API da Dataprev e importa os dados necessários.

**4\. Quais verbas passam a compor a margem consignável?**

As verbas rescisórias previstas na Portaria MTE nº 1.115/2026, como férias indenizadas, férias proporcionais, férias em dobro, adicional constitucional de 1/3, aviso prévio indenizado e respectivas médias, quando presentes na rescisão.

**5\. Se houver mais de um contrato de empréstimo, como o sistema procede?**

Todos os contratos retornados pela API são importados e considerados individualmente durante o cálculo da rescisão.

**6\. O que acontece quando o percentual de garantia é zero?**

Não será realizado desconto utilizando as verbas rescisórias daquele contrato, pois não existe percentual de garantia informado.

O TRCT informará essa situação ao trabalhador.

**7\. Preciso importar manualmente os dados do Crédito do Trabalhador?**

Não é obrigatório. A importação manual continua disponível pela tela **Lançamento de Movimento**, mas, ao calcular a rescisão, o sistema verifica automaticamente se os dados estão atualizados e realiza a consulta necessária para que o cálculo utilize as informações mais recentes disponíveis.

**8\. O que acontece se eu mudar o funcionário, a empresa ou a data de demissão depois que os dados já foram importados?**

Ao calcular novamente a rescisão, o sistema realiza uma nova verificação e atualiza as informações do Crédito do Trabalhador com base nos dados atuais.

**9\. Como sei se houve algum problema na verificação automática?**

Quando a consulta não puder ser concluída, o sistema apresenta um aviso na aba **Avisos** do Cálculo, informando o motivo da ocorrência e a orientação para tentar novamente ou conferir os dados.

## **Artigos Relacionados**

*   [Lançamento do Crédito do Trabalhador no Pessoal+](https://ajuda.sankhya.com.br/hc/pt-br/articles/35831517422871)