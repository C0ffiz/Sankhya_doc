# Lançamento de movimento por Evento

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/38299661897239-Lan%C3%A7amento-de-movimento-por-Evento](https://ajuda.sankhya.com.br/hc/pt-br/articles/38299661897239-Lan%C3%A7amento-de-movimento-por-Evento)

---

# Lançamento de movimento por Evento

**Módulo:** Pessoal+  
**Caminho de acesso:** Pessoal+ > Rotinas Folha  
**ID da Tela:**  br.com.sankhya.rh.MovimentacoesFolha

---

## **Descrição e Usabilidade**

### **1\. Descrição da Funcionalidade**

A opção **Lançamento de movimento por evento** permite lançar um mesmo evento para vários funcionários de forma rápida e centralizada.

Essa forma de lançamento é indicada quando o objetivo é aplicar um evento específico para diversos colaboradores simultaneamente, informando os valores ou índices diretamente na lista de funcionários.

Os lançamentos podem ser feitos:

*   [**Por Funcionário**](https://ajuda.sankhya.com.br/hc/pt-br/articles/38268572935319)
    
*   **Por Evento**
    

Este artigo explica o **lançamento por evento**.

<table style="margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #FAEEDA; border-color: #854F0B;"><p><strong style="color: #633806;">⚠️ </strong><span style="color: hsl(32,89%,21%);"><strong style="color: #633806;">Atenção</strong></span></p><p>Se já existir folha calculada para a competência, não é possível lançar novos movimentos para os colaboradores dessa referência. Antes de lançar, acesse o <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/40106318532247" target="_blank" rel="noopener noreferrer"><strong>Gerenciador de Folhas</strong></a> e exclua o cálculo da folha desses funcionários; depois de lançar o movimento, calcule a folha novamente.</p></td></tr></tbody></table>

### **2\. Pré-requisitos**

Para utilizar a rotina, é necessário:

*   Ter acesso ao módulo **Pessoal+** e às rotinas de folha.
    
*   Ter eventos previamente cadastrados.
    
*   A folha da referência não pode estar calculada para os funcionários que receberão o lançamento. Caso já exista cálculo, acesse o [**Gerenciador de Folhas**](https://ajuda.sankhya.com.br/hc/pt-br/articles/40106318532247) e exclua-o antes de lançar o movimento.
    

### **3\. Jornada de Uso**

![lançarmovimentoevento.gif](https://ajuda.sankhya.com.br/hc/article_attachments/38326343691543)

#### **Lançar evento**

1.  Acesse a tela **Lançamento de Movimento** (Pessoal+ > Rotinas Folha) e selecione **Por evento**.
    
2.  No painel de filtros, informe:
    
    *   **Empresa**;
        
    *   **Referência**;
        
    *   **Tipo de Movimento**.
        
        O movimento determina:
        
        *   Em qual folha o lançamento será feito;
            
        *   Se o lançamento será mensal ou fixo.
            
3.  Clique em **Pesquisar** para carregar os eventos.
    
4.  Clique no **card do evento** desejado.
    
    O sistema exibirá as informações do evento e a lista de colaboradores da empresa.
    
    Se algum colaborador já possuir a folha da referência calculada, será exibido o aviso **Com folha calculada**, impedindo o lançamento.
    
5.  Para selecionar os colaboradores, você pode:
    
    *   utilizar o botão **Filtrar** para localizar colaboradores;
        
    *   selecionar, clicando na linha de cada colaborador.
        
6.  Após a seleção, o botão **Informar Valores** será habilitado.
    
7.  Clique em **Informar Valores**
    
8.  Informe:
    
    *   Valor (eventos em unidade Valor);
        
    *   Índice (eventos em Hora/Dia).
        
9.  Se desejar incluir mais colaboradores para o mesmo evento, utilize o botão **Selecionar Outros Funcionários**.
    
10.  Caso queira lançar um único valor para todos os colaboradores selecionados, acione o botão **Lançar valor único**, informe o valor e confirme.
     
11.  Após revisar os dados, clique em **Lançar Movimentos**.
     
12.  O sistema exibirá a mensagem: **"Movimentos lançados com sucesso!"**
     

![Causa FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/38327937977495) Após o lançamento dos movimentos, já é possível **realizar o cálculo da folha dos funcionários** normalmente.

#### **Visualizar, editar ou excluir lançamentos**

*   **Visualizar** **e conferir os eventos lançados**
    1.  Selecione o tipo de movimento **Por funcionário**.
    2.  Preencha os **filtros** e clique em **Pesquisar**.
    3.  Selecione o(s) funcionário(s) e clique na aba **Visualização**.
        
        ![visualizarmovimentoevento.gif](https://ajuda.sankhya.com.br/hc/article_attachments/38326315340055)
        
*   **Editar valor ou índice do evento lançado**
    1.  Estenda o card do evento e passe o mouse sobre a linha do mesmo, clique em **Editar evento** (lápis) e salve a alteração.
        
        ![editarlançamentomovimentoporfuncionario.gif](https://ajuda.sankhya.com.br/hc/article_attachments/38326315343255)
        
*   **Excluir eventos**
    1.  Para excluir, estenda o card do evento e passe o mouse sobre a linha do mesmo, clique em **Excluir evento** (lixeira) e confirme a exclusão.
        
        ![excluirlançamentomovimentoporfuncionario.gif](https://ajuda.sankhya.com.br/hc/article_attachments/38326315344919)
        
    2.  Caso queira excluir o lançamento em lote, clique em **Ver movimentações**, selecione os colaboradores, clicando em seus respectivos cards, e, depois, em **Excluir movimentos** (lixeira).
        
        ![excluirmovimentolote.gif](https://ajuda.sankhya.com.br/hc/article_attachments/38326315349015)
        

### **4\. Pontos de Atenção**

*   **Eventos com parametrização personalizada**
    
    Eventos com parametrização personalizada (por exemplo, um evento de insalubridade configurado de forma específica para a empresa) podem não ser gerados automaticamente durante o cálculo da folha. Nesses casos, lance o evento manualmente pelo **Lançamento de Movimento**, como **Movimento Fixo**, para que ele passe a ser considerado também nas competências seguintes.
    
    A replicação de um lançamento fixo para a competência seguinte só ocorre depois que a referência atual é fechada. Se a referência ainda não tiver sido fechada, o lançamento fixo não aparece automaticamente na próxima competência, isso não indica um erro, apenas que o fechamento ainda está pendente.
    
*   **Rescisão Complementar**
    
    Ao selecionar o tipo de movimento **Rescisão Complementar**, o sistema exibirá o aviso:
    
    _**"Só é possível lançar movimentos de Rescisão Complementar dentro da referência de desligamento do funcionário. Para pagamentos em referências posteriores, utilize o tipo Verba de Meses Anteriores."**_
    
*   **Folha já calculada**
    
    Se a folha estiver calculada para o colaborador:
    
    *   Não será possível realizar novos lançamentos.
        
    *   Será exibido o aviso **Com folha calculada**.
        
    
    Para liberar o lançamento, acesse o [**Gerenciador de Folhas**](https://ajuda.sankhya.com.br/hc/pt-br/articles/40106318532247), exclua o cálculo da folha do(s) funcionário(s) e, em seguida, lance o movimento normalmente. Depois de lançado, calcule a folha novamente.
    
*   **Lançamento via API**
    
    Quando o lançamento for realizado via API:
    
    *   As mesmas validações do lançamento manual serão aplicadas.
        
    *   É necessário preencher corretamente todos os campos.
        
*   **Bloqueio para eventos de Plano de Saúde**
    
    O sistema impedirá o lançamento quando o evento possuir simultaneamente:
    
    *   **Natureza da rubrica:** 9219
        
    *   **Código de incidência de IRRF:** 09, 67 ou 9067
        
    *   **Tipo de rubrica:** 2
        
    
    Ao tentar lançar o movimento nessas condições, o sistema exibirá uma mensagem de bloqueio do lançamento.
    

### **5\. Dicas de Usabilidade**

*   Utilize este modo quando precisar lançar o mesmo evento para muitos colaboradores.
    
*   Use filtros para agilizar a seleção.
    
*   Sempre confirme se a folha não está calculada antes de iniciar o processo.
    

## **Artigos Relacionados**

*   [Lançamento de movimento por funcionário](https://ajuda.sankhya.com.br/hc/pt-br/articles/38268572935319)
    
*   [Cadastro de Eventos](https://ajuda.sankhya.com.br/hc/pt-br/articles/33041194565911)