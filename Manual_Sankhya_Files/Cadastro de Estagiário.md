# Cadastro de Estagiário

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/41826803259415-Cadastro-de-Estagi%C3%A1rio](https://ajuda.sankhya.com.br/hc/pt-br/articles/41826803259415-Cadastro-de-Estagi%C3%A1rio)

---

# Cadastro de Estagiário

**Módulo:** Pessoal+  
**Caminho de Acesso:** Pessoal+ > Cadastros > Configuração Funcionários  
**ID da Tela:** br.com.sankhya.cadastro.funcionarios

---

## **Descrição e Usabilidade**

### **1\. Descrição da Funcionalidade**

O cadastro de estagiário permite registrar estudantes contratados por meio de estágio obrigatório ou não obrigatório, conforme as regras previstas na legislação, garantindo que o sistema realize corretamente o tratamento desse tipo de vínculo durante os processos de folha de pagamento e integração com o eSocial.

O estágio **não caracteriza vínculo empregatício**, desde que sejam atendidos todos os requisitos estabelecidos pela **Lei nº 11.788/2008 (Lei do Estágio)**, como a celebração do Termo de Compromisso de Estágio (TCE), a supervisão da instituição de ensino e da concedente, além da compatibilidade entre as atividades desenvolvidas e o curso do estudante.

Por esse motivo, o cadastro do estagiário possui configurações específicas que o diferenciam de uma admissão regida pela Consolidação das Leis do Trabalho (CLT). Entre essas diferenças estão:

*   utilização de um padrão de cadastro específico para estagiários;
*   informação da **Bolsa Estágio** em substituição ao salário-base;
*   parametrizações próprias de contrato e regime trabalhista;
*   adequação das informações de lotação e cargo às atividades de estágio.

Embora o processo de cadastro seja semelhante ao de uma admissão convencional, essas configurações são indispensáveis para que o sistema execute corretamente os cálculos da folha, as obrigações legais e a geração dos eventos do eSocial.

### **2\. Pré-requisitos**

Antes de cadastrar um estagiário, verifique se:

*   possui permissão de acesso à tela **Configuração Funcionários** (Pessoal+ > Cadastros).  Essa liberação é feita na tela **Acessos** (Configurações > Controle de Acesso), pelo administrador do sistema;
*   o estudante possui Termo de Compromisso de Estágio (TCE) formalizado;
*   o cargo e a lotação destinados ao estágio já estão cadastrados;
*   o [padrão de cadastro](https://ajuda.sankhya.com.br/hc/pt-br/articles/41316403366551) para estagiários está disponível no sistema.

### **3\. Jornada de Uso**

#### **3.1 Cadastre o estagiário**

1.  Acesse a tela **Configuração Funcionários** (Pessoal+ > Cadastros);
    
2.  Após selecionar a **Empresa** desejada, clique no botão ![Botão Novo FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/41827522635287) **Cadastrar Funcionário**;
    
3.  Ao iniciar o cadastro, escolha se deseja fazer o cadastro utilizando um padrão cadastrado previamente ou sem padrão;
    
    ![padraofunc-estagiario.png](https://ajuda.sankhya.com.br/hc/article_attachments/41829233772439)
    
    <table style="background-color: #f4fdff; border-style: none; margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #E6F4EE; border-color: #006B3F;"><p><span data-markdown-start-index="1971">💡 </span><span style="color: hsl(155,100%,21%);"><span data-markdown-start-index="1971"><strong>Dica</strong></span></span></p><p><span data-markdown-start-index="1987">A seleção do padrão é recomendada, pois ele aplica automaticamente as parametrizações específicas para esse tipo de vínculo, reduzindo configurações manuais e evitando inconsistências na folha de pagamento e no eSocial.</span></p></td></tr></tbody></table>
    
4.  Preencha o **CPF** e o **Nome** do estagiário;
    
    <table style="background-color: #f4fdff; border-style: none; margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #f4fdff; border-color: #185FA5;"><p><span data-markdown-start-index="1971">ℹ️</span><span data-markdown-start-index="1971">&nbsp;</span><span style="color: #640A8E;"><span data-markdown-start-index="1980"><strong>Notas</strong></span></span></p><ul><li data-list-item-id="e52be1e0ea94aad046fec33d8ffeb4e43">O preenchimento da&nbsp;<strong>Matrícula</strong>&nbsp;depende da configuração do campo&nbsp;<strong data-start="124" data-end="175">Gera Matrícula do Funcionário automaticamente</strong>, disponível na aba&nbsp;<strong data-start="195" data-end="217">Informações Gerais</strong>&nbsp;da tela&nbsp;<strong data-start="226" data-end="238">Empresas </strong>(Pessoal+ &gt; Cadastros).</li><li data-list-item-id="e9a0eebe05bfd783a4bf5fb9b0852a0f7"><p>O campo&nbsp;<strong data-start="249" data-end="259">Código</strong>&nbsp;pode ser preenchido automaticamente ou manualmente, conforme a configuração definida no botão&nbsp;<strong data-start="393" data-end="417">Configuração da Tela</strong>, opção&nbsp;<strong data-start="425" data-end="438">Numeração</strong>.</p><p>Ao ativar o parâmetro&nbsp;<strong data-start="481" data-end="555" data-is-only-node="">Utiliza Sequência do Cód. Funcionário por Empresa? – FPCODFUNCPOREMP</strong>, o sistema gera uma sequência de códigos exclusiva para cada empresa. Caso contrário, será única para todas as empresas.</p><p>📚 Para saber mais, acesse <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/41317860396823" target="_blank" rel="noopener noreferrer">Definição da Numeração dos Cadastros no Pessoal+</a>.</p></li></ul></td></tr></tbody></table>
    
5.  Após preencher os dados cadastrais obrigatórios, acesse a aba **Contrato** e informe o valor da **Bolsa Estágio / Pró-Labore**;
    
    ![bolsaestagio-estagiario.png](https://ajuda.sankhya.com.br/hc/article_attachments/41829283438487)
    
    <table style="margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #FAEEDA; border-color: #854F0B;"><p><strong style="color: #633806;">⚠️ </strong><span style="color: hsl(32,89%,21%);"><strong style="color: #633806;">Atenção</strong></span></p><p><span data-markdown-start-index="2682">Estagiários não possuem salário-base. O pagamento é realizado por meio da Bolsa Estágio, conforme previsto no Termo de Compromisso de Estágio.</span></p></td></tr></tbody></table>
    
6.  Acesse a aba **Lotação** e selecione o **Cargo** compatível com as atividades desenvolvidas pelo estagiário;
    
    ![cargo-estagiario.png](https://ajuda.sankhya.com.br/hc/article_attachments/41829348633111)
    
    Essas informações devem refletir as atividades previstas no Termo de Compromisso de Estágio.
    
7.  Na aba **Admissão**, informe o regime trabalhista conforme o tipo de vínculo de estágio:
    
    ![admissao-estagiario.png](https://ajuda.sankhya.com.br/hc/article_attachments/41830266289175)
    
    *   **Código de Categoria para o eSocial**: 901 - Estagiário;
        
    *   **Situação no eSocial**: Oficial (S-2200/S-2300);
        
    *   **Vínculo**: 02 - Estagiário;
        
    *   **Regime Trabalhista**: CLT - Consolidação das Leis de Trabalho;
        
    *   **Regime de Jornada**: Submetidos Horário Trabalho (Cap. II CLT);
        
    *   **Regime Previdenciário**: RGPS - Regime Geral Previdência Social;
        
    *   **Tabela de Categoria \[FGTS\]**: 00 Estagiários.
        
8.  Na seção **Período de Experiência**, marque **Dispensado da Experiência**, pois não se aplica contrato de experiência para essa contratação;
    
9.  Na aba **Estágio**, preencha os dados do Termo de Compromisso de Estágio (TCE);
    
    ![abaestagio-estagiario.png](https://ajuda.sankhya.com.br/hc/article_attachments/41829437586711)
    
10.  Após preencher todas as informações obrigatórias:
     
     *   revise os dados informados;
         
     *   clique em **Salvar**.
         
         O estagiário estará apto para participar dos processos da folha de pagamento de acordo com as regras aplicáveis ao estágio.
         

#### **3.2 Envio ao eSocial**

Após concluir o cadastro do estagiário, acesse a **Central do eSocial** (Pessoal+ > Rotinas Folha) para gerar e enviar o evento **S-2300 – Trabalhador Sem Vínculo de Emprego/Estatutário**, responsável por comunicar ao eSocial o ingresso do estagiário na empresa.

O envio desse evento depende de:

*   cadastro do estagiário concluído;
*   informações contratuais preenchidas corretamente;
*   categoria do trabalhador configurada como **901 – Estagiário**;
*   configurações do ambiente do eSocial devidamente parametrizadas.

Após a geração do evento, acompanhe seu processamento pela **Central do eSocial**, verificando se o retorno foi recepcionado com sucesso.

<table style="margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #FAEEDA; border-color: #854F0B;"><p><strong style="color: #633806;">⚠️ </strong><span style="color: hsl(32,89%,21%);"><strong style="color: #633806;">Atenção</strong></span></p><p>O estagiário <strong data-start="1090" data-end="1121">não utiliza o evento S-2200</strong>, destinado aos trabalhadores com vínculo empregatício. Como o estágio não gera vínculo de emprego, sua admissão é comunicada exclusivamente por meio do <strong data-start="1274" data-end="1291">evento S-2300</strong>, conforme as regras do eSocial.</p></td></tr></tbody></table>

### **4\. Pontos de Atenção**

*   O estágio não gera vínculo empregatício quando observados os requisitos da Lei nº 11.788/2008.
*   O cadastro deve ser realizado utilizando o padrão específico para estagiários.
*   Estagiários recebem Bolsa Estágio, e não salário-base.
*   O cargo e a lotação devem ser compatíveis com as atividades previstas no estágio.
*   Informações incorretas podem impactar o processamento da folha e a geração dos eventos do eSocial.

### **5\. Dicas de Usabilidade**

*   Utilize sempre o padrão de cadastro de estagiário.
*   Revise o valor da Bolsa Estágio antes de concluir o cadastro.
*   Mantenha os dados do Termo de Compromisso de Estágio atualizados.
*   Verifique se o cargo está compatível com as atividades exercidas pelo estudante.

## **Perguntas Frequentes (FAQ)**

**1\. O estagiário possui vínculo empregatício?**

Não. O estágio não gera vínculo empregatício quando atende aos requisitos previstos na Lei nº 11.788/2008.

**2\. O estagiário possui salário-base?**

Não. O pagamento é realizado por meio da Bolsa Estágio.

**3\. Posso utilizar um cadastro padrão de empregado CLT para estagiários?**

Não é recomendado. Utilize sempre o padrão específico para estagiários para que o sistema aplique automaticamente as parametrizações necessárias.

**4\. É obrigatório informar a Bolsa Estágio?**

Sim. Esse valor é utilizado pelo sistema durante o processamento da folha.

**5\. O cargo influencia o cadastro do estagiário?**

Sim. O cargo deve ser compatível com as atividades previstas no estágio e com o Termo de Compromisso.

**6\. O estagiário é enviado ao eSocial?**

Sim. O cadastro deve seguir as regras vigentes do eSocial para essa categoria de trabalhador, conforme o tipo de vínculo informado.

## **Artigos Relacionados**

*   [Cadastro de Funcionários](https://ajuda.sankhya.com.br/hc/pt-br/articles/21069685487639)
*   [Central do eSocial](https://ajuda.sankhya.com.br/hc/pt-br/articles/7064222145175)
*   [Requisição de Transferência - Transferência de estagiário](https://ajuda.sankhya.com.br/hc/pt-br/articles/30772702977431)