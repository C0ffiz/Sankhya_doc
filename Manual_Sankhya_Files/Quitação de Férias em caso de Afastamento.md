# Quitação de Férias em caso de Afastamento

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/31144991936151-Quita%C3%A7%C3%A3o-de-F%C3%A9rias-em-caso-de-Afastamento](https://ajuda.sankhya.com.br/hc/pt-br/articles/31144991936151-Quita%C3%A7%C3%A3o-de-F%C3%A9rias-em-caso-de-Afastamento)

---

# Quitação de Férias em caso de Afastamento

**Módulo:** Pessoal+  
**Caminho de Acesso:** Pessoal+ > Rotinas Folha > Ocorrências  
**ID da Tela:** br.com.sankhya.rh.Ocorrencias

---

## **Descrição e Usabilidade**

### **1\. Descrição da Funcionalidade**

A rotina de quitação de férias é utilizada quando o colaborador permanece afastado por período igual ou superior a 180 dias, nas situações previstas pelo Art. 133 da CLT.

Quando configurada, o Pessoas+ realiza automaticamente a quitação do período aquisitivo de férias e ajusta os períodos aquisitivos do colaborador após o retorno do afastamento.

<table style="margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #FAEEDA; border-color: #854F0B;"><p><strong style="color: #633806;">⚠️ </strong><span style="color: hsl(32,89%,21%);"><strong style="color: #633806;">Atenção</strong></span></p><p>Esta regra é diferente do <strong data-start="914" data-end="975">Bloqueio de Cálculo de Férias para Funcionários Afastados</strong>. Enquanto o bloqueio impede o cálculo de férias durante um afastamento incompatível, a quitação trata da perda do período aquisitivo em afastamentos de longa duração.</p></td></tr></tbody></table>

### **2\. Pré-requisitos**

*   Parâmetro **Quita férias na abertura para afastados - PQUITAFERABERT** habilitado na tela **Preferências** (Configurações > Avançado).
*   Ocorrência cadastrada com a opção **Quita Férias por Afastamentos – Art. 133 CLT** marcada.
*   Lançamento do afastamento realizado na tela **Ocorrências** (Pessoal+ > Rotinas Folha).
*   O campo **Data de Término** da ocorrência deve permanecer em branco enquanto o colaborador estiver afastado.

### **3\. Jornada de Uso**

1.  Acesse a tela **Ocorrências** (Pessoal+ > Rotinas Folha) e localize a ocorrência cadastrada:
    *   Marque na aba **Cadastro** da ocorrência  a opção **Quita Férias por Afastamentos - Art. 133 CLT;**
        
        ![QUITA-FERIAS.png](https://ajuda.sankhya.com.br/hc/article_attachments/35487698656919)
        

*   Volte a aba **Lançamento**, e faça o lançamento da ocorrência para o colaborador, a **Data de término não deve ser preenchida.** Pois, esta só deve ser preenchida quando o colaborador retornar efetivamente do seu afastamento. 
    
    ![Rotina de Quitação de Férias em caso de Afastamento 3.png](https://ajuda.sankhya.com.br/hc/article_attachments/31593841267479)
    

2.  O sistema tem um 'Job' interno que realiza o processo de rodar a quitação das férias de forma automática, esse processo costuma acontecer durante a noite, ou seja, será possível validar a quitação das férias no dia seguinte ao lançamento do afastamento. 
3.  É possível realizar essa quitação de forma manual clicando no botão **Rodar Quitação de Férias, Atualiza Regras, Atualiza Liderança** da tela **Painel de Configurações**.
    
    ![Rotina de Quitação de Férias em caso de Afastamento 4.png](https://ajuda.sankhya.com.br/hc/article_attachments/31593794531223)
    
    <table style="margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #FAEEDA; border-color: #854F0B;"><p><strong style="color: #633806;">⚠️ </strong><span style="color: hsl(32,89%,21%);"><strong style="color: #633806;">Atenção</strong></span></p><p>Importante lembrar que <strong>o sistema não vai realizar o processo de quitação de férias</strong> caso na ocorrência tenha sido preenchido o campo <strong>Data de término</strong>.&nbsp;</p></td></tr></tbody></table>
    
    Nesse período de afastamento não será possível calcular férias para o colaborador, visto que o sistema apresentará a seguinte mensagem: 
    
    ![mceclip5.png](https://ajuda.sankhya.com.br/hc/article_attachments/31144991915671)
    
    Caso selecione a opção **Sim** para seguir com o cálculo, o sistema não irá trazer o período aquisitivo:
    
    ![Rotina de Quitação de Férias em caso de Afastamento 8.png](https://ajuda.sankhya.com.br/hc/article_attachments/31593794541207)
    
    E se mesmo assim tentar calcular as férias, será apresentada a seguinte mensagem: 
    
    ![mceclip7.png](https://ajuda.sankhya.com.br/hc/article_attachments/31144991916439)
    
    Já na tela **Requisições > Férias,** na aba **Aquisitivos** ficará da seguinte forma: 
    
    ![Rotina de Quitação de Férias em caso de Afastamento 9.png](https://ajuda.sankhya.com.br/hc/article_attachments/31593794542871)
    
4.  Quando o colaborador retornar do afastamento deve-se editar a ocorrência de afastamento informando a **Data de término** do afastamento. Após isso, o sistema irá finalizar de forma automática a quitação das férias, ajustando os períodos aquisitivos do colaborador. 
    
    ![Rotina de Quitação de Férias em caso de Afastamento 10.png](https://ajuda.sankhya.com.br/hc/article_attachments/31593841274263)
    
    ![Rotina de Quitação de Férias em caso de Afastamento 11.png](https://ajuda.sankhya.com.br/hc/article_attachments/31593794545175)
    
    A tabela de férias do colaborador será alterada de forma automática, ficando a primeira linha com o período aquisitivo quitado, tendo a data fim alterada para a data de término do afastamento do mesmo. E na segunda linha ficará o novo período aquisitivo começando no dia seguinte do término do afastamento.
    
    A a tela **Requisições > Férias,** na aba **Aquisitivos** ficará da seguinte forma: 
    
    ![Rotina de Quitação de Férias em caso de Afastamento 14.png](https://ajuda.sankhya.com.br/hc/article_attachments/31593794549015)