# Integração de Apontamentos e Faltas Pontotel x  Verbas e Faltas Sankhya

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/35056595712279-Integra%C3%A7%C3%A3o-de-Apontamentos-e-Faltas-Pontotel-x-Verbas-e-Faltas-Sankhya](https://ajuda.sankhya.com.br/hc/pt-br/articles/35056595712279-Integra%C3%A7%C3%A3o-de-Apontamentos-e-Faltas-Pontotel-x-Verbas-e-Faltas-Sankhya)

---

# Integração de Apontamentos e Faltas Pontotel x Verbas e Faltas Sankhya

**Módulo**: Pessoas+ / Integrações  
**Versão Mínima**: Pessoal+ 5.1.0  
**Caminho de Acesso**: Pontotel > Gestão > Relatórios e Registros > Exportações: E02 - Arquivo para importação de apontamentos

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

A **integração de apontamentos e faltas entre Pontotel e Sankhya permite que os dados de fechamento da folha (verbas e faltas) parametrizados na Pontotel sejam enviados diretamente para o Sankhya Om**, eliminando a necessidade de exportação manual de arquivos. 

O processo pode ser realizado por meio de exportação de arquivo ou, de forma mais ágil, pelo acionamento de um botão na Pontotel, que registra os dados automaticamente nas tabelas do Sankhya Om.

### **2\. Pré-requisitos**

*   **Permissões necessárias**
    *   Ter contratado e implementado o Pessoal+ e o Sankhya Om.
    *   Ter realizado o [setup de integração Sankhya/Pontotel](https://ajuda.sankhya.com.br/hc/pt-br/articles/34875102231063).
*   **Parâmetros essenciais**
    *   Parametrização de verbas na Pontotel (E02).
    *   Módulo Pessoal+ atualizado na versão 5.1.0 ou superior.
*   **Configurações relacionadas**
    *   Base Sankhya online e responsiva durante as consultas.
    *   Token válido e URL atualizada no [Gateway](https://developer.sankhya.com.br/reference/requisi%C3%A7%C3%B5es-via-gateway).
    *   O período da folha deve estar aberto no Sankhya Om.
    *   O código do empregado na Pontotel deve seguir o padrão: código do empregador + código do funcionário no Sankhya Om.

### **3\. Diagrama de fluxo**

![fluxo-apontamento-faltas-integracao.png](https://ajuda.sankhya.com.br/hc/article_attachments/35056729668119)

### **4\. Jornada de Uso**

**4.1.** O usuário efetua o fechamento da folha normalmente na Pontotel.

**4.2.** Acessa **Gestão > Relatórios e Registros > Exportações: E02 - Arquivo para importação de apontamentos** e gera o arquivo (.txt ou .xls) de apontamentos para validação dos dados do período.

![relatorio-faltas-pontotel.png](https://ajuda.sankhya.com.br/hc/article_attachments/35060117067799)

**4.3.** Após a validação, seleciona a opção "Integrar verbas e faltas". 

Os dados do arquivo são enviados diretamente ao Sankhya Om, sem necessidade de exportar da Pontotel e importar no outro sistema.

**4.4.** Acompanha o status da integração pelo ícone de notificações (sininho).

![acompanhamento-integracao-falta.png](https://ajuda.sankhya.com.br/hc/article_attachments/35060717154327)

**4.5**. Consulta o relatório gerado para verificar sucessos e falhas.

O relatório gerado mostra, na aba "Sucessos", os valores integrados para cada empregado, tanto para verbas quanto para faltas.

Quando os colchetes aparecem vazios "\[\]", significa que o empregado foi considerado, mas não há valores para envio no período integrado.

![relatorio-empregrados-pontotel.png](https://ajuda.sankhya.com.br/hc/article_attachments/35060717156759)

Na aba "Falhas", o relatório mostra os empregados que tiveram problemas no envio dos valores para o Sankhya Om, com o motivo do ocorrido.

Caso queira visualizar no Pessoas+ os valores integrados, acessa a tela Lançamento de Movimento para as verbas e Faltas para as faltas.

#### **Faltas**

Somente as ocorrências de faltas existentes na folha do empregado na Pontotel serão integradas para a TFPFAL do Sankhya Om.

![faltas-integradas-sankhya.png](https://ajuda.sankhya.com.br/hc/article_attachments/35059345832215)

![Atenção FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/35059414778775) Débitos de banco de horas não são considerados faltas para integração.

O DSR utiliza a função _FaltasPeriodo_ no Sankhya Om para buscar registros na tabela TFPFAL e identificar faltas, dias de desconto de DSR ou férias, permitindo descontos sem parametrização de apontamento/verba na Pontotel.

Antes de ativar a integração, deve-se verificar se já utiliza os dados da tabela TFPFAL nos cálculos da Sankhya (faltas, descontos de DSR e férias) e se há verba parametrizada na Pontotel para calcular faltas e descontos de DSR, evitando, cálculos e descontos duplicados.

#### **Faltas e Suspensões**

Para que faltas derivadas de suspensões sejam integradas, é necessário que a folha do empregado na Pontotel tenha as duas sinalizações: falta e suspensão.

![falta-suspensao-integracao.png](https://ajuda.sankhya.com.br/hc/article_attachments/35059609582103)

Com ambas as sinalizações, a falta é enviada ao Sankhya Om para registro na TFPFAL com a informação de que se refere a uma suspensão.

O próprio Sankhya Om, ao identificar que é suspensão, reflete esse lançamento automaticamente no histórico de ocorrências do colaborador.

#### **Dados integrados**

Os dados Código de Empresa e Código de Funcionário são contemplados também, para a identificação do colaborador ao qual a verba e/ou falta se refere.

**Verbas**

<table style="background-color: transparent; border-collapse: collapse; border-spacing: 0px; border-style: solid; border-width: 1px; margin-left: 0px; margin-right: auto;" class="wysiwyg-table-resized"><colgroup><col style="width: 28%;"> <col style="width: 52%;"> <col style="width: 20%;"></colgroup><tbody><tr><td style="background-color: #90ee90; border-style: solid; border-width: 1px; padding: 0px;"><strong>&nbsp; Dado</strong></td><td style="background-color: #90ee90; border-style: solid; border-width: 1px; padding: 0px;"><strong>&nbsp; O que é</strong></td><td style="background-color: #90ee90; border-style: solid; border-width: 1px; padding: 0px;"><strong>&nbsp; Exemplo</strong></td></tr><tr><td style="border-style: solid; border-width: 1px; padding: 0px; vertical-align: middle;" colspan="3"><span style="color: #2F3941;">&nbsp; Tabela onde os dados são registrados: TFPMOV</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Código do evento</span></td><td style="border-style: solid; border-width: 1px; padding: 0px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; &nbsp; Código da verba</span></td><td style="border-style: solid; border-width: 1px; padding: 0px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; &nbsp; 1234</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Data da alteração</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Data da integração</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; 01/12/2023</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Referência</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Período relativo aos movimentos</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Novembro</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Tipo do evento</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Provento (1) / Base (0) / Desconto (-1)</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; 0</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Tipo de movimento</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Mensal (M)</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; M</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Unidade</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Horas (H) / Dias (D)</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; D</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Índice</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Valor da verba</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; 20.10</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Sequência</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Valor fixo</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; 500</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Valor movimentação</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Valor fixo</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; 0</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Código usuário</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Código usuário de integração</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; 0</span></td></tr></tbody></table>

**Faltas**

<table style="background-color: transparent; border-collapse: collapse; border-spacing: 0px; border-style: solid; border-width: 1px; margin-left: 0px; margin-right: auto;" class="wysiwyg-table-resized"><colgroup><col style="width: 23%;"> <col style="width: 57%;"> <col style="width: 20%;"></colgroup><tbody><tr><td style="background-color: #90ee90; border-style: solid; border-width: 1px; padding: 0px;"><strong>&nbsp; Dado</strong></td><td style="background-color: #90ee90; border-style: solid; border-width: 1px; padding: 0px;"><strong>&nbsp; O que é</strong></td><td style="background-color: #90ee90; border-style: solid; border-width: 1px; padding: 0px;"><strong>&nbsp; Exemplo</strong></td></tr><tr><td style="border-style: solid; border-width: 1px; padding: 0px; vertical-align: middle;" colspan="3"><span style="color: #2F3941;">&nbsp; Tabela onde os dados são registrados: TFPFAL</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Data</span></td><td style="border-style: solid; border-width: 1px; padding: 0px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; &nbsp; Data da ocorrência da falta</span></td><td style="border-style: solid; border-width: 1px; padding: 0px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; &nbsp; 01/11/2023</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Tipo</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Tipo do registro</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; -1</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Data da alteração</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Data da integração</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; 01/12/2023</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Origem</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Origem do lançamento (Ponto, "P")</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; P</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Horas</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Quantidade de horas de jornada prevista na data</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; 8</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Código usuário</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Código usuário de integração</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; 698</span></td></tr><tr><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; SUSPDISCIPLINAR</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; Indica se a falta é relativa a uma suspensão</span></td><td style="border-style: solid; border-width: 1px; vertical-align: middle;"><span style="color: #2F3941;">&nbsp; S</span></td></tr></tbody></table>

### **5\. Pontos de Atenção**

*   Os valores de verbas só serão registrados no Sankhya Om se o período estiver aberto e o funcionário não tiver folha calculada.
*   Para integrar valores de períodos fechados, é necessário reabri-lo no Sankhya Om.
*   Para funcionários com folha já calculada, exclua os valores existentes antes de integrar novamente.
*   Só serão integradas faltas que existam na folha do empregado e não estejam registradas no Sankhya Om.
*   Faltas derivadas de suspensões exigem identificação de ambos os eventos na folha.
*   Faltas referentes a débito de banco de horas não são integradas.
*   Se o valor calculado para a verba for zero, não será integrado.

### **6\. Dicas de Usabilidade**

*   Antes de integrar, deve-se gerar e validar o arquivo de apontamentos para evitar erros.
*   Integrar inicialmente apenas um local de trabalho para validação e travar a folha dos empregados antes do envio para garantir integridade dos dados.
*   Utilizar o relatório de integração para identificar e corrigir eventuais falhas.

### **7\. Casos de Uso**

✅ **Exemplo Real:** 

Integração de verbas e faltas de um período aberto para funcionários sem folha calculada, com validação prévia dos dados.

  
❌ **Erro Comum:** 

Tentativa de integração para período fechado ou funcionário com folha já calculada, resultando em falha no registro.

## **FAQ – Dúvidas Frequentes**

1.  **Posso integrar verbas para períodos fechados?**
    
    Não. É necessário reabrir o período no Sankhya Om antes da integração.
    
2.  **O que fazer se o funcionário já tiver folha calculada?**
    
    Exclua os valores existentes para permitir novo registro pela Pontotel.
    
3.  **Como validar se as faltas foram integradas corretamente?**
    
    Consulte o relatório de integração e verifique os lançamentos no Sankhya Om.
    
4.  **Faltas por suspensão são integradas automaticamente?**
    
    Sim, desde que ambas as sinalizações (falta e suspensão) estejam presentes na folha do empregado.
    
5.  **O que acontece se o valor da verba for zero?**
    
    Não será integrado ao Sankhya Om.
    

## **Artigos Relacionados**

*   [Ocorrências](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044610494)
*   [Faltas](https://ajuda.sankhya.com.br/hc/pt-br/articles/4408248097047)
*   [Setup inicial de integração Sankhya <> Pontotel](https://ajuda.sankhya.com.br/hc/pt-br/articles/34875102231063)
*   [Integração de Empresas Sankhya x Empregadores Pontotel](https://ajuda.sankhya.com.br/hc/pt-br/articles/34891901568919)
*   [Integração de Funcionários Sankhya x Empregados Pontotel](https://ajuda.sankhya.com.br/hc/pt-br/articles/34973663307031)
*   [Integração de Locais de Trabalho Sankhya x Pontotel (Departamento + Cidade de Trabalho)](https://ajuda.sankhya.com.br/hc/pt-br/articles/34944782141207)
*   [Integração de Escalas Pontotel e Carga Horária Sankhya](https://ajuda.sankhya.com.br/hc/pt-br/articles/34981462276887)
*   [Integração de Férias Sankhya x Férias Pontotel](https://ajuda.sankhya.com.br/hc/pt-br/articles/35006040384023)
*   [Integração de Ocorrências Sankhya x Dispensas e Afastamentos Pontotel](https://ajuda.sankhya.com.br/hc/pt-br/articles/35032053719959)
*   [Integração de Usuários (Sankhya) x Usuários (Pontotel)](https://ajuda.sankhya.com.br/hc/pt-br/articles/35039187052951)