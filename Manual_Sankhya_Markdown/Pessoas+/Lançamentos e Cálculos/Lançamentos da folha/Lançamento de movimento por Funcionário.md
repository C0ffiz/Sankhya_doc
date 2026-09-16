# Lançamento de movimento por Funcionário

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/38268572935319-Lan%C3%A7amento-de-movimento-por-Funcion%C3%A1rio](https://ajuda.sankhya.com.br/hc/pt-br/articles/38268572935319-Lan%C3%A7amento-de-movimento-por-Funcion%C3%A1rio)

---

# Lançamento de movimento por Funcionário

**Módulo:** Pessoal+  
**Caminho de acesso:** Pessoal+ > Rotinas Folha  
**ID da Tela:**  br.com.sankhya.rh.MovimentacoesFolha

---

## **Descrição e Usabilidade**

### **1\. Descrição da Funcionalidade**

A rotina **Lançamento de movimento** permite incluir eventos diretamente na folha de pagamento, como proventos, descontos, empréstimos, dissídio, férias e rescisões.

Nesta tela é possível:

*   lançar movimentos para um ou vários funcionários;
    
*   visualizar lançamentos realizados;
    
*   editar ou excluir eventos;
    
*   importar movimentos por planilha.
    

Os lançamentos podem ser feitos:

*   **Por Funcionário**
    
*   [**Por Evento**](https://ajuda.sankhya.com.br/hc/pt-br/articles/38299661897239)
    

Este artigo explica o **lançamento por funcionário**.

<table style="margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #FAEEDA; border-color: #854F0B;"><p><strong style="color: #633806;">⚠️ </strong><span style="color: hsl(32,89%,21%);"><strong style="color: #633806;">Atenção</strong></span></p><p>Se já existir folha calculada para a competência, não é possível lançar novos movimentos para os colaboradores dessa referência. Antes de lançar, acesse o <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/40106318532247" target="_blank" rel="noopener noreferrer"><strong>Gerenciador de Folhas</strong></a> e exclua o cálculo da folha desses funcionários; depois de lançar o movimento, calcule a folha novamente.</p></td></tr></tbody></table>

### **2\. Pré-requisitos**

Para utilizar a rotina, é necessário:

*   Ter acesso ao módulo **Pessoal+** e às rotinas de folha.
    
*   Ter eventos previamente cadastrados.
    
*   Para Rescisão Complementar: possuir licença **30362 – E-SOCIAL/W** e desligamento enviado ao eSocial.
    
*   A folha da referência não pode estar calculada para os funcionários que receberão o lançamento. Caso já exista cálculo, acesse o [**Gerenciador de Folhas**](https://ajuda.sankhya.com.br/hc/pt-br/articles/40106318532247) e exclua-o antes de lançar o movimento.
    

### **3\. Jornada de Uso**

![lançamentomovimentoporfuncionario.gif](https://ajuda.sankhya.com.br/hc/article_attachments/38297809638295)

#### **Lançar movimentos**

1.  Acesse a tela **Lançamento de Movimento** (Pessoal+ > Rotinas Folha) e selecione **Por funcionário**.
    
2.  Informe:
    
    *   **Empresa**
        
    *   **Referência**
        
    
    Utilize o campo **Tipo de Filtro** para agilizar a busca por:
    
    *   Empresa
        
    *   Departamento
        
    *   Funcionário
        
    *   Sindicato
        
    *   Situação do Funcionário
        
3.  Clique em **Pesquisar**.
    
4.  Acione o botão [**Importar Movimentos por Planilha**](#h_01KH1TT5904ZSV2391B1SZXJ1G), ou selecione o(s) funcionário(s) desejado(s) clicando no(s) respectivo(s) card(s). 
    
5.  Após escolher o(s) funcionário(s), clique na aba **Lançamento**.
    
6.  Defina no campo **Tipo de Movimento** como o evento será aplicado:
    
    *   **Mensal:** somente na referência atual;
        
    *   **Fixo:** permanece nas próximas referências.
        
    
    Ou selecione a folha que receberá o lançamento:
    
    *   Adiantamento;
        
    *   13º salário;
        
    *   Dissídio;
        
    *   Férias;
        
    *   Verbas de Meses Anteriores;
        
    *   Participação nos Lucros;
        
    *   Produção;
        
    *   Rescisão;
        
    *   Avulso;
        
    *   Rescisão Complementar.
        
7.  Informe o **Evento** desejado e a **Unidade** do evento:
    
    *   Unidade **Valor** → informar valor;
        
    *   Unidade **Hora/Dia** → informar índice.
        
    
    <table style="margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #feffed;"><p><strong>🔎 Evento Plano de Saúde</strong></p><p data-start="104" data-end="330">A partir da<strong> versão 5.85</strong>, ao lançar evento de <strong>plano de saúde</strong>, o sistema sugere automaticamente no campo <strong>Optante</strong>, o próximo <strong data-start="210" data-end="255">optante ainda não utilizado na referência</strong>, evitando indicação repetida do titular e reduzindo erros de lançamento.</p><p data-start="612" data-end="634">A ordenação considera:</p><ul><li data-start="637" data-end="679" data-list-item-id="e8a4af756281f7b972fde7d5982d8b8ee"><p data-start="639" data-end="679">a <strong data-start="641" data-end="673">próxima sequência disponível</strong>; ou</p></li><li data-start="682" data-end="726" data-list-item-id="ec211f121c920c7fca01218cee9b57606"><p data-start="684" data-end="726">a <strong data-start="686" data-end="725">menor sequência ainda não utilizada</strong>.</p></li></ul><p data-start="729" data-end="831">Se todas as sequências já tiverem sido utilizadas, o sistema sugere a <strong data-start="800" data-end="830">menor sequência cadastrada</strong>.</p><p data-start="332" data-end="484" data-is-last-node="" data-is-only-node="">Caso o usuário selecione um <strong>optante</strong> que já possua lançamento na mesma referência, será exibida a mensagem de confirmação abaixo para concluir a inclusão.</p><p data-start="332" data-end="484" data-is-last-node="" data-is-only-node=""><em>“Já existe um lançamento de plano de saúde para o optante XXX nesta referência. Deseja lançar novamente?”</em></p></td></tr></tbody></table>
    
8.  Opções disponíveis:
    
    *   **Sequência personalizada**: quando desmarcada, a sequência do evento será gerada automaticamente para cada colaborador selecionado. Se marcada, o campo **Próxima sequência** será exibido para informar o número de sequência desejado.
        
    *   **Considerar o valor informado para cada parcela**: quando marcada, o campo de unidade **Valor** será usado como o valor de **cada** parcela.
        
    *   **Rateio**: quando marcada, exibirá na tela os campos de rateio do movimento.
        
    *   **Parcelamento (opcional)**: se não desejar parcelar esse movimento, mantenha o campo **número de parcelas** preenchido com (**0**) zero ou **1**. Caso queira parcelar o valor, informe o número de parcelas e a conta bancária para pagamento.
        
        O sistema apresenta as referências e o valor de cada parcela.
        
        ![parcelamentomovimento.gif](https://ajuda.sankhya.com.br/hc/article_attachments/38298569181335)
        
        ⚠️ É importante ressaltar que, quando houver parcelamento para um colaborador e for gerada a rescisão de contrato, o sistema puxa, automaticamente, todos os saldos ainda devidos para realizar o pagamento ou desconto.
        
9.  Após configurar, clique em **Finalizar Adição** no canto superior direito da tela.
    
10.  E, depois, clique em **Lançar Movimentos** e confirme a ação.
     

![Causa FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/38327904148759)Após o lançamento dos movimentos, já é possível **realizar o cálculo da folha dos funcionários** normalmente.

#### **Importar movimentos por planilha**

1\. Para realizar o lançamento de movimentos em lote, é necessário baixar o modelo da planilha por meio do botão **Download Planilha Movimentos**, preencher os dados e salvar em formato .xlsx.

2\. Após informar os filtros, clique em **Importar Movimentos por Planilha.**

![importador-econsignado-esocial-1.gif](https://ajuda.sankhya.com.br/hc/article_attachments/38298650790039)

3\. Clique sobre o tipo de movimento:

*   Outros Movimentos;
*   [Crédito do Trabalhador (eConsignado)](https://ajuda.sankhya.com.br/hc/pt-br/articles/35831517422871-Lan%C3%A7amento-do-Cr%C3%A9dito-do-Trabalhador-no-Pessoal#h_01JR8PTPZE0CKK26PRWXEJP737).

4\. Confirme a importação. 

#### **Visualizar, editar, adicionar ou excluir lançamentos**

Agora, na aba **Visualização,** é possível:

*   **Visualizar** e conferir os eventos lançados;
    
*   **Editar valor ou índice** do evento lançado: para isso, estenda o card do evento e passe o mouse sobre a linha do mesmo, clique em **Editar evento** (lápis) e salve a alteração.
    
    ![editarlançamentomovimentoporfuncionario.gif](https://ajuda.sankhya.com.br/hc/article_attachments/38297883625367)
    
*   **Adicionar evento**: caso necessite lançar um novo evento para o colaborador, acione o botão **Adicionar movimento** e faça o lançamento.
    
    ![lançaroutromovimento.gif](https://ajuda.sankhya.com.br/hc/article_attachments/38299138664343)
    
*   **Excluir eventos**: para excluir, estenda o card do evento e passe o mouse sobre a linha do mesmo, clique em **Excluir evento** (lixeira) e confirme a exclusão.
    
    ![excluirlançamentomovimentoporfuncionario.gif](https://ajuda.sankhya.com.br/hc/article_attachments/38297947597719)
    
    Caso queira excluir o lançamento em lote, clique em **Ver movimentações**, selecione os colaboradores, clicando em seus respectivos cards, e, depois, em **Excluir movimentos** (lixeira).
    
    ![excluirmovimentolote.gif](https://ajuda.sankhya.com.br/hc/article_attachments/38298190577047)
    
    ⚠️ Se a folha estiver calculada, o evento não poderá ser excluído. Nesse caso, exclua primeiro o cálculo da folha.
    

### **4\. Pontos de Atenção**

*   **Folha já calculada**
    
    Se a folha já estiver calculada para o colaborador, não será possível lançar novos movimentos para ele. Acesse o [**Gerenciador de Folhas**](https://ajuda.sankhya.com.br/hc/pt-br/articles/40106318532247), exclua o cálculo da folha desse(s) funcionário(s), realize o lançamento do movimento e, em seguida, calcule a folha novamente.
    
*   **Eventos personalizados**
    
    Lançamento de eventos personalizados, sejam proventos que não incidem INSS, por exemplo, ou descontos, devem possuir identificação: **200 – Outros Eventos Suplementares**, para que assim, sejam corretamente calculados tanto **nas folhas suplementares de Autônomos ou Intermitentes** e posteriormente na unificação do cálculo Mensal.
    
    Neste caso, é necessário:
    
    1.  Duplicar o evento, utilizando as mesmas configurações já existentes.
    2.  Alterar apenas a identificação do evento, vinculando-o ao **código** **200 – Outros Eventos Suplementares**.
    3.  Lembrar que este evento deve ser utilizado **exclusivamente para funcionários autônomos ou intermitentes**.
    
    Após criar o evento com a identificação 200, a verba poderá ser lançada normalmente através da **folha Suplementar (aba Honorários)**.
    
*   **Colaboradores desligados**
    
    É permitido realizar **lançamentos de movimento para colaboradores já desligados**, desde que o lançamento esteja relacionado aos seguintes **tipos de folha**:
    
    *   **Dissídio**
    *   **Verbas de Meses Anteriores**
    *   **Participação nos Lucros**
    *   **Rescisão Complementar**
    
    Esses tipos de folha possibilitam registrar valores devidos ao colaborador após o desligamento, conforme a natureza do pagamento.
    
*   **Rescisão Complementar**
    
    A opção **Rescisão Complementar** só será apresentada no **Tipo de Movimento**, caso o(s) funcionário(s) selecionado(s) respeite(m) as regras descritas abaixo:
    
    *   A referência da demissão é igual à do lançamento  
        ou
    *   A demissão é anterior e o funcionário está em quarentena ativa.
        
        Regras adicionais:
        
        *   Evento deve possuir rubrica **2801 – Quarentena Remunerada;**
            
            Caso não existam eventos configurados conforme mencionado, será apresentada a mensagem: 
            
            _**"Só é permitido o lançamento de eventos de quarentena remunerada em referências posteriores à da rescisão original."**_
            
        *   Desligamento deve estar enviado ao eSocial (S-2299/S-2399).
            
            Caso contrário, a seguinte mensagem será exibida:
            
            _**"O cálculo de Rescisão Complementar só é possível para funcionários que tenham o evento de desligamento (S-2299 / S-2399) finalizado com sucesso no eSocial."**_
            
*   **Dissídio**
    
    Para lançar diferenças de dissídio:
    
    *   Deve existir convenção com data de vigência igual à referência, ou seja, os funcionários selecionados devem estar configurados no sindicato cuja referência do lançamento seja a mesma do campo **"Data de Entrada em Vigor"** da sub-aba **"Geral"** da aba [Convenção coletiva, Acordo coletivo ou Sentença Normativa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360058937953-Sindicato#AbaConven%C3%A7%C3%A3ocoletiva,AcordocoletivoouSenten%C3%A7aNormativa) da tela [Sindicato](https://ajuda.sankhya.com.br/hc/pt-br/articles/360058937953-Sindicato), caso contrário, ao realizar o lançamento, será exibida a mensagem:
        
        _**"Não existe Convenção, Acordo ou Sentença com data de entrada em vigor igual à referência do lançamento. Lançamentos para folha de dissídio só podem ser feitos nestas condições."**_
        
    *   O evento não pode ter a marcação **Tem seus valores recalculados** habilitada na aba **Avançado** do cadastro de **Eventos**.
        
        Se estiver habilitada, o sistema exibirá a seguinte mensagem no momento do lançamento:
        
        _**"Apenas eventos definidos que não tem seus valores recalculados podem ser lançados para folha de dissídio."**_
        
*   **Evento 9253 – Empréstimo eConsignado**
    
    Ao lançar este evento, informe:
    
    *   Instituição financeira;
    *   Observação eConsignado;
    *   Número do contrato eConsignado.
    
    O valor da parcela deve ser lançado mensalmente conforme arquivo de importação do **Portal Emprega Brasil**.
    
    Para saber mais detalhes sobre a utilização do evento 9253, acesse o artigo [Crédito do trabalhador (eConsignado) no eSocial](https://ajuda.sankhya.com.br/hc/pt-br/articles/30769824971031).
    
*   **Importação por planilha**
    
    As colunas da planilha devem corresponder à tabela **TFPMOV**.
    
    Em caso de erro, será necessário excluir os lançamentos e importar novamente.
    
*   **Bloqueio para eventos de Plano de Saúde**
    
    O sistema impedirá o lançamento quando o evento possuir simultaneamente:
    
    *   **Natureza da rubrica:** 9219
    *   **Código de incidência de IRRF:** 09, 67 ou 9067
    *   **Tipo de rubrica:** 2
    
    Ao tentar lançar o movimento nessas condições, o sistema exibirá uma mensagem de bloqueio do lançamento.
    

### **5\. Dicas de Usabilidade**

*   Ao selecionar vários funcionários, o lançamento será feito para todos.
    
*   Use filtros para agilizar a busca de colaboradores.
    
*   Utilize parcelamento para evitar lançamentos manuais mensais.
    
*   Confira os lançamentos na aba **Visualização** antes de finalizar o processo.
    

## **Artigos Relacionados**

*   [Lançamento de movimento por evento](https://ajuda.sankhya.com.br/hc/pt-br/articles/38299661897239)
    
*   [Cadastro de Eventos](https://ajuda.sankhya.com.br/hc/pt-br/articles/33041194565911)
    
*   [Crédito do trabalhador (eConsignado) no eSocial](https://ajuda.sankhya.com.br/hc/pt-br/articles/30769824971031)