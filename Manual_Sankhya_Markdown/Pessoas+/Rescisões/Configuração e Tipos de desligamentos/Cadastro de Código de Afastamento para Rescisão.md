# Cadastro de Código de Afastamento para Rescisão

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/13729923854487-Cadastro-de-C%C3%B3digo-de-Afastamento-para-Rescis%C3%A3o](https://ajuda.sankhya.com.br/hc/pt-br/articles/13729923854487-Cadastro-de-C%C3%B3digo-de-Afastamento-para-Rescis%C3%A3o)

---

# Cadastro de Código de Afastamento para Rescisão

**Módulo:** Pessoal+  
**Caminho de Acesso:** Pessoal+ > Cadastros   
**ID da Tela:** br.com.sankhya.rh.CodigoAfastamento

---

## **Descrição e Usabilidade**

### **1\. Descrição da Funcionalidade**

O **Código de Afastamento** é utilizado para identificar os diferentes tipos de desligamento ou afastamento do funcionário, como licenças, transferências, afastamentos legais, entre outros.

Ele é fundamental para garantir que as informações enviadas aos órgãos oficiais estejam corretas, especialmente em relação a:

*   eSocial (eventos de desligamento);
    
*   FGTS;
    
*   RAIS;
    
*   TRCT – Termo de Rescisão de Contrato de Trabalho.
    

#### **Base legal**

A correta classificação do afastamento está relacionada às seguintes normas:

*   Consolidação das Leis do Trabalho (CLT);
    
*   Manual de Orientação do eSocial (evento S-2299 – Desligamento);
    
*   Manual da RAIS;
    
*   Manual da GRRF/FGTS;
    
*   Layout oficial do TRCT.
    

Cada tipo de desligamento possui regras específicas quanto a direitos trabalhistas (aviso prévio, 13º salário, férias, multa do FGTS, entre outros).

Essa tela é utilizada para cadastrar e parametrizar esses códigos conforme as regras da empresa.

![Código-de-afastamento.png](https://ajuda.sankhya.com.br/hc/article_attachments/17849034004247)

### **2\. Pré-requisitos**

**Permissões necessárias**

*   Deve **ter acesso liberado para a tela Código de Afastamento**. Essa liberação é feita na tela **Acessos** (Configurações > Controle de Acesso), pelo administrador do sistema.

### **3\. Jornada de Uso**

1.  Acesse a tela **Código de Afastamento** (Pessoal+ > Cadastros).
    
2.  Clique em ![Botão Novo FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/38662170824855) **Cadastrar Códigos de Afastamento**.
    
3.  Preencha os campos:
    
    *   **Cód. Afastamento**: informe um código numérico interno para identificação no sistema.
    *   **Descrição**: preencha um nome claro que identifique o motivo do afastamento.
    *   **Código Governamental**: informe o código oficial correspondente ao motivo do afastamento.
4.  Na aba **Geral**, configure os direitos aplicáveis ao afastamento:
    
    <table class="wysiwyg-table-resized"><colgroup><col style="width: 27%;"> <col style="width: 42%;"> <col style="width: 31%;"></colgroup><tbody><tr><td style="background-color: #66cc66;"><strong>Campo</strong></td><td style="background-color: #66cc66;"><strong>Funcionalidade</strong></td><td style="background-color: #66cc66;"><strong>Observação</strong></td></tr><tr><td><strong>Direito a férias com menos de um ano</strong></td><td><p>Indica se o afastamento gera direito a férias proporcionais em caso de saída antes de um ano.</p><ul data-source-line="104"><li data-source-line="104" data-list-item-id="e59e60a39cb4e8ac7ffb272aa14454839">Marcado: funcionário tem direito a férias proporcionais mesmo não completando um ano.</li><li data-source-line="105" data-list-item-id="ee181dc49b77455a924341e6f2ba2d641">Desmarcado: sem direito a férias proporcionais antes de um ano completo.</li></ul></td><td><ul data-source-line="104"><li data-source-line="106" data-list-item-id="e46ccf3f1b429244f7209cb1b2aeb15a1">Afeta cálculo de verbas rescisórias para afastamentos curtos.</li><li data-source-line="107" data-list-item-id="eef6e5bdf88b94e2112fc65e2650a3329"><p>Importante para validação de legislação trabalhista (CLT Art. 146-148).</p><p>Exemplo: marcar para licenças remuneradas; desmarcar para afastamentos não remunerados.</p></li></ul></td></tr><tr><td><strong>Direito ao aviso prévio</strong></td><td><p>Define se o colaborador tem direito a aviso prévio durante este afastamento.</p><ul data-source-line="92"><li data-source-line="92" data-list-item-id="e30eefdaa617471966f0107c526b9bf9a">Marcado: o sistema obrigará o cumprimento de aviso prévio;</li><li data-source-line="93" data-list-item-id="e8f2a5b4950e81794b5110619db1d23e2">Desmarcado: não há obrigatoriedade de aviso prévio.</li></ul></td><td><ul data-source-line="92"><li data-source-line="94" data-list-item-id="eb17d5311adcab5fe3f5fc2b74545cb9e">Afeta o cálculo de dias de aviso prévio indenizado (se rescindir durante afastamento).</li><li data-source-line="94" data-list-item-id="eac11d096d107c1156dcf72c81d1e976f"><p>Integrado com cálculo de indenizações trabalhistas.</p><p>Exemplo: marcar para demissões; desmarcar para afastamentos que não geram rescisão.&nbsp;</p></li></ul></td></tr><tr><td><strong>Abate nos meses das médias</strong></td><td><p>Define se o período de afastamento deve ser excluído do cálculo de médias salariais.</p><ul data-source-line="113"><li data-source-line="116" data-list-item-id="e3a157ce969691d86773d7573e82efb2f">Marcado: o mês/período é desconsiderado para cálculos de médias.</li><li data-source-line="116" data-list-item-id="edfc3a07d69c4eff4fd8c91e6e8d8e0b5">Desmarcado: o período é incluído normalmente nas médias.</li></ul></td><td><ul data-source-line="116"><li data-source-line="118" data-list-item-id="e91fea14104608f9d82ce9c6ed3680c9b"><p>Afeta cálculos de:</p><ul data-source-line="119"><li data-source-line="119" data-list-item-id="e07ebd14450270a8aba3bba1c5af1491a">gratificações semestrais ou anuais;</li><li data-source-line="120" data-list-item-id="e67b7a7373539f47b271cbee00f7b851a">bônus baseados em média;</li><li data-source-line="121" data-list-item-id="e3107f7021dbce9d739f46cc6f92782ce">médias para contribuições previdenciárias.</li></ul><p>Exemplo: marcar para afastamentos não remunerados ou sem atividade; desmarcar para períodos normais.</p></li><li data-source-line="123" data-list-item-id="ef5df988bb314cff1b0f817f1d9cf3eb2">Importante para garantir justiça em benefícios baseados em médias.</li></ul></td></tr><tr><td><strong>Direito ao décimo terceiro</strong></td><td><p>Indica se o afastamento gera direito ao pagamento de décimo terceiro salário.</p><ul data-source-line="80"><li data-source-line="80" data-list-item-id="edbe29e0c500a985d8bbc1aad8edfc08c">Marcado: o período de afastamento é contabilizado para cálculo de 13º;</li><li data-source-line="81" data-list-item-id="e6ab99525dad7af16b524ecd8fd131150">Desmarcado: o período não conta para o 13º.</li></ul></td><td><ul><li data-list-item-id="e1cdbcb9280b16a5030151036baa05505"><p>Afeta o cálculo do décimo terceiro proporcional.</p><p>Exemplo: marcar para férias e licenças remuneradas; desmarcar para faltas injustificadas.</p></li></ul></td></tr><tr><td><strong>Direito à multa do FGTS</strong></td><td>Indica se o funcionário tem direito à multa de 40% sobre o saldo do FGTS durante este afastamento</td><td><ul data-source-line="68"><li data-source-line="70" data-list-item-id="ec621d25d002309dc2ee54c7512e31845">Afeta cálculos automaticamente no processamento de folha.</li><li data-source-line="71" data-list-item-id="e988417f435f770ed6cba9553f3489490"><p>Importante para afastamentos que resultam em rescisão.</p><p>Exemplo: marcar para demissões sem justa causa; desmarcar para afastamentos temporários.</p></li></ul></td></tr></tbody></table>
    
5.  Selecione o **Tipo de Tabela** conforme a finalidade do código:
    *   RAIS;
        
    *   Causa do afastamento;
        
    *   FGTS.
        
6.  O **Código HomologNet** corresponde ao campo **"22 – Causa do Afastamento"** do arquivo TRCT.
    
    ⚠️ É obrigatório quando o **Tipo de Tabela** for **Causa do afastamento**.
    
    A lista já está fixa no sistema, sendo necessário apenas selecionar a opção correspondente.
    
    Essa configuração é feita uma única vez e será utilizada sempre que o código for aplicado.
    
7.  Finalizado o cadastro, clique em ![botão Salvar.FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/23967315950999) **Salvar \[F7\]**.

**Exemplo:** Demissão Sem Justa Causa

**Código:** 60

**Descrição:** Demissão sem justa causa

**Código Governamental**: 31

**Tipo de Tabela**: Causa do Afastamento

**Direitos**:

✓ **Multa FGTS** (Sim - 40%)

✓ **Décimo Terceiro** (Sim)

✓ **Aviso Prévio** (Sim ou indenizado)

✓ **Férias < 1 ano** (Sim)

☐ **Abate em Médias** (Não)

<table><tbody><tr><td style="background-color: #f6fcf5;"><p>Onde esse cadastro é utilizado no sistema:</p><p>1️⃣ <strong>Tela Cálculos de Rescisão</strong></p><p>Ao realizar uma rescisão na rotina de cálculo, o sistema utilizará o &nbsp;Código de Afastamento para:</p><ul><li data-list-item-id="ed488ae5d898e8761494442c0bd67181b">Determinar os direitos do funcionário;</li><li data-list-item-id="ed5f0d0d869e3d5021bc59aac5600ce90">Aplicar regras de cálculo (aviso, médias, 13º, multa FGTS);</li><li data-list-item-id="ea2a59a64c169bc0b0b7b77c995ba0e62">Definir o motivo enviado ao eSocial;</li><li data-list-item-id="e52341d32f96328c6104ad44e302090b9">Preencher informações no TRCT.</li></ul><p>2️⃣ <strong>Aba Afastamento da tela Configuração Funcionários</strong></p><p>No cadastro do funcionário, o Código de Afastamento selecionado será vinculado ao histórico do funcionário, registrando oficialmente o motivo do desligamento.</p><p>Essa informação passa a compor o histórico funcional e será utilizada em obrigações legais.</p></td></tr></tbody></table>

### **4\. Pontos de Atenção**

*   O Código Governamental deve estar alinhado com a legislação vigente.
    
*   Alterações em códigos já utilizados podem impactar históricos e obrigações transmitidas.
    
*   Sempre valide a parametrização antes de fechar a folha.
    
*   O **Tipo de Tabela** **Causa do afastamento** exige preenchimento do **Código HomologNet**.
    
*   Inconsistências podem gerar:
    
    *   rejeição no evento S-2299 do eSocial;
        
    *   divergências na GRRF;
        
    *   problemas no TRCT.
        
*   O cadastro dos Códigos de Rescisão apenas configura os códigos no sistema. O envio ao eSocial acontece na **Central do eSocial**, após salvar e calcular a rescisão do funcionário.
    

### **5\. Dicas de Usabilidade**

*   Utilize descrições padronizadas.
    
*   Evite duplicidade de códigos para o mesmo motivo.
    
*   Revise a parametrização junto ao contador antes de criar novos códigos.
    
*   Realize testes em ambiente de homologação quando houver mudanças.
    

### **Artigos Relacionados**

*   [Como realizar uma rescisão no sistema](https://ajuda.sankhya.com.br/hc/pt-br/articles/5764158461847)
    
*   [Gerenciador de Folhas](https://ajuda.sankhya.com.br/hc/pt-br/articles/4424800696599)
    
*   [Central do eSocial](https://ajuda.sankhya.com.br/hc/pt-br/articles/7064222145175)
    

[\[voltar ao topo\]](#top)