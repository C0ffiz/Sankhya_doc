# Cadastro de Tipo de Rescisão

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/38710044143895-Cadastro-de-Tipo-de-Rescis%C3%A3o](https://ajuda.sankhya.com.br/hc/pt-br/articles/38710044143895-Cadastro-de-Tipo-de-Rescis%C3%A3o)

---

# Cadastro de Tipo de Rescisão

**Módulo:** Pessoal+  
**Caminho de Acesso:** Pessoal+ > Cadastros  
**ID da Tela:** br.com.sankhya.rh.TipoRescisao

---

## **Descrição e Usabilidade**

### **1\. Descrição da Funcionalidade**

A tela **Tipo de Rescisão** é utilizada para cadastrar e configurar os diferentes motivos de desligamento utilizados no sistema.

Para cada tipo de rescisão, devem ser informados os códigos exigidos pelos órgãos governamentais, garantindo que:

*   O cálculo da rescisão seja adequado às indenizações e direitos do trabalhador;
    
*   As guias de FGTS sejam geradas de forma adequada;
    
*   As informações enviadas ao eSocial estejam consistentes;
    
*   As obrigações como RAIS e GFIP sejam atendidas corretamente.
    

### **2\. Pré-requisitos**

**Permissões necessárias**

*   Deve ter permissão para **consultar dados dos funcionários****.**
*   Deve **ter acesso liberado para a tela Tipo de Rescisão**. Essa liberação é feita na tela **Acessos** (Configurações > Controle de Acesso), pelo administrador do sistema.

**Configurações relacionadas**

Antes de cadastrar um **Tipo de Rescisão**, verifique:

*   Conhecimento do motivo legal do desligamento;
    
*   Consulta à [Tabela 19 – Motivos de Desligamento do eSocial](https://www.gov.br/esocial/pt-br/documentacao-tecnica/manuais/leiautes-esocial-v-1-1-beta/tabelas.html#19);
    
*   [Cadastro de Código de Afastamento para Rescisão](https://ajuda.sankhya.com.br/hc/pt-br/articles/13729923854487) realizado.
    

### **3\. Jornada de Uso**

![tipo-rescisao-p+.png](https://ajuda.sankhya.com.br/hc/article_attachments/38710122660375)

1.  Acesse a tela **Tipo de Rescisão** (Pessoal+ > Cadastros).
    
2.  Clique em ![Botão Novo FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/38710122661143) **Cadastrar Tipo de Rescisão**.
    
3.  Preencha:
    

<table class="wysiwyg-table-resized"><colgroup><col style="width: 21%;"> <col style="width: 50%;"> <col style="width: 29%;"></colgroup><tbody><tr><td style="background-color: #66cc66;"><strong>Campos</strong></td><td style="background-color: #66cc66;"><strong>Funcionalidade</strong></td><td style="background-color: #66cc66;"><strong>Observações</strong></td></tr><tr><td style="vertical-align: top;"><strong>Cód.Tipo Rescisão</strong></td><td style="vertical-align: top;">Identificador único do tipo de rescisão.</td><td><p data-start="1099" data-end="1243">Pode ser preenchido automaticamente ou manualmente, conforme a configuração do botão <img class="wysiwyg-image-resized" style="aspect-ratio: 65/32; width: 21.29%;" src="https://ajuda.sankhya.com.br/hc/article_attachments/42315327970711" alt="botão-configuração-da-tela-FINAL.jpg" width="65" height="32"> <strong data-start="1206" data-end="1242">Configuração da Tela &gt; Numeração</strong>.</p></td></tr><tr><td style="vertical-align: top;"><strong>Descrição</strong></td><td style="vertical-align: top;">Descrição detalhada do tipo de rescisão.</td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;" colspan="3"><strong>Aba Geral</strong></td></tr><tr><td style="vertical-align: top;"><strong data-start="1401" data-end="1429">Cód. Afastamento da RAIS</strong></td><td style="vertical-align: top;">Código de afastamento conforme tabela oficial do eSocial/RAIS.</td><td rowspan="3">É importante&nbsp;mencionar&nbsp;que para cada&nbsp;Tipo de Rescisão, há um&nbsp;<a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/13729923854487" target="_blank" rel="noopener noreferrer">Código de Afastamento</a>&nbsp;específico para Causa, FGTS e RAIS que devem ser devidamente informados, do contrário, o processo não será realizado corretamente.</td></tr><tr><td style="vertical-align: top;"><strong data-start="1432" data-end="1457">Cód. Afastamento FGTS</strong></td><td style="vertical-align: top;">Código de afastamento conforme tabela oficial do FGTS/Caixa.</td></tr><tr><td style="vertical-align: top;"><strong data-start="1460" data-end="1489">Cód. Causa do Afastamento</strong></td><td style="vertical-align: top;">Código de causa do afastamento conforme eSocial.</td></tr><tr><td style="vertical-align: top;"><strong data-start="1492" data-end="1513">Cód. Saque (FGTS)</strong></td><td style="vertical-align: top;"><p>Código de tipo de saque de FGTS permitido conforme a rescisão.</p><ul data-source-line="141"><li data-source-line="142" data-list-item-id="e289e7b9f848306330ac094f3b0db0415">Valores aceitos:<ul data-source-line="143"><li data-source-line="143" data-list-item-id="e6f08fdf96efabc3eef34ed902e740611"><code>S</code>&nbsp;ou&nbsp;<code>1</code>&nbsp;= Saque liberado imediatamente</li><li data-source-line="144" data-list-item-id="ec47679412ca6a98c822ea279dc5e3c9a"><code>N</code>&nbsp;ou&nbsp;<code>0</code>&nbsp;= Saque não permitido / Bloqueado</li><li data-source-line="145" data-list-item-id="e76225fcf65aa5bf2e9ce29dd94f1a8bf"><code>C</code>&nbsp;= Saque parcial permitido (contribuições)</li><li data-source-line="146" data-list-item-id="e77957ba43130f5b65f17647e1abf2a71"><code>T</code>&nbsp;= Saque total permitido (após período de carência)</li><li data-source-line="147" data-list-item-id="ed4a671135e3e4ef26154c0ca45f69250"><code>A</code>&nbsp;= Saque autorizado após liberação</li><li data-source-line="148" data-list-item-id="ee3ffe05326426868c9f3e2e11706159f"><code>M</code>&nbsp;= Saque multa (40% de multa)</li></ul></li><li data-source-line="149" data-list-item-id="ed2a8b8ca23fa273697909a6a062f4c2b">Determina se e quando o funcionário pode sacar:<ul data-source-line="150"><li data-source-line="150" data-list-item-id="e843467483ba2db9a1c99764759766843">Sem justa causa: Saque total + 40% de multa</li><li data-source-line="151" data-list-item-id="e53bd44cb58e2a0e752507aecd064a4e9">Com justa causa: Sem saque (bloqueado)</li><li data-source-line="152" data-list-item-id="e54a826bc2f9f2afbc4f34948a7eb95a7">Acordo: Saque total, sem multa</li><li data-source-line="153" data-list-item-id="eb58143e07c07e843f12d1cc3b01c3b28">Morte: Saque total pelos beneficiários</li></ul></li></ul></td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;"><strong data-start="1582" data-end="1608">Permite gerar previsão</strong></td><td style="vertical-align: top;">Indica se este tipo de rescisão permite gerar previsões de rescisão.</td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;"><strong data-start="1516" data-end="1547">Motivo desligamento eSocial</strong></td><td style="vertical-align: top;">Motivo técnico do desligamento conforme definições da tabela 19 do eSocial.</td><td>&nbsp;</td></tr></tbody></table>

4.  Clique em ![botão Salvar.FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/38710502496151) **Salvar (F7)**.
    

### **4\. Pontos de Atenção**

*   Os códigos de RAIS, FGTS e Causa devem estar alinhados ao motivo real da rescisão. Configuração incorreta pode gerar:
    
    *   Recolhimento indevido de FGTS;
        
    *   Geração apenas de GFIP sem GRRF;
        
    *   Inconsistências no eSocial.
        
        **Exemplo:** se uma Dispensa sem Justa Causa estiver configurada com código de FGTS de Pedido de Demissão, o recolhimento poderá ocorrer apenas via GFIP, sem geração de GRRF.
        
*   Sempre valide o **Motivo de desligamento eSocial** antes de utilizar o tipo no cálculo.
    
*   O cadastro do Tipo de Rescisão apenas configura os códigos no sistema. O envio ao eSocial acontece na **Central do eSocial**, após salvar e calcular a rescisão do funcionário.
    

### **5\. Dicas de Usabilidade**

*   Utilize descrições padronizadas para facilitar a identificação pelos usuários.
    
*   Revise os códigos sempre que houver atualização na legislação.
    
*   Teste a previsão antes de aplicar o tipo de rescisão em produção.
    

### **Artigos Relacionados**

*   [Aviso Prévio](https://ajuda.sankhya.com.br/hc/pt-br/articles/38693057310487)
    
*   [Cálculo de Rescisão](https://ajuda.sankhya.com.br/hc/pt-br/articles/5764158461847)