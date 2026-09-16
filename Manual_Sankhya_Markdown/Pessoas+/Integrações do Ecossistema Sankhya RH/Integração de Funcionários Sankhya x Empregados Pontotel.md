# Integração de Funcionários Sankhya x Empregados Pontotel

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/34973663307031-Integra%C3%A7%C3%A3o-de-Funcion%C3%A1rios-Sankhya-x-Empregados-Pontotel](https://ajuda.sankhya.com.br/hc/pt-br/articles/34973663307031-Integra%C3%A7%C3%A3o-de-Funcion%C3%A1rios-Sankhya-x-Empregados-Pontotel)

---

# Integração de Funcionários Sankhya x Empregados Pontotel

**Módulo**: Pessoas+ / Integrações  
**Caminho de Acesso**: Menu Principal > Integrações > Empregados > Sankhya x Pontotel

---

## **Sumário**

[Descrição e Usabilidade](#descri%C3%A7%C3%A3o-e-usabilidade)

*   [1\. Descrição da Funcionalidade](#1-descri%C3%A7%C3%A3o-da-funcionalidade)
*   [2\. Pré-requisitos](#2-pr%C3%A9-requisitos)
*   [3\. Diagrama de Fluxo](#3-diagrama-de-fluxo)
*   [4\. Jornada de Uso](#4-jornada-de-uso)
*   [5\. Pontos de Atenção](#5-pontos-de-aten%C3%A7%C3%A3o)
*   [6\. Dicas de Usabilidade](#6-dicas-de-usabilidade)
*   [7\. Casos de Uso](#7-casos-de-uso)

[FAQ – Dúvidas Frequentes](#faq-%E2%80%93-d%C3%BAvidas-frequentes)

[Artigos Relacionados](#artigos-relacionados)

---

## **Descrição e Usabilidade**

### **1\. Descrição da Funcionalidade**

A **integração de colaboradores entre Sankhya e Pontotel** automatiza o cadastro, atualização, transferência e demissão de funcionários, garantindo que as informações estejam sincronizadas entre os sistemas. 

O processo identifica funcionários não dispensados de ponto na Sankhya e cria ou atualiza os respectivos empregados na Pontotel, utilizando o código composto (CODEMP+CODFUNC) como referência. Isso elimina retrabalho manual, reduz inconsistências e agiliza a gestão de pessoal.

### **2\. Pré-requisitos**

*   **Permissões necessárias**
    *   Ter contratado e implementado o Pessoal+ e o Sankhya Om;
    *   Ter realizado o [setup de integração Sankhya/Pontotel](https://ajuda.sankhya.com.br/hc/pt-br/articles/34875102231063).
*   **Parâmetros essenciais**
    *   Habilitação do recurso Log de Alterações do Gateway (parâmetro LOGTABOPER - Ativar armazenamento de log de modificações em tab = ligado na tela Preferências do Sankhya Om).
*   **Configurações relacionadas**
    *   Base Sankhya online e responsiva durante as consultas.
    *   Token válido e URL atualizada no [Gateway](https://developer.sankhya.com.br/reference/requisi%C3%A7%C3%B5es-via-gateway).

### **3\. Diagrama de fluxo**

![fluxo-integ-empregados-sankhya-pontotel.png](https://ajuda.sankhya.com.br/hc/article_attachments/34973901412887)

### **4\. Jornada de Uso**

**4.1.** O usuário realiza o cadastro ou atualização do funcionário no Sankhya Om, preenchendo todos os campos obrigatórios para a integração (Empresa, CPF, Carga Horária, Departamento, Cidade de Trabalho, Sindicato).

**4.2.** Certifica de que o funcionário está em atividade normal e que não está dispensado de ponto.

![empregado-integ-sankhya-pontotel.png](https://ajuda.sankhya.com.br/hc/article_attachments/34974195744919)

**4.3.** Aguarda a execução automática da integração (a cada 12 horas). O sistema valida os dados e verifica se não há inconsistências.

**4.4.** O empregado é criado ou atualizado na Pontotel, refletindo as informações do Sankhya Om. Em caso de transferência ou demissão, o cadastro é atualizado conforme as regras do processo.

**4.6.** Campos integrados: funcionário (Sankhya) → empregado (Pontotel)

<table style="border-style: solid; border-width: 1px; margin-left: 0px; margin-right: auto;" class="wysiwyg-table-resized"><colgroup><col style="width: 26%;"> <col style="width: 28%;"> <col style="width: 46%;"></colgroup><tbody><tr><td style="background-color: #90ee90; border-style: solid; border-width: 1px;"><span style="color: #2F3941;"><strong>&nbsp; Campo Sankhya</strong></span></td><td style="background-color: #90ee90; border-style: solid; border-width: 1px;"><span style="color: #2F3941;"><strong>&nbsp; Campo Pontotel</strong></span></td><td style="background-color: #90ee90; border-style: solid; border-width: 1px;"><span style="color: #2F3941;"><strong>&nbsp; Descrição</strong></span></td></tr><tr><td style="border-style: solid; border-width: 1px;" colspan="3"><span style="color: #2F3941;">&nbsp; Tabelas consultadas no Sankhya: TFPFUNC, TFPFHO, TFPEMP, TFPFCO e TSICID</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Nome Funcionário</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Nome</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">Nome cadastrado na folha</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Dia apura ponto (Empresa)</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Dia de início da folha</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">Dia de apuração do ponto do cadastro da Empresa</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; CPF</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Senha Registro</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">CPF do cadastro. Pode ser alterado após a admissão.</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Departamento</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;" rowspan="2"><span style="color: #2F3941;">&nbsp; Local de Trabalho</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;" rowspan="2"><span style="color: #2F3941;">Concatenação da informação do departamento + cidade de trabalho do empregado</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Cidade de Trabalho</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Empresa</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Empregador</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">Empresa</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Sindicato</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Regra de Cálculo</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">Código do sindicato</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Data admissão</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Admissão</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">Data de admissão</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Carga Horária&nbsp;</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Escala</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">Código da carga horária</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Dia de início da Carga Horária</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Dia início da Escala</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">Dia de início da escala</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Código da Empresa</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;" rowspan="2"><span style="color: #2F3941;">&nbsp; Código</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;" rowspan="2"><span style="color: #2F3941;">Concatenação do código da empresa (CODEMP) com o código do funcionário (CODFUNC)</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Código do Funcionário</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; PIS</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; PIS</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">PIS válido (opcional)</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; RG</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Identidade</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">RG válido (opcional)</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; CTPS</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; CTPS</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">CTPS válida (opcional)</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Função</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Função</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">Função atribuída ao cadastro do empregado na Sankhya</span></td></tr><tr><td style="border-style: solid; border-width: 1px;"><span style="color: #2F3941;">&nbsp; Email</span></td><td style="border-style: solid; border-width: 1px;"><span style="color: #2F3941;">&nbsp; Email</span></td><td style="border-style: solid; border-width: 1px;"><span style="color: #2F3941;">Email válido (opcional)</span></td></tr></tbody></table>

### **5\. Pontos de Atenção**

*   O código do empregado (CODEMP+CODFUNC) não deve ser alterado manualmente na Pontotel, para manter a referência entre os sistemas.
*   Funcionários "Dispensados do Ponto" não são integrados.
*   Em caso de duplo vínculo, será feito um novo cadastro na Pontotel, sendo o PIN padrão o CPF + "1" ao final do mesmo.
*   Em caso de transferência, o cadastro atual é demitido e admitido um novo, com o mesmo PIN e informações atualizadas conforme consta no Sankhya Om.
*   Não há deleção automática: exclusões no Sankhya Om devem ser replicadas manualmente na Pontotel.
*   Alterações diretas na Pontotel serão sobrescritas pela próxima integração, caso não estejam atualizadas no Sankhya Om.
*   Transferências e demissões exigem que não haja batidas de ponto após a data de desligamento.
*   Se o log de alterações não estiver habilitado, a integração ocorrerá apenas na execução de consistência diária.

### **6\. Dicas de Usabilidade**

*   Utilizar filtros no Sankhya Om para visualizar apenas funcionários elegíveis à integração.
*   Manter o cadastro sempre atualizado para evitar falhas na sincronização.
*   Para autônomos ou funcionários dispensados de controle de ponto, marcar a opção **"Dispensado de Ponto"** no cadastro.
*   Realizar o setup completo da integração antes de habilitar o fluxo.

### **7\. Casos de Uso**

✅ **Exemplo Real:** 

Cadastro de novo funcionário no Sankhya Om com todos os dados obrigatórios preenchidos, integração automática e criação do empregado na Pontotel.

❌ **Erro Comum:** 

Alteração manual do código do empregado na Pontotel, causando perda de referência e duplicidade de cadastro.

## **FAQ – Dúvidas Frequentes**

1.  **O que acontece se um funcionário for dispensado de ponto na Sankhya?**
    
    Ele não será integrado à Pontotel.
    
2.  **Posso alterar o código do empregado na Pontotel?**
    
    Não. Isso causa perda de referência e duplicidade de cadastro.
    
3.  **Como tratar transferências e demissões?**
    
    O cadastro é atualizado conforme as regras, desde que não haja batidas de ponto após a data de desligamento.
    
4.  **E se o log de alterações não estiver habilitado?**
    
    A integração ocorrerá apenas na execução de consistência diária.
    

## **Artigos Relacionados**

*   [Setup inicial de integração Sankhya <> Pontotel](https://ajuda.sankhya.com.br/hc/pt-br/articles/34875102231063)
*   [Configuração Funcionários](https://ajuda.sankhya.com.br/hc/pt-br/articles/21069685487639)
*   [Integração de Empresas Sankhya x Empregadores Pontotel](https://ajuda.sankhya.com.br/hc/pt-br/articles/34891901568919)
*   [Integração de Locais de Trabalho Sankhya x Pontotel (Departamento + Cidade de Trabalho)](https://ajuda.sankhya.com.br/hc/pt-br/articles/34944782141207)
*   [Integração de Escalas Pontotel e Carga Horária Sankhya](https://ajuda.sankhya.com.br/hc/pt-br/articles/34981462276887)
*   [Integração de Férias Sankhya x Férias Pontotel](https://ajuda.sankhya.com.br/hc/pt-br/articles/35006040384023)
*   [Integração de Ocorrências Sankhya x Dispensas e Afastamentos Pontotel](https://ajuda.sankhya.com.br/hc/pt-br/articles/35032053719959)
*   [Integração de Usuários (Sankhya) x Usuários (Pontotel)](https://ajuda.sankhya.com.br/hc/pt-br/articles/35039187052951)
*   [Integração de Apontamentos e Faltas Pontotel x Verbas e Faltas Sankhya](https://ajuda.sankhya.com.br/hc/pt-br/articles/35056595712279)