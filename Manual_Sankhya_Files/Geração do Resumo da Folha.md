# Geração do Resumo da Folha

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/17268960280727-Gera%C3%A7%C3%A3o-do-Resumo-da-Folha](https://ajuda.sankhya.com.br/hc/pt-br/articles/17268960280727-Gera%C3%A7%C3%A3o-do-Resumo-da-Folha)

---

# Geração do Resumo da Folha

**Módulo:** Pessoal+  
**Caminho de Acesso:** Pessoal+ > Rotinas Folha > Gerenciador de Folhas > Resumo da Folha  
**ID da Tela:** br.com.sankhya.rh.GerenciadorFolha

---

## **Descrição e Usabilidade**

### **1\. Descrição da Funcionalidade**

O **Resumo da Folha** gera um relatório analítico da folha calculada, permitindo conferir valores, contribuições e totais por funcionário de forma rápida e segura.

### **2\. Pré-requisitos**

Antes de gerar o resumo, verifique:

![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/38500911654935)**Acesso à(s) empresa(s)**

*   Usuário inserido no **Grupo de decisores** (Painel de Configurações ) correspondentes à(s) empresa(s). 
    
    *   Acesse o **Painel de Configurações** (Pessoal+ > Configurações > Painel de Configurações).
    *   Vá até a seção **Grupo de Decisores**.
    *   Clique sobre o card do **grupo de usuários**, em seguida, certifique-se de que a empresa esteja na lista ao lado direito da tela.
        
        Caso não esteja, basta clicar no sinal de **adição** e adicionar a empresa desejada.
        
    
    ![acessoempresa-rotinascalculosfolhas.gif](https://ajuda.sankhya.com.br/hc/article_attachments/39732942951703)
    

![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/38500911654935)**Permissão concedida para gerar o resumo da folha**

*   Acesse o **Painel de Configurações** (Pessoal+ > Configurações > Painel de Configurações).
*   Vá até a seção **Configuração de Permissões**.
*   Selecione a tela **Gerenciador de Folhas**, em seguida, o grupo de usuários desejado e certifique-se de que a permissão **Resumo da Folha** esteja habilitada.
    
    ![permissao-resumofolhas.gif](https://ajuda.sankhya.com.br/hc/article_attachments/39733137591063)
    

**![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/38500911654935)Folha calculada**

*   A folha deve estar **calculada** na referência desejada.
    

**![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/38500911654935)Registro Fiscal por Departamento (quando aplicável)**

*   Se a empresa utiliza Registro Fiscal por Departamentos (parâmetro **FPREGFISCAL**), é obrigatório preencher o campo **Registro Fiscal** na aba **Geral** do cadastro de **todos os Departamentos**. 
    
    Vale lembrar que o **departamento** é usado apenas para casos de tomadores de serviço.
    

**![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/38500911654935)Configuração das bases de cálculo**

*   Base IRRF → Evento **1904** com Identificação da base = **12**
    
*   Base INSS → Evento **1901** com Identificação da base = **8**
    

### **3\. Jornada de Uso**

1.  Acesse o **Gerenciador de Folhas** (Pessoal+ > Rotinas Folha).
    
2.  Filtre:
    
    *   Empresa;
        
    *   Referência;
        
    *   Tipo da folha;
        
    *   Status.
        

![](https://ajuda.sankhya.com.br/hc/article_attachments/17268683476759)

3.  Localize a folha calculada e clique sobre ela.
    
4.  Clique no botão **Resumo da Folha** (ícone da impressora).
    

![](https://ajuda.sankhya.com.br/hc/article_attachments/17268661235607)

5.  Configure o pop-up nas abas:
    

*   Empresas;
    
*   Geração;
    
*   Departamentos;
    
*   Ordenação Funcionários;
    
*   Funcionários.
    

![](https://ajuda.sankhya.com.br/hc/article_attachments/17268714344087)

Configure cada aba conforme a sua necessidade.

![](https://ajuda.sankhya.com.br/hc/article_attachments/17268706062359)

6.  Clique em:
    

*   **Download PDF** ou
    
*   **Pré-visualizar**
    

![resumo da folha.png](https://ajuda.sankhya.com.br/hc/article_attachments/35934417899031)

### **4\. Pontos de Atenção**

#### **✅ Parâmetros importantes**

*   **FPNOVORESUMOFOL**: habilita o novo layout do resumo.
    
    Quando este parâmetro está ligado, o sistema emite o resumo atualizado, com o layout mais recente.
    
*   **FPRELRESFOLHA**: define o código do modelo do relatório cadastrado na tela **Relatórios Formatados**.
*   **FPCOMPENSCAMPO9**: ativa a compensação dos valores referentes à **retenção de terceiros**.
    
    Quando habilitado, o sistema deduz automaticamente o valor retido nas notas das contribuições previdenciárias devidas no mês, incluindo valores de outras entidades e fundos. Isso permite compensar esses valores diretamente na competência.
    
*   **ZERARESC**: apresenta o valor líquido das rescisões que estiverem zeradas.
*   **ZERARFER**: apresenta o valor líquido das folhas de férias que estiverem zeradas.
    
    ![acesse também FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/38687128725143) Acesse o artigo [Zeramento de Férias e Rescisão no Resumo da Folha](https://ajuda.sankhya.com.br/hc/pt-br/articles/4544050476951) para melhor compreensão.
    

#### **✅ Valor Parte Empresa**

Certifique-se de que a opção **INSS Emp. Func:** esteja marcada na aba **Geral** do **Registro Fiscal** vinculado à empresa, bem como os percentuais dos tributos e encargos aplicáveis à empresa que irão compor os cálculos e guias.

#### **✅ Exibição do CNPJ da Filial no Relatório**

Para visualizar o **CNPJ da Filial** no relatório, a opção **Imprimir apenas totalizadores** não deve estar habilitada.

Quando essa opção estiver desmarcada, o relatório apresentará:

*   no primeiro cabeçalho, as informações da **Matriz**;
    
*   logo abaixo da **Competência**, os dados da **Filial**, incluindo o respectivo CNPJ.
    

Caso a opção esteja marcada, o sistema exibirá apenas os totalizadores, sem detalhar as informações por estabelecimento.

#### **✅ Contribuições Previdenciárias (INSS sobre a Receita Bruta)**

As **Contribuições Previdenciárias (INSS sobre a Receita Bruta)** somente serão apresentadas quando houver **valor maior que zero** informado no campo **“Valor do INSS da Receita Bruta”**, localizado na aba **Desoneração da Folha** do **Registro Fiscal**.

#### **✅ Retenção de terceiros**

Para que os valores referentes à **retenção de terceiros** sejam gerados **tanto na guia GPS quanto no Resumo da Folha**, é necessário garantir as seguintes configurações:

*   **Parâmetro FPCOMPENSCAMPO9 ligado**: esse parâmetro habilita a compensação dos valores de retenção de terceiros nas contribuições previdenciárias.
    
*   **Na geração da guia GPS**, a opção **Utiliza valor de retenção no 13º salário** deve estar desmarcada.  
    As retenções não se aplicam às folhas de 13º salário, portanto essa opção não deve ser marcada.
    
*   **Na geração do Resumo da Folha, os tipos de folha selecionados devem ser os mesmos utilizados na geração da GPS**, **exceto o tipo 13º Salário**, que **não deve ser incluído**, pois não participa dessa dedução.
    

#### **✅ PIS sobre a folha**

1.  Configurar na tela **Registro Fiscal**, aba **Geral**, que a **Empresa** é **Contribuinte**, informar o **Código de Receita** e o valor da **Alíquota**.
2.  Criar eventos com Bases de Cálculo configuradas:
    *   Evento Base PIS = 20
    *   Evento PIS = 114
    *   Desmarcar a opção Imprime em documentos para esses dois eventos.
    *   Vincular a [base de cálculo do PIS](https://ajuda.sankhya.com.br/hc/pt-br/articles/28240000315543-PIS-sobre-a-folha-de-pagamento#Basedec%C3%A1lculo) a todos os eventos que dependem dela.
3.  Cálculos confirmados
    *   Folha Mensal deve ter todos os eventos do item acima calculados individual ou coletivamente.
        

#### **✅ Licença-maternidade – Conferência de INSS e Compensação**

Os valores pagos a título de licença-maternidade **não possuem incidência de INSS patronal** e podem ser utilizados para **compensação**.

Se houver divergência nos valores apurados, realize as seguintes verificações:

1.  **Configuração dos eventos de licença-maternidade**
    
    Verifique se os eventos de licença gestante estão configurados com a **identificação** correta.
    
    Essa identificação é indispensável para que o **Resumo da Folha**, a **Guia GPS** e a **Integração com o Financeiro** realizem o cálculo correto da compensação e da apuração previdenciária.
    
2.  **Parâmetros na emissão do Resumo da Folha**
    
    Ao gerar o relatório, na aba **Resumos**, marque as opções:
    
    ✔ **Demonstrar Resumos de Previdência e FGTS**
    
    ✔ **Utiliza Valores de Retenção/Compensação de INSS**
    
    Essas opções são fundamentais para empresas que possuem valores de licença-maternidade a compensar, garantindo que o relatório apresente corretamente os valores previdenciários.
    

#### **✅ Rescisões**

Caso haja divergência entre o valor da multa do FGTS apresentado no resumo da rescisão e o valor exibido no FGTS Digital, verifique o evento utilizado no cálculo e a fórmula configurada para a multa.

### **5\. Dicas de Usabilidade**

*   Utilize os mesmos tipos de folha do processo de geração da GPS para manter a consistência das conferências.
    
*   Gere o resumo agrupado por Matriz/Filial para conferência com o eCAC.
    
*   Use o resumo por departamento apenas para análises internas detalhadas.
    
*   Revise as bases de cálculo dos eventos sempre que houver divergência de valores.
    

## **Artigos Relacionados**

*   [Gerenciador de Folhas](https://ajuda.sankhya.com.br/hc/pt-br/articles/4424800696599)
    
*   [Cadastro de Eventos e Bases de Cálculo](https://ajuda.sankhya.com.br/hc/pt-br/articles/33041194565911)