# Cadastro de Aviso Prévio

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/38693057310487-Cadastro-de-Aviso-Pr%C3%A9vio](https://ajuda.sankhya.com.br/hc/pt-br/articles/38693057310487-Cadastro-de-Aviso-Pr%C3%A9vio)

---

# Cadastro de Aviso Prévio

**Módulo:** Pessoal+  
**Caminho de Acesso:** Pessoal+ > Cadastros  
**ID da Tela:** br.com.sankhya.rh.AvisoPrevio

---

## **Sumário**

[Descrição e Usabilidade](#h_01KJG66HGT5NAW80CN7RKADNQE)

1.  [Descrição da Funcionalidade](#h_01KJG66HGVKY866XFFPVDNWD1H)
2.  [Pré-requisitos](#h_01KJG66HH5496R8Z1E6YDZT7YA)
3.  [Jornada de Uso](#h_01KJG66HH956CMN4KM2GYGHFRZ)
    
    [3.1 Pesquisar registros existentes](#h_01KJG66HH9SJR7FJ1APBX6MTTP)  
    [3.2 Cadastrar Aviso Prévio manualmente](#h_01KJG77KFT9VZ8S7R5KJH8CBA7)  
    [3.3 Exemplos de configuração](#h_01KJGV2TRM4SBDA9SFA4XHYSQD)  
    [3.4 Cancelamento de Aviso](#h_01KJGWTAEV2NHFPAEWYBGRA3NS)  
    [3.5 Emissão do Relatório](#h_01KJG66HJNEKTEDAVTH0P324GK)
    
4.  [Ponto de Atenção](#h_01KJG66HJTE7QHZH1R8515F4R6)
5.  [Dicas de Usabilidade](#h_01KJG66HJYZTN76RDYKNXXA2S6)

[Perguntas Frequentes (FAQ)](#perguntas-frequentes-faq)

[Artigos Relacionados](#h_01KJG66HJZ3JK817BZTRJ3Z6JJ)

---

## **Descrição e Usabilidade**

### **1\. Descrição da Funcionalidade**

O **Aviso Prévio** é a comunicação formal da rescisão do contrato de trabalho por uma das partes (empresa ou colaborador), conforme prazos definidos em lei.

No sistema, o registro do aviso:

*   Pode ser feito manualmente nesta tela;
    
*   Pode ser gerado automaticamente por meio de **Requisição de Rescisão**;
    
*   É utilizado para o cálculo da **folha de rescisão**;
    
*   Permite a emissão do **relatório para assinatura do colaborador**.
    

Em casos de rescisão decorrente de **Processo Trabalhista** com Tipo de Contrato:

*   3 – Trabalhador com vínculo formalizado, com inclusão ou alteração de data de desligamento;
    
*   4 – Trabalhador com vínculo formalizado, com alteração nas datas de admissão e desligamento.
    

O aviso é gerado automaticamente.

### **2\. Pré-requisitos**

**Permissões necessárias**

*   Deve ter permissão para **consultar dados dos colaboradores****.**
*   Deve **ter acesso liberado para a tela Aviso Prévio**. Essa liberação é feita na tela **Acessos** (Configurações > Controle de Acesso), pelo administrador do sistema.

**Configurações relacionadas**

Antes de cadastrar o aviso, verifique:

*   O colaborador deve estar devidamente cadastrado;
    
*   O motivo de desligamento deve estar conforme a **Tabela 19 – Motivos de Desligamento do eSocial**;
    
*   Caso utilize **Requisição**, ela deve estar criada e aprovada.
    
*   [Cadastro de Código de Afastamento para Rescisão](https://ajuda.sankhya.com.br/hc/pt-br/articles/13729923854487) realizado.
    
*   [Cadastro do Tipo de Rescisão](https://ajuda.sankhya.com.br/hc/pt-br/articles/38710044143895) realizado.
    

### **3\. Jornada de Uso**

#### **3.1 Pesquisar registros existentes**

Na tela inicial:

1.  Clique em **Configurações de Filtros**;
    
2.  Utilize as abas:
    
    *   **Campos** → pesquisa direta na tabela TFPAVI (ex.: CODFUNC);
        
    *   **Relacionamentos** → pesquisa por dados vinculados (ex.: Nome do Funcionário).
        
        **Exemplo:** ao marcar somente a opção **Funcionário** da aba **Campos**, o filtro **irá pesquisar o colaborador somente pelo Código** (CODFUNC); se marcar a opção **Funcionário** da aba **Relacionamentos**, o filtro **irá pesquisar o colaborador pelo Nome** (NOMEFUNC).
        

![filtrosconsulta-aviso-previo.gif](https://ajuda.sankhya.com.br/hc/article_attachments/38736505134231)

#### **3.2 Cadastrar Aviso Prévio manualmente**

1.  Clique em ![Botão Novo FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/38693582003863) **Cadastrar Aviso Prévio**;
    
2.  Informe:
    
    *   **Empresa**
        
    *   **Funcionário**
        
3.  O campo **Sequência** será gerado automaticamente.
    

![aba-geral-aviso-previo.png](https://ajuda.sankhya.com.br/hc/article_attachments/38693607590167)

4.  Na aba **Geral**, preencha os campos abaixo:
    
    <table class="wysiwyg-table-resized" style="margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 21%;"> <col style="width: 48%;"> <col style="width: 31%;"></colgroup><tbody><tr><td style="background-color: #66cc66;"><strong>Campos</strong></td><td style="background-color: #66cc66;"><strong>Funcionalidade</strong></td><td style="background-color: #66cc66;"><strong>Observações</strong></td></tr><tr><td style="vertical-align: top;">Tipo Rescisão</td><td>Indica o tipo de desligamento cadastrado previamente na tela <strong>Tipo de Rescisão</strong> (Pessoal+ &gt; Cadastros) conforme a&nbsp;<a href="https://www.gov.br/esocial/pt-br/documentacao-tecnica/manuais/leiautes-esocial-v-1-1-beta/tabelas.html#19" target="_blank" rel="noopener noreferrer">Tabela 19 - Motivos de desligamento</a>&nbsp;disponibilizada na documentação técnica do eSocial.</td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Programa de Demissão Voluntária</td><td style="vertical-align: top;">Deve ser utilizada quando o desligamento do colaborador ocorrer por adesão a um <strong data-start="170" data-end="177">PDV</strong>, seja para dispensa individual ou coletiva, conforme previsto em <strong data-start="243" data-end="283">Convenção Coletiva de Trabalho (CCT)</strong> ou <strong data-start="287" data-end="324">Acordo Coletivo de Trabalho (ACT)</strong>, nos termos do art. 477-B da CLT.</td><td><p data-start="360" data-end="511">Essa opção somente ficará habilitada quando o <strong data-start="427" data-end="474">código do motivo de desligamento no eSocial</strong> for diferente dos seguintes códigos:</p><p data-start="513" data-end="591"><code data-start="513" data-end="517">10</code>, <code data-start="519" data-end="523">11</code>, <code data-start="525" data-end="529">12</code>, <code data-start="531" data-end="535">13</code>, <code data-start="537" data-end="541" data-is-only-node="">28</code>, <code data-start="543" data-end="547">29</code>, <code data-start="549" data-end="553">30</code>, <code data-start="555" data-end="559">34</code>, <code data-start="561" data-end="565">36</code>, <code data-start="567" data-end="571">37</code>, <code data-start="573" data-end="577">40</code>, <code data-start="579" data-end="583">43</code> e <code data-start="586" data-end="590">44</code>.</p></td></tr><tr><td style="vertical-align: top;">Ativar Preenchimento Manual</td><td><p data-start="1705" data-end="1888">Em empresas cuja regra de cálculo possui a opção <strong data-start="1754" data-end="1798">Permitir aviso prévio inferior a 30 dias</strong> habilitada (Regras de Cálculo &gt; Propriedades &gt; Aviso Prévio), a tela de Aviso Prévio disponibiliza a opção <strong data-start="1856" data-end="1887">Ativar Preenchimento Manual</strong>.</p><p data-start="1890" data-end="2097">Ao utilizar essa opção, pode-se informar manualmente a data de fim das atividades do colaborador, permitindo cadastrar avisos prévios trabalhados com duração inferior a 30 dias, quando necessário.</p><p data-start="2099" data-end="2110"><strong data-start="2099" data-end="2110">Exemplo</strong></p><ul data-start="2112" data-end="2201"><li data-section-id="1tl3u95" data-start="2112" data-end="2149" data-list-item-id="ed2ed147d55b16a05eb43c9ebab7904f2">Data de início do aviso: 01/08/2025</li><li data-section-id="11ceu54" data-start="2150" data-end="2201" data-list-item-id="ef5d6e455efb4e0f33cb8a6fa40594b54">Data fim das atividades informada manualmente: 15/08/2025</li></ul><p data-start="2203" data-end="2273">Nesse cenário, o aviso prévio será considerado com 15 dias de duração.</p></td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Tipo Aviso</td><td style="vertical-align: top;"><p data-start="19" data-end="85">Classifica o <strong data-start="31" data-end="48">Tipo de Aviso</strong> conforme a situação do desligamento:</p><ul data-source-line="129"><li data-source-line="129" data-list-item-id="e8fce4ded8a63a03323caa7991cc690ef"><p data-source-line="129"><strong>Trabalhado</strong>: colaborador trabalha durante o período de aviso e o período é contado normalmente.</p></li><li data-source-line="133" data-list-item-id="ed3164346e6ce77b265a6cc42293ab28b"><p data-source-line="133"><strong>Dispensado</strong>: colaborador é dispensado de trabalhar, recebe como indenização.</p></li><li data-source-line="137" data-list-item-id="e3b0620b0a63a680062bc2c553a100170"><p data-source-line="137"><strong>Indenizado</strong>: similar a dispensado, com nomenclatura específica.</p><ul data-source-line="138"><li data-source-line="139" data-list-item-id="e94c410b3b1f311ee9fc48a1af754a5b7">Valor é pago na folha como indenização.</li></ul></li></ul></td><td><ul><li data-list-item-id="e07299d841e43858ddf323950a1004d7c"><p data-start="143" data-end="269">Nos casos de <strong data-start="171" data-end="187">mútuo acordo</strong>, o tipo de aviso deve ser informado como <strong data-start="229" data-end="243">Indenizado</strong>, e não como Trabalhado.</p><p data-start="143" data-end="269">O pagamento ou desconto da diferença de dias não trabalhados será realizado automaticamente por meio dos seguintes eventos:</p><ul><li data-list-item-id="e8ec0529f1a7cf48ff6f346bdc8fc0dac"><p data-start="143" data-end="269"><strong data-start="397" data-end="411">Evento 251</strong> – pagamento pelo empregador;</p></li><li data-start="443" data-end="484" data-list-item-id="e05f1941c8e591566180c3bebb7ae2ab3"><p data-start="445" data-end="484"><strong data-start="445" data-end="459">Evento 252</strong> – desconto do empregado.</p></li></ul></li><li data-start="443" data-end="484" data-list-item-id="e45d1d279c96cfd3cea194a3b24c1d5a8"><p data-start="445" data-end="484">Ao incluir um aviso por <strong data-start="531" data-end="553">quebra de contrato</strong> com o Tipo Aviso <strong data-start="574" data-end="588">Dispensado</strong>, o sistema calculará automaticamente o desconto dos dias faltantes até o término do contrato.</p><p data-start="445" data-end="484">Esses dias descontados <strong data-start="709" data-end="751">não serão demonstrados no Aviso Prévio</strong>, pois o cálculo ocorre diretamente na rescisão.</p></li></ul></td></tr><tr><td style="vertical-align: top;">Data Notificação Aviso Prévio</td><td><div><div>Data em que o aviso prévio foi comunicado/notificado ao colaborador:</div></div><ul><li data-list-item-id="e6c268178edba6e1c16339361cdcfe23c">Para <strong data-start="248" data-end="275">Aviso Prévio Dispensado</strong> ou <strong data-start="279" data-end="293">Indenizado</strong>, deve ser a mesma <strong>data de início</strong> do aviso prévio.</li><li data-list-item-id="e30b60606f4edef75255b7e1167c5a407">Para <strong data-start="420" data-end="465">Aviso Prévio Trabalhado</strong>, deve ser um dia anterior à<strong> data de início</strong> do aviso prévio.</li></ul></td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Data Início Aviso Prévio</td><td><div><div>Data em que o período de aviso prévio começa efetivamente a ser contado:</div></div><ul data-start="2101" data-end="2231"><li data-start="2101" data-end="2172" data-list-item-id="e1b41a987b2c4540746e768408b545b16"><p data-start="2103" data-end="2172">Aviso Dispensado ou Indenizado → início na mesma data da notificação;</p></li><li data-start="2173" data-end="2231" data-list-item-id="ead3270b0023be1bbd80402d63b6fb233"><p data-start="2175" data-end="2231">Aviso Trabalhado → início no dia seguinte à notificação.</p></li></ul></td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Iniciativa do Aviso</td><td><p>Indica quem tomou a iniciativa de iniciar o processo de rescisão:</p><ul data-source-line="53"><li data-source-line="53" data-list-item-id="ebad2939c933ed1f9189aef74128c6b12"><strong>Empresa</strong>: demissão por iniciativa da empresa (com ou sem justa causa).</li><li data-source-line="54" data-list-item-id="e16cb3e91d82f638346d9badd4b013eb1"><strong>Colaborador</strong>: pedido de demissão solicitado pelo colaborador.</li></ul></td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Opção p/ Red. Jornada</td><td><p data-start="35" data-end="144">Indica a alternativa da jornada conforme a situação do aviso prévio<strong> trabalhado</strong>:</p><ul data-start="146" data-end="281"><li class="wysiwyg-list-bold" data-start="146" data-end="181" data-list-item-id="e9553cd459a5dc25c332b8e665c4e33fa"><p data-start="148" data-end="181"><strong data-start="148" data-end="179">Abater Quant. Dias de Aviso</strong></p></li><li class="wysiwyg-list-bold" data-start="182" data-end="235" data-list-item-id="eb347c88e27389cc3d9fb29037cf8fb52"><p data-start="184" data-end="235"><strong data-start="184" data-end="233">Reduz 1 dia por semana conf. Lei n.º 5.889/73</strong></p></li><li class="wysiwyg-list-bold" data-start="236" data-end="257" data-list-item-id="e77b868f73bc7717a43c8cde7fbbc6076"><p data-start="238" data-end="257"><strong data-start="238" data-end="255">Não se aplica</strong></p></li><li class="wysiwyg-list-bold" data-start="258" data-end="281" data-list-item-id="ea23a179ab9a6fed2fcd6e6b13a84960b"><p data-start="260" data-end="281"><strong data-start="260" data-end="281">Reduzir a Jornada</strong></p></li></ul></td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Dias Aviso</td><td style="vertical-align: top;"><p>Quantidade de dias que constituem o período de aviso prévio.</p><p>É preenchido automaticamente conforme a&nbsp;<strong>Data Início Aviso Prévio</strong>&nbsp;informada.</p></td><td>⚠️ Acesse o artigo&nbsp;<a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/29904519221783" target="_blank" rel="noopener noreferrer">Reflexo afastamento na contagem do Aviso Prévio</a>&nbsp;para saber se deverá ter dedução na quantidade de dias do&nbsp;Aviso Prévio&nbsp;por motivo de afastamento.</td></tr><tr><td style="vertical-align: top;">Fim das Atividades</td><td>Indica o último dia de atividades do colaborador.</td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Data Homologação</td><td>Data da homologação oficial da rescisão perante órgãos competentes.</td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Quitação Rescisão (Data Prevista)</td><td>Data prevista para quitação de todas as obrigações rescisórias.</td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Indicador de cumprimento de Aviso Prévio</td><td><p>Classifica como o aviso prévio foi cumprido ou tratado:</p><p data-source-line="216"><strong>1. Cumprimento total</strong></p><ul data-source-line="217"><li data-source-line="217" data-list-item-id="ebc407e8a0d3ed329b464e71871244c64">Aviso foi totalmente cumprido conforme previsto.</li><li data-source-line="218" data-list-item-id="e364b1ee676c0d16d1d22b3a82995cc88">Colaborador trabalhou ou foi indenizado durante todo o período.</li><li data-source-line="219" data-list-item-id="e1a544490ab524cf368273756f75c0ea6">Data Fim Atividades = Data Final Aviso Prévio.</li><li data-source-line="220" data-list-item-id="efd22b5a47aca0b638593c21787c88064">Nenhum desconto ou redução no aviso.</li></ul><p data-source-line="222"><strong>2. Cumprimento parcial em razão de novo emprego</strong></p><ul data-source-line="223"><li data-source-line="223" data-list-item-id="e090d6e3d5322e190d018f1c61c642703">Colaborador conseguiu novo emprego e saiu antes.</li><li data-source-line="224" data-list-item-id="e8e7fcaec1cc81a503a0e20ceee286c59">Aviso não foi completamente cumprido.</li><li data-source-line="225" data-list-item-id="ede98d94842ea9e59b99baff763baf758">Colaborador foi liberado para novo trabalho.</li><li data-source-line="226" data-list-item-id="e913ceef82fb85c19c766f8312dbba8cc">A empresa pode exigir compensação pelos dias não cumpridos.</li></ul><p data-source-line="228"><strong>3. Outras hipóteses de cumprimento parcial do aviso</strong></p><ul data-source-line="229"><li data-source-line="229" data-list-item-id="ef7c75c236965f014eb7f6564de26e36a"><p>Outros motivos para cumprimento parcial.</p><p>Exemplo: acordo entre partes, transferência, etc.</p></li></ul><p data-source-line="234"><strong>4. Aviso prévio indenizado ou não exigível</strong></p><ul data-source-line="235"><li data-source-line="235" data-list-item-id="ea6442c014ede5c2d978c4860987b9448">Aviso foi completamente indenizado ou dispensado.</li></ul><p data-source-line="240"><strong>5. Cumprimento parcial por iniciativa da empresa</strong></p><ul data-source-line="241"><li data-source-line="241" data-list-item-id="ed7b4f1b030f06b6ace61dde704668819">Empresa liberou colaborador antes do término e pagou os dias restantes como indenização.</li><li data-source-line="243" data-list-item-id="efce3c32cd13ed55874af63f989821ddb">Comum quando tipo = Trabalhado</li></ul></td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Dias de Aviso a serem indenizados pelo Empregador</td><td>Campo considerado apenas quando o aviso for <strong data-start="735" data-end="749">Trabalhado</strong> e a quantidade de dias de aviso for <strong data-start="786" data-end="808">superior a 30 dias</strong>. Nessa situação, o sistema ajustará automaticamente a data final conforme os dias indenizados.</td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Nº Processo Trabalhista</td><td>É preenchido automaticamente quando houver rescisão decorrente de&nbsp;<a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/11592868813719" target="_blank" rel="noopener noreferrer">Processo Trabalhista</a>.</td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Data Alteração</td><td>Indica alteração no cadastro do Aviso Prévio.</td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Observação</td><td>Informação relevante sobre o aviso.</td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;" colspan="3"><strong>Seção FGTS</strong></td></tr><tr><td style="vertical-align: top;">Saldo FGTS</td><td>Saldo do FGTS a ser utilizado ou informado no cálculo da rescisão.</td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Calcula mês Anterior</td><td><p>Opção para incluir mês anterior no cálculo do FGTS na rescisão:</p><ul data-source-line="308"><li data-source-line="309" data-list-item-id="e936aec0693396a9fa0fd57baab924929">Marcada: sistema inclui contribuições do mês anterior;</li><li data-source-line="310" data-list-item-id="ee15312f9ca40abcab37a0e41cace2bdc">Desmarcada: apenas o mês de rescisão é considerado.</li></ul></td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;" colspan="3"><strong>Seção Informações de remuneração após o desligamento</strong></td></tr><tr><td style="vertical-align: top;">Indicativo de situação de remuneração após desligamento</td><td><p>Classifica se houve remuneração após o desligamento do colaborador:</p><p data-source-line="337"><strong>Quarentena</strong></p><ul data-source-line="338"><li data-source-line="338" data-list-item-id="ece7a75f011854cccb8828a2f5b487784">Colaborador está em período de quarentena (afastamento preventivo).</li><li data-source-line="339" data-list-item-id="eecfb30241e7c0635602b45d07bd59d80">Ainda recebe remuneração durante o período.</li><li data-source-line="340" data-list-item-id="e7fdcfcfc41ec47c8d875903ba4ddbc90">Comum em casos de COVID-19 ou isolamento legal.</li></ul><p data-source-line="329"><strong>Desligamento/Término Legal com Data Anterior a Competências com Remunerações Informadas no eSocial</strong></p><ul data-source-line="330"><li data-source-line="330" data-list-item-id="ec5d261d09dfac73355075be955a22078">Colaborador foi desligado em data anterior a períodos com remuneração.</li><li data-source-line="331" data-list-item-id="ec0af33c8d5c777e22f1e9bd16eb4e3d8">Aplicável quando há pagamentos após a rescisão oficial.</li></ul></td><td>&nbsp;</td></tr><tr><td style="vertical-align: top;">Data fim remuneração</td><td>Data até a qual o colaborador ainda recebe remuneração após o desligamento.</td><td>A data precisa ser posterior à data de desligamento/término do colaborador quando o indicativo for Quarentena, e deve ser o último dia trabalhado quando o indicativo for Desligamento/Término reconhecido judicialmente, com data anterior às competências com remunerações já informadas no eSocial.</td></tr></tbody></table>
    
5.  Clique em ![botão Salvar.FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/38702055905175) **Salvar (F7)**.
    

#### **3.3 Exemplos de configuração**

<table class="wysiwyg-table-resized" style="margin-left: 0px; margin-right: auto;"><colgroup><col style="width: 49%;"> <col style="width: 51%;"></colgroup><tbody><tr><td style="vertical-align: top;"><p><strong>&nbsp;<img src="https://ajuda.sankhya.com.br/hc/article_attachments/42315314647959" alt="1 FINAL.png" width="25" height="25"> Demissão Sem Justa Causa - Aviso Prévio Trabalhado</strong></p><p><strong>Funcionário: </strong>João Silva&nbsp;<br><strong>Data Notificação Aviso Prévio</strong>: 15/02/2026<br><strong>Iniciativa do Aviso</strong>: Empresa<br><strong>Tipo Aviso</strong>: Trabalhado<br><strong>Dias Aviso</strong>: 30</p><p><strong>Data Início Aviso Prévio</strong>: 16/02/2026 (dia seguinte à notificação)<br><strong>Fim das Atividades</strong>: 17/03/2026</p><p><strong>Resultado</strong>:<br>- João trabalha de 16/02/2026 até 17/03/2026<br>- Período normal de aviso prévio trabalhado<br>- Recebe FGTS, 13º, férias + 1/3 e indenizações<br>- Rescisão processada na folha de março</p></td><td><p><strong><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42315298698903" alt="2 FINAL.png" width="25" height="25"> Aviso Prévio Trabalhado 60 dias com 10 dias Indenizados</strong></p><p><strong>Funcionário</strong>: Maria Santos&nbsp;<br><strong>Data Notificação Aviso Prévio</strong>: 10/02/2026<br><strong>Iniciativa do Aviso</strong>: Empresa<br><strong>Tipo Aviso</strong>: Trabalhado<br><strong>Dias Aviso</strong>: 60<br><strong>Dias de Aviso a serem indenizados pelo Empregador</strong>: 10<br><strong>Data Início Aviso Prévio</strong>: 11/02/2026 (dia seguinte)<br><strong>Data Final Aviso</strong> (conforme dias): 12/04/2026 (11/02 + 60)<br><strong>Fim das Atividades</strong>: 02/04/2026 (11/02 + 50 dias trabalhados)<br><strong>Indicador de cumprimento de Aviso Prévio</strong>: Cumprimento Parcial por Iniciativa da Empresa<br><strong>Data Homologação</strong>: 05/04/2026<br><strong>Data Quitação Prevista</strong>: 02/05/2026 (até 30 dias após fim)</p><p>Campos FGTS e Remuneração:<br><strong>Saldo FGTS</strong>: R$ 5.000,00 (preenchido na folha rescisão)<br><strong>Calcula Mês Anterior</strong>: SIM (incluir fevereiro)<br><strong>Indicativo Remuneração</strong>: Desligamento/Término Legal<br><strong>Data Fim Remuneração</strong>: 02/04/2026 (mesma data fim atividades)</p><p><strong>Resultado</strong>:<br>- Maria trabalha de 11/02/2026 até 02/04/2026 (50 dias)<br>- 10 dias finais são indenizados pela empresa<br>- Rescisão calcula benefícios até 02/04/2026<br>- FGTS inclui contribuições de fevereiro e março<br>- Sem remuneração após 02/04/2026<br>- Recebe FGTS, 13º, férias + 1/3<br>- Empresa economiza 10 dias de trabalho<br>- Rescisão processada na folha de abril</p></td></tr><tr><td style="vertical-align: top;"><p><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42315314648983" alt="3 FINAL.png" width="25" height="25"> <strong>Pedido de Demissão &nbsp;- Aviso Prévio Dispensado</strong></p><p><strong>Funcionário</strong>: Carlos Silva&nbsp;<br><strong>Data Notificação Aviso Prévio</strong>: 15/02/2026<br><strong>Iniciativa do Aviso</strong>: Colaborador<br><strong>Tipo Aviso</strong>: Dispensado<br><strong>Dias Aviso</strong>: 30</p><p><strong>Data Início Aviso Prévio</strong>: 15/02/2026 (mesma data)<br><strong>Fim das Atividades</strong>: 16/03/2026<br><strong>Dias de Aviso a serem indenizados pelo Empregador</strong>: NÃO APLICÁVEL<br><strong>Indicador de cumprimento de Aviso Prévio</strong>: Aviso Prévio Indenizado ou Não Exigível<br><strong>Data Homologação</strong>: 17/03/2026<br><strong>Data Quitação Prevista</strong>: 16/04/2026</p><p><strong>Resultado</strong>:<br>- Carlos é dispensado imediatamente (não trabalha)<br>- Valor do aviso prévio é pago como indenização<br>- Recebe FGTS, 13º, férias + 1/3<br>- Rescisão é imediata<br>- Pagamento pode ser feito até 16/04/2026</p></td><td><p><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42315298705047" alt="4 FINAL.png" width="25" height="25">&nbsp;<strong> Demissão por Justa Causa - Aviso Prévio Indenizado</strong></p><p><strong>Funcionário</strong>: Pedro Costa&nbsp;<br><strong>Data Notificação Aviso Prévio</strong>: 05/02/2026<br><strong>Iniciativa do Aviso</strong>: Empresa<br><strong>Tipo Aviso</strong>: Indenizado<br><strong>Dias Aviso</strong>: 30</p><p><strong>Data Início Aviso Prévio</strong>: 05/02/2026 (mesma data)<br><strong>Fim das Atividades</strong>: 06/03/2026<br><strong>Dias de Aviso a serem indenizados pelo Empregador</strong>: NÃO APLICÁVEL<br><strong>Indicador de cumprimento de Aviso Prévio</strong>: Aviso Prévio Indenizado ou Não Exigível<br><strong>Data Homologação</strong>: 07/03/2026<br><strong>Data Quitação Prevista</strong>: 06/04/2026</p><p>Campos FGTS e Remuneração:<br><strong>Saldo FGTS</strong>: R$ 0,00 (sem direito - justa causa)<br><strong>Calcula Mês Anterior</strong>: NÃO APLICÁVEL<br><strong>Indicativo Remuneração</strong>: Desligamento/Término Legal<br><strong>Data Fim Remuneração</strong>: 06/03/2026 (mesma data fim atividades)</p><p><strong>Resultado</strong>:<br>- Pedro é afastado imediatamente (justa causa)<br>- Valor do aviso prévio é indenizado<br>- Sem direito a FGTS (demissão por justa causa)<br>- Sem direito a 13º (demissão por justa causa)<br>- Férias normais (sem acréscimo de 1/3)<br>- Rescisão por justa causa</p></td></tr><tr><td><p><strong><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42315298706327" alt="5 FINAL.png" width="25" height="25"> Aviso Prévio Trabalhado com Cumprimento Parcial (Novo Emprego)</strong></p><p><strong>Funcionário</strong>: Ana Silva&nbsp;<br><strong>Data Notificação Aviso Prévio</strong>: 20/02/2026<br><strong>Iniciativa do Aviso</strong>: Empresa<br><strong>Tipo Aviso</strong>: Trabalhado<br><strong>Dias Aviso</strong>: 30</p><p><strong>Data Início Aviso Prévio</strong>: 21/02/2026 (dia seguinte)<br><strong>Fim das Atividades</strong>: 22/03/2026 (teórica)<br><strong>Data Fim das Atividades</strong>: 01/03/2026 (colaborador saiu mais cedo)<br><strong>Dias de Aviso a serem indenizados pelo Empregador</strong>: 0 (não aplicável neste caso)<br><strong>Indicador de cumprimento de Aviso Prévio</strong>: Cumprimento Parcial em Razão de Novo Emprego<br><strong>Data Homologação</strong>: 02/03/2026<br><strong>Data Quitação Prevista</strong>: 01/04/2026</p><p>Campos FGTS e Remuneração:<br><strong>Saldo FGTS</strong>: R$ 4.500,00<br><strong>Calcula Mês Anterior</strong>: NÃO (apenas fevereiro)<br><strong>Indicativo Remuneração</strong>: Desligamento/Término Legal<br><strong>Data Fim Remuneração</strong>: 01/03/2026 (mesma data fim atividades)</p><p><strong>Resultado</strong>:<br>- Ana encontrou novo emprego e saiu em 01/03/2026<br>- Aviso não foi completamente cumprido (21 dias faltantes)<br>- Empresa pode cobrar compensação pelos dias não cumpridos<br>- Rescisão calcula benefícios até 01/03/2026<br>- FGTS inclui apenas fevereiro (conforme checkbox)<br>- Sem remuneração após 01/03/2026</p></td><td><p>&nbsp;<img src="https://ajuda.sankhya.com.br/hc/article_attachments/42315314650007" alt="6 FINAL.png" width="25" height="25"> <strong>Aviso Prévio com Quarentena (Remuneração Após Desligamento)</strong></p><p><strong>Funcionário</strong>: Bruno Costa&nbsp;<br><strong>Data Notificação Aviso Prévio</strong>: 15/02/2026<br><strong>Iniciativa do Aviso</strong>: Empresa<br><strong>Tipo Aviso</strong>: Trabalhado<br><strong>Dias Aviso</strong>: 30</p><p><strong>Data Início Aviso Prévio</strong>: 16/02/2026 (dia seguinte)<br><strong>Fim das Atividades</strong>: 17/03/2026<br><strong>Dias de Aviso a serem indenizados pelo Empregador</strong>: 0<br><strong>Indicador de cumprimento de Aviso Prévio</strong>: Cumprimento Total<br><strong>Data Homologação</strong>: 18/03/2026<br><strong>Data Quitação Prevista</strong>: 17/04/2026</p><p>Campos FGTS e Remuneração:<br><strong>Saldo FGTS</strong>: R$ 6.000,00<br><strong>Calcula Mês Anterior</strong>: SIM<br><strong>Indicativo Remuneração</strong>: Quarentena (CRÍTICO)<br><strong>Data Fim Remuneração</strong>: 03/04/2026 (POSTERIOR ao desligamento)</p><p><strong>Resultado</strong>:<br>- Bruno trabalha normalmente até 17/03/2026<br>- Entra em quarentena a partir de 18/03/2026<br>- Continua recebendo até 03/04/2026 (período de quarentena)<br>- Data Fim Remuneração &gt; Data Fim Atividades (03/04 &gt; 17/03)<br>- Rescisão processa benefícios até 17/03<br>- Quarentena é remunerada até 03/04<br>- FGTS inclui contribuições de fevereiro<br>- Importante para a conformidade do eSocial.<br>&nbsp;</p></td></tr></tbody></table>

#### **3.4 Cancelamento de Aviso**

Utilize esta seção quando o aviso prévio precisar ser **revogado antes do término**.

Para registrar o cancelamento e permitir a inclusão de um novo aviso para o mesmo colaborador:

1.  Informe:
    
    *   **Data** do cancelamento;
        
    *   **Motivo** (Outros, Determinação Judicial, Reconsideração Art. 489 CLT, Cumprimento de norma legal).
        

Após confirmar o cancelamento, o sistema permitirá o cadastro de um **novo aviso prévio** para o colaborador.

#### **3.5 Emissão do Relatório**

Após salvar o **Aviso Prévio**, é necessário configurar os parâmetros na tela **Preferências** (Configurações > Avançado) para que o relatório seja emitido com o motivo correto de rescisão.

Configure os seguintes parâmetros:

⚠️Os códigos informados nesses parâmetros devem corresponder a relatórios previamente cadastrados na tela **Relatórios Formatados**.

*   **Aviso Dispensado Quebra Contrato Func. – FPRELTAVIPREQFD**
    
    Informe o código do relatório de **quebra de contrato dispensado**, para que o aviso prévio seja baixado com o motivo correto da rescisão.
    
*   **Aviso Indenizado Quebra Contrato Func. – FPRELTAVIPREQFI**
    
    Informe o código do relatório referente à **quebra de contrato com aviso indenizado pelo funcionário**, garantindo que o motivo da rescisão seja exibido corretamente no documento.
    
*   **Term. do Cont. de Trab. Emp. Exp. – FPRELTAVIPREVEE**
    
    Informe o código do relatório por **término de contrato determinado**, garantindo que o motivo da rescisão seja considerado corretamente.
    
*   **Term. do Cont. de Trab. Emp. Exp. – FPRELTAVIPREVFE**
    
    Informe o código do relatório de **fim de contrato de experiência**, assegurando a baixa correta do aviso.
    
*   **Aviso Prévio Indenizado Iniciativa da Empresa - FPRELTAVIPREVEI**
    
    Configure o código do relatório utilizado quando o aviso for **indenizado por iniciativa da empresa**.
    
*   **Aviso Prévio indenizado funcionário - FPRELTAVIPREVFI**
    
    Defina o código do relatório para emissão do aviso prévio **indenizado por iniciativa do funcionário**.
    
*   **Aviso Prévio Dispensado Empresa - FPRELTAVIPREVED**
    
    Informe o código do relatório para emissão do aviso prévio **dispensado por iniciativa da empresa**.
    
*   **Aviso Prévio Dispensado Iniciativa do Empregado – FPRELTAVIPREVFD**
    
    Defina o código do relatório utilizado quando o aviso prévio for **dispensado por iniciativa do colaborador**.
    
*   **Aviso Prévio Trabalhado Iniciativa da Empresa – FPRELATAVIPREVE**
    
    Informe o código do relatório para emissão do aviso **trabalhado por iniciativa da empresa**, assegurando que o layout e o motivo do desligamento sejam apresentados corretamente.
    
*   **Aviso Prévio Trabalhado Iniciativa Funcionário - FPRELTAVIPREVFT**
    
    Informe o código do relatório para emissão do aviso **trabalhado por iniciativa do funcionário**.
    
*   Retorne à tela **Aviso Prévio** e clique no botão **Outras Opções**...;
    
*   Selecione uma das opções:
    
    *   **Baixar em PDF**
        
    *   **Mostrar em nova aba**
        
*   O sistema emitirá o relatório conforme o tipo de aviso e o motivo de rescisão configurados.
    

![relatorio-aviso-previo.gif](https://ajuda.sankhya.com.br/hc/article_attachments/38735528893975)

Para emissão em lote:

*   Selecione vários colaboradores (Ctrl);
    
*   Clique em **Outras Opções > Baixar Aviso Prévio em PDF**.
    

### **4\. Pontos de Atenção**

*   A disponibilidade da opção **Ativar Preenchimento Manual** depende da configuração da empresa na regra de cálculo para o aviso prévio.
    
*   O campo **Dias de Aviso a serem indenizados pelo Empregador** só é utilizado quando o aviso for **Trabalhado e superior a 30 dias.**
    
*   Em caso de **quebra de contrato**, o sistema calcula automaticamente o desconto dos dias faltantes.
    
*   Verifique as configurações realizadas na tela **Regras de Cálculo > Aba Propriedades > Sub-aba Aviso Prévio**
    
    *   Nessa sub-aba estão disponíveis os campos relacionados à aplicação da **Lei 12.506/2011**, que instituiu o **aviso prévio proporcional ao tempo de serviço** do empregado.
        
        É nessa configuração que o sistema define:
        
        *   a forma de contagem do tempo de serviço;
            
        *   a aplicação dos dias adicionais (3 dias por ano completo em caso de rescisão por iniciativa da empresa);
            
        *   o limite máximo de dias de aviso prévio.
            
        
        ⚠️ Configurações incorretas nessa tela podem impactar diretamente o cálculo do aviso proporcional na rescisão.
        
*   Descumprimento do aviso deve ser informado na tela de **Cálculos**, seção **Descumprimento de Aviso Prévio**.
    
*   Não é permitido criar aviso prévio para colaborador em:
    *   férias;
    *   licença prolongada;
    *   com contrato suspenso.
*   **Data de Homologação** só é válida se a rescisão foi processada.

### **5\. Dicas de Usabilidade**

*   Utilize Requisição sempre que o processo interno exigir fluxo de aprovação.
    
*   Revise as datas antes de salvar, pois impactam diretamente o cálculo da rescisão.
    
*   Verifique se não existem eventos posteriores enviados ao eSocial antes de finalizar o desligamento.
    

## **Perguntas Frequentes (FAQ)**

1.  **Qual é o mínimo de dias para aviso prévio?**
    
    Conforme a legislação brasileira, o mínimo é 30 dias. Podem ser maiores conforme categoria ou acordo coletivo.
    
2.  **Como funciona o cálculo da data de início do aviso?**
    
    A regra depende do tipo:
    
    *   Aviso Dispensado/Indenizado: Data Início = Data de Notificação (mesma data)
        
    *   Aviso Trabalhado: Data Início = Dia seguinte à Data de Notificação
        
3.  **Qual é a diferença entre Aviso Dispensado e Aviso Indenizado?**
    
    Ambos representam que o colaborador não trabalha durante o período, mas o termo "Indenizado" é mais específico para casos de rescisão. Na prática, funcionam de forma similar - a data de início é a data da notificação.
    
4.  **O que é "Iniciativa do Aviso"?**
    
    Define quem solicitou a rescisão:
    
    *   Empresa: demissão por iniciativa da empresa;
        
    *   Colaborador: pedido de demissão pelo colaborador.
        
5.  **O que acontece se o aviso for cancelado?**
    
    O colaborador é reintegrado, nenhuma rescisão é processada e o aviso fica marcado como cancelado. Volta a trabalhar normalmente.
    
6.  **Como funciona o aviso prévio trabalhado?**
    
    O colaborador continua trabalhando durante todo o período de aviso. A data de início é o dia seguinte à notificação e trabalha até a data final do aviso.
    
7.  **Pode haver dois avisos prévios simultaneamente?**
    
    Não, o sistema valida para evitar duplicatas. Um colaborador só pode ter um aviso vigente por vez.
    
8.  **Como é calculada a data final?**
    
    Data Final = Data Início + Número de Dias (ambos incluídos no cálculo).
    
9.  **Se notificar na sexta-feira, qual será a data de início para um aviso trabalhado?**
    
    Se notificado na sexta-feira (por exemplo, 15/02/2026), a data de início será segunda-feira (16/02/2026 - próximo dia útil considerado, conforme as regras de sua empresa).
    
10.  **Qual é o impacto de um aviso prévio na folha de pagamento?**
     
     O aviso prévio impacta:
     
     *   Cálculo de 13º salário proporcional
         
     *   Cálculo de férias proporcionais
         
     *   FGTS e multa de FGTS (conforme iniciativa)
         
     *   Demais indenizações trabalhistas conforme legislação
         

### **Artigos Relacionados**

*   [Cadastro de Eventos](https://ajuda.sankhya.com.br/hc/pt-br/articles/33041194565911)
    
*   [Regras de Cálculo](https://ajuda.sankhya.com.br/hc/pt-br/articles/4405310442007)
    
*   [Cálculo de Rescisão](https://ajuda.sankhya.com.br/hc/pt-br/articles/5764158461847)
    
*   [Central do eSocial](https://ajuda.sankhya.com.br/hc/pt-br/articles/7064222145175)
    
*   [Requisição de Rescisão](https://ajuda.sankhya.com.br/hc/pt-br/articles/360059085273-Requisi%C3%A7%C3%B5es#Rescis%C3%A3o)