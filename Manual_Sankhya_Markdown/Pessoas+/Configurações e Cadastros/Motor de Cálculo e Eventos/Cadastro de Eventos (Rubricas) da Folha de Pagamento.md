# Cadastro de Eventos (Rubricas) da Folha de Pagamento

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/33041194565911-Cadastro-de-Eventos-Rubricas-da-Folha-de-Pagamento](https://ajuda.sankhya.com.br/hc/pt-br/articles/33041194565911-Cadastro-de-Eventos-Rubricas-da-Folha-de-Pagamento)

---

# Cadastro de Eventos (Rubricas) da Folha de Pagamento

**Módulo:** Pessoal+  
**Caminho de acesso:** Pessoal+ > Cadastros  
**ID da Tela:** br.com.sankhya.rh.CadastroEventos

---

## **Sumário**

[Descrição e Usabilidade](#h_01JYRSHEA47DN2ARPJMPBAAK5J)

[1\. Descrição da Funcionalidade](#h_01HA7B8E3FQG6AQ73CZ3Z4J3C5)  
[2\. Pré-requisitos](#h_01JZ0FRRR0NJXMADWG0S08FCA0)  
[3\. Jornada de Uso](#h_01JXZD26W5467K5JX25EQ46AT1)

*   [Como pesquisar por um Evento](#h_01K3V6Z9BHNJ9P602J9BXJTM21)
*   [Como funciona o filtro da tela](#h_01JYKM6N55WR86HHBJKQQXDMPB)
*   [Como cadastrar um novo evento](#h_01JYKM9JC5ETB2SW3YE3JFTQHX)
*   [Como editar, duplicar ou excluir um evento](#h_01JZ0GSF6D7S12FMFSQ8M6VCS1)
*   [Relatório de Conferência de Rubricas para eSocial (S-1010)](#h_01KV8E1MA0ND5QRCVX8YTDYG3Z)

[4\. Pontos de Atenção](#h_01JY6G3YYX358XHFEX7M9RDGT0)  
[5\. Dicas de Usabilidade](#h_01JXZD26WHDATS0Q60K45PGVJJ)

[Perguntas frequentes (FAQ)](#h_01JZTGDM4BPFYCDKTCMF2KXQMZ)

[Artigos Relacionados](#h_01JY6MFXR43YR051W1QRBKC7VM)

---

## **Descrição e Usabilidade**

### **1\. Descrição da Funcionalidade**

A tela de **Eventos** (rubricas) permite cadastrar, consultar e manter as verbas utilizadas nos cálculos da folha de pagamento.  Os eventos detalham os valores pagos, descontos e informações legais exigidas, sendo essenciais para o processamento salarial, atendimento à legislação e integração com o eSocial. 

O sistema oferece eventos padrão, conforme legislação, e permite a criação de eventos personalizados para atender necessidades específicas da empresa, integrando-os às fórmulas de cálculo e bases legais. 

Os **Eventos** (ou rubricas) incluem:

*   **proventos**: valores a serem pagos (salário, hora extra, comissão);
*   **descontos**: o que será descontado (faltas, INSS, IRRF);
*   **demonstrativos**: informações obrigatórias por lei que não afetam o valor final da folha (ex: eventos informativos para o FGTS ou eSocial).

Os eventos padrão são atualizados automaticamente pelo sistema após a atualização do módulo Pessoal+.

Para verificar as alterações realizadas em cada versão, clique no botão **Download de Planilha de Alterações**. Será gerado um arquivo com o detalhamento das modificações, onde os campos alterados são destacados na cor **amarela**.

![plan-alteracoeseventos-pessoas+.gif](https://ajuda.sankhya.com.br/hc/article_attachments/41262803988247)

####  ![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42315104331799) **Como os eventos são organizados**

![eventospadpers-pessoas+.gif](https://ajuda.sankhya.com.br/hc/article_attachments/41262996676375)

Na tela **Eventos**, os dados estão divididos em duas abas:

*   **Eventos padrão**: já vêm prontos no sistema e seguem a legislação.
    
    É necessário manter os eventos **protegidos** para garantir que as atualizações de versão, ajustes e/ou melhorias sejam aplicados automaticamente, mantendo a base padronizada e atualizada.
    
*   **Eventos personalizados**: eventos criados pela sua empresa para necessidades específicas, como regras sindicais, benefícios, proventos ou descontos diferenciados, integrações com o financeiro ou casos em que a empresa adota entendimento diferente sobre um evento padrão do sistema.

Esses eventos são apresentados em **cartões (cards)**, com ícones coloridos que ajudam a identificá-los:

<table class="wysiwyg-table-resized" style="margin-left: 0px; margin-right: auto;"><colgroup><col style="width: NaN%;"> <col style="width: NaN%;"> <col style="width: NaN%;"></colgroup><tbody><tr><td style="background-color: #90ee90; text-align: center;"><strong>Tipo de evento</strong></td><td style="background-color: #90ee90; text-align: center;"><strong>Cor do ícone no card</strong></td><td style="background-color: #90ee90; text-align: center;"><strong>Significado</strong></td></tr><tr><td><span style="color: #2F3941;">Provento</span></td><td><span style="color: #2F3941;">verde</span></td><td><span style="color: #2F3941;">valor a receber (salário, comissões, entre outros)</span></td></tr><tr><td><span style="color: #2F3941;">Desconto</span></td><td><span style="color: #2F3941;">vermelho</span></td><td><span style="color: #2F3941;">valor a descontar (faltas, INSS, entre outros)</span></td></tr><tr><td><span style="color: #2F3941;">Neutro</span></td><td><span style="color: #2F3941;">azul</span></td><td><span style="color: #2F3941;">informação sem impacto no valor final da folha</span></td></tr></tbody></table>

####  ![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42315104331799) **Diferença entre eventos ativos e inativos**

*   **Eventos ativos**: estão sendo usados no cálculo da folha, aparecem com ícones coloridos.
*   **Eventos inativos**: desativados. Aparecem em **cinza**, sem ícone.

Os eventos são listados em ordem crescente de **código**, sempre mostrando **primeiro os ativos**, depois os inativos.

### **2\. Pré-requisitos**

#### **Permissões necessárias**

1.  Libere à tela por meio da rotina de **Acessos** (Configurações > Controle de Acessos).
2.  Acesse o **Painel de Configurações** (Pessoal+ > Configurações > Painel de Configurações).
    1.  Clique no card **Configuração de permissões**.
    2.  Selecione a tela **Eventos**, em seguida, o grupo de usuários desejado e certifique-se de que a permissão **Controle geral** esteja habilitada para permitir o cadastro e a edição de eventos.

#### **Configurações relacionadas**

*   Cadastro de fórmulas, bases de cálculo, integrações com eSocial e parametrização de características e grupos financeiros.

### **3\. Jornada de Uso**

#### **Como pesquisar por um Evento**

1.  Utilize o botão **Pesquisar** na parte superior da tela. 
2.  Digite uma palavra-chave ou o código do evento para encontrá-lo de forma rápida e prática.

![pesqeventos-pessoas+.gif](https://ajuda.sankhya.com.br/hc/article_attachments/41263189658775)

💡Ao lado do botão de pesquisa, pode-se definir a quantidade de cards exibidos por página na grade e também, ordenar os eventos por código ou descrição, tanto em ordem crescente quanto decrescente.

#### **Como funciona o filtro da tela**

1.  Clique no botão **Filtrar** para buscar eventos por tipo (ativos, inativos, proventos, neutros, descontos, compõe eSocial ou não compõe eSocial).
    
    ![filtros-eventos.png](https://ajuda.sankhya.com.br/hc/article_attachments/41263362816791)
    
    O mesmo filtro funciona nas duas abas (Eventos padrão e Eventos personalizados).
    

#### **Como cadastrar um novo evento**

Para criar um evento novo (personalizado):

**1.** Clique no botão ![botão Novo P+.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/33144872658583) **+** **Adicionar Evento;**

**2.** Preencha as informações nas abas que o sistema mostrar:

![novo-evento.png](https://ajuda.sankhya.com.br/hc/article_attachments/37088059083671)

🔹**Básico**

*   Dê um **nome e característica** ao evento;
    
    <table style="margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #FAEEDA; border-color: #854F0B;"><p><strong style="color: #633806;">⚠️ </strong><span style="color: hsl(32,89%,21%);"><strong style="color: #633806;">Atenção</strong></span></p><p><span style="color: #2F3941;">A característica deve ser escrita em letras maiúsculas, sem caracteres especiais e com o máximo de 25 caracteres.</span></p></td></tr></tbody></table>
    
*   Escolha se é **Provento, Desconto** ou **Neutro;**
*   Indique se **entra no líquido da folha**;
*   Marque se **deve aparecer no holerite**;
*   Escolha uma **fórmula de cálculo**;
*   Informe se ele **deve ser enviado ao eSocial**;
*   Defina se ele **integra contabilidade, provisões ou médias**;
*   Indique a **Sequência** para o cálculo.
    
    **Exemplo:** observe a importância da Sequência, com o exemplo do evento de Imposto de Renda. 
    
    Para obter o valor da sua base, todos os proventos incidentes nesse imposto devem ser somados e o valor do INSS deve ser abatido, sendo assim, o Imposto de Renda deve ter uma Sequência maior do que a do INSS e dos eventos de proventos com incidência. O sistema possui duas regras para definição da ordem de cálculo: através do código do evento, onde os de menor código são calculados primeiro, ou através da Sequência.
    
    <table style="background-color: #f4fdff; border-style: none; margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #f4fdff; border-color: #185FA5;"><p><span data-markdown-start-index="1971">ℹ️</span><span data-markdown-start-index="1971">&nbsp;</span><span style="color: #640A8E;"><span data-markdown-start-index="1971"><strong>Dependência entre os campos Base Líquida e Compõe eSocial</strong></span></span></p><p data-start="384" data-end="541">Os campos <strong data-start="394" data-end="410">Base Líquida</strong> e <strong data-start="413" data-end="431">Compõe eSocial</strong> possuem uma regra de dependência para evitar configurações incompatíveis com o envio das rubricas ao eSocial.<span aria-hidden="true"></span></p><p data-start="543" data-end="588">O comportamento é definido da seguinte forma:</p><ul><li data-list-item-id="e9166eb705d3a8a035c84a1abc8bb2bff"><p>Quando <strong>Base Líquida</strong> = <strong>Sim</strong><span aria-hidden="true"></span></p><p>O sistema:</p><ul><li data-list-item-id="e8eb6621531d1c78456595022e66ced03">define automaticamente <strong data-start="1056" data-end="1080">Compõe eSocial = Sim</strong>;</li><li data-list-item-id="eb3f73ba02642b1bef3568dfe698b7871">bloqueia o campo <strong data-start="1101" data-end="1119">Compõe eSocial</strong> para alteração.</li></ul><p>Nesse cenário, o evento deve obrigatoriamente compor o eSocial.</p></li><li data-list-item-id="e74435d6b19b94f3b1d69823084ca9243"><p>Quando <strong>Base Líquida</strong> = <strong>Não</strong></p><p>O sistema <strong data-start="1393" data-end="1455">não altera automaticamente o valor atual de Compõe eSocial </strong>e ele fica disponível para edição.</p></li></ul><p>A combinação <strong data-start="1807" data-end="1829">Base Líquida = Não</strong> e <strong data-start="1832" data-end="1856">Compõe eSocial = Sim</strong> é válida. Existem eventos que não são utilizados como base líquida, mas precisam compor o eSocial.</p><p data-start="1983" data-end="2046">Ao salvar o evento, o sistema verifica a combinação dos campos.</p><p data-start="2048" data-end="2111">Para <strong data-start="2053" data-end="2071">eventos ativos</strong>, não é permitido salvar a configuração:</p><ul data-start="2113" data-end="2166"><li data-section-id="dmbgh1" data-start="2113" data-end="2138" data-list-item-id="ed7e725ad7bcee00dad864a6201165434"><strong data-start="2115" data-end="2137">Base Líquida = Sim</strong>;</li><li data-section-id="1u4gyrq" data-start="2139" data-end="2166" data-list-item-id="e07f917e55f4bf648bac5b339e9f4a912"><strong data-start="2141" data-end="2165">Compõe eSocial = Não</strong>.</li></ul><p data-start="2168" data-end="2263">Caso essa combinação seja identificada, o sistema bloqueia o salvamento e apresenta a mensagem:</p><p data-start="2168" data-end="2263"><em><strong data-start="2267" data-end="2367">"Não foi possível salvar. Eventos com Base Líquida ativa devem obrigatoriamente compor o eSocial."</strong></em></p></td></tr></tbody></table>
    

🔹**Avançado**

*   Marque os impostos que **o evento deve calcular (INSS, FGTS, IRRF)**;
*   Escolha se ele entra na **DIRF** ou **SEFIP**;
*   Informe se será usado para calcular **diferença de dissídio, férias, faltas** ou **API**.

🔹**eSocial**

*   Preencha a **Natureza da Rubrica** (conforme tabela do eSocial);
*   Defina se **há incidência de PIS**;
*   Marque corretamente os impostos para que o eSocial aceite os dados.
    
    <table style="margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #FAEEDA; border-color: #854F0B;"><p><strong style="color: #633806;">⚠️ </strong><span style="color: hsl(32,89%,21%);"><strong style="color: #633806;">Atenção</strong></span></p><p><span style="color: #2F3941;">Eventos ativos e integrados ao eSocial devem ter a marcação <strong>Compõe eSocial</strong> habilitada.</span></p></td></tr></tbody></table>
    

🔹**Bases de Cálculo**

*   O sistema preenche automaticamente com base nas regras de cálculo;
*   Também é possível adicionar ou excluir bases manualmente.
    
    <table style="margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #FAEEDA; border-color: #854F0B;"><p><strong style="color: #633806;">⚠️ </strong><span style="color: hsl(32,89%,21%);"><strong style="color: #633806;">Atenção</strong></span></p><p><strong>Eventos personalizados não são inseridos automaticamente nas bases de cálculo padrão</strong> durante a atualização dos pacotes de eventos e fórmulas. Essa configuração deve ser realizada manualmente, conforme as necessidades da empresa, para garantir que os eventos personalizados sejam considerados corretamente nas bases desejadas (por exemplo, margem consignável, INSS, FGTS, entre outras).</p></td></tr></tbody></table>
    
*   Após criar ou alterar um evento personalizado, revise suas bases de cálculo e incidências para evitar divergências no processamento da folha.

🔹**Documentação**

*   Descreva para que serve o evento, como ele deve ser usado, e se há lei relacionada.

🔹 [**Rubricas no eSocial**](https://ajuda.sankhya.com.br/hc/pt-br/articles/37087067045911)

*   Essa aba apresenta o **histórico de envios bem-sucedidos da rubrica para o eSocial (Evento S-1010)**.

**3.** Após preencher tudo, clique em **Confirmar alterações.**

<table style="margin-left: 0px; margin-right: auto;"><tbody><tr><td style="background-color: #FAEEDA; border-color: #854F0B;"><p><strong style="color: #633806;">⚠️ </strong><span style="color: hsl(32,89%,21%);"><strong style="color: #633806;">Atenção</strong></span></p><p><span style="color: #2F3941;">Se houver alguma regra incorreta (como impostos ou fórmulas incompatíveis), será exibido um aviso impedindo o salvamento.</span></p></td></tr></tbody></table>

#### **Como editar, duplicar ou excluir um evento**

*   **Editar:** abra o card do evento e ajuste as informações permitidas.
*   **Duplicar:** passe o mouse sobre o card e clique em **Duplicar** e confirme.
*   **Excluir:** passe o mouse sobre o card, clique na lixeira e confirme. **Eventos padrão Sankhya não podem ser editados ou excluídos**.

#### **Relatório de Conferência de Rubricas para eSocial (S-1010)**

O botão **Conferência de Rubricas para eSocial (S-1010)** permite consultar, em um único relatório, como as rubricas estão atualmente registradas no eSocial. 

A consulta exibe as informações do último evento S-1010 enviado com sucesso, facilitando a validação das incidências de INSS, IRRF e FGTS, a conferência da parametrização dos eventos e a identificação de possíveis inconsistências antes do fechamento da folha ou do envio das obrigações acessórias.

Para saber mais, acesse [Relatório de Conferência de Rubricas para eSocial (S-1010)](https://ajuda.sankhya.com.br/hc/pt-br/articles/41258999019159).

### **4\. Pontos de Atenção**

*   **Evento de movimento** do tipo valor deve ser configurado da seguinte forma:
    *   ative a marcação **Tem seus valores recalculados** na aba Avançado;
    *   desative as marcações **Aplicar percentual em todos os eventos da folha complementar (mensalistas)** e **Aplicar percentual em todos os eventos da folha complementar (não mensalistas)** na aba [Propriedades](https://ajuda.sankhya.com.br/hc/pt-br/articles/4405310442007-Regras-de-C%C3%A1lculos#abapropriedades) da [Regra de Cálculo](https://ajuda.sankhya.com.br/hc/pt-br/articles/4405310442007);
    *   informe o código do evento no parâmetro **FPEVECALCCOMP** para que ele seja recalculado com base no percentual do reajuste.
*   Eventos com recálculo automático, ou seja, configurados no parâmetro **FPEVERECAUTO**, **não podem** ter regras com percentual aplicado.
*   Eventos de [Movimento por Funcionários](https://ajuda.sankhya.com.br/hc/pt-br/articles/38268572935319) não podem ter o campo **Evento como regra em cálculo de** preenchido na aba **Básico**.
*   Campos como **Característica** e **Código** são únicos e não editáveis após o salvamento.
*   A marcação **Integra Contabilidade?** deve ser usada com cautela para garantir o correto envio aos módulos financeiros.
*   Para **os eventos padrões Sankhya** não é possível alterar as incidências de impostos: INSS, IRRF, FGTS, Base DIRF e Base SEFIP.
*   O campo **Incidência p/ PIS** só será exibido na aba eSocial quando houver ao menos uma empresa matriz cadastrada no sistema como contribuinte do PIS sobre a folha (marcação **Empresa contribuinte** ativada na tela **Registro Fiscal**), assim como as informações inseridas, impactando a rotina da folha e o eSocial. Empresas não contribuintes ou casos em que não há empresas contribuintes cadastradas no sistema não serão afetados pelas alterações da versão S-1.3 relacionados ao PIS PASEP e o campo não será exibido.
*   **Após o cadastro de cada evento, deverá gerar** **cada um e enviar através do evento S-1010 ao eSocial pela tela Central do eSocial.**

### **5\. Dicas de Usabilidade**

*   Use **filtros rápidos** para localizar eventos por tipo (Provento, Desconto, Neutro), ou ainda a pesquisa por código, ou descrição para localizar um evento.
*   Ao duplicar eventos, revise todos os campos antes de salvar.
*   Aproveite a integração automática com fórmulas e bases, mas sempre confira incidências e vínculos.
*   Consulte as abas eSocial e Avançado para garantir conformidade legal.
*   A aba **Documentação** é utilizada para registrar justificativas e regras específicas de eventos personalizados.

## **Perguntas frequentes (FAQ)**

**1\. O que são eventos padrão?** 

São os que já vêm no sistema Sankhya, conforme a lei.

**2\.** **O que são eventos personalizados?**

São os eventos que a empresa cria para atender situações específicas, como bônus internos ou acordos.

**3\. Posso alterar um evento padrão?** 

Não. Eles são protegidos para evitar erros.

**4\. Como sei se o evento está ativo ou inativo?**

Eventos ativos aparecem coloridos. Inativos aparecem em cinza.

**5\. Preciso cadastrar evento para hora extra ou INSS?**

Não. Já existem eventos padrão para isso.

**6\. Consigo ver todos os eventos juntos?**

Não. Eles estão divididos em duas abas: padrão e personalizados.

**7.** **Posso criar um evento com código personalizado?**

Sim, mas os códigos serão atribuídos automaticamente a partir de 10.000.

**8\. Eventos personalizados são enviados ao eSocial?**

Sim, desde que estejam com a marcação “Compõe eSocial” habilitada.

**9\. Posso excluir qualquer evento?**

Sim, exceto eventos padrão da Sankhya.

## **Artigos Relacionados**

*   [Fórmulas](https://ajuda.sankhya.com.br/hc/pt-br/articles/13061392411287)
*   [Fórmulas contábeis](https://ajuda.sankhya.com.br/hc/pt-br/articles/10086051863063)
*   [Padronização de eventos](https://ajuda.sankhya.com.br/hc/pt-br/articles/11467714112407)
*   [Lançamento de Movimento](https://ajuda.sankhya.com.br/hc/pt-br/articles/13968004985495)
*   [Configuração de férias](https://ajuda.sankhya.com.br/hc/pt-br/articles/7084333899415)
*   [Acumulados do Ano](https://ajuda.sankhya.com.br/hc/pt-br/articles/8085396691351)
*   [Eventos Pessoal não existe ou não pode ser usado aqui](https://ajuda.sankhya.com.br/hc/pt-br/articles/7918034010647)
*   [Os eventos de médias não estão sendo exibidos no campo de médias na tela de cálculo](https://ajuda.sankhya.com.br/hc/pt-br/articles/32909754314007)
*   [Relatório de Rescisão não pode ser gerado pois os eventos xx não estão configurados](https://ajuda.sankhya.com.br/hc/pt-br/articles/7758888580503)
*   [Erro na Integração Contábil – Eventos Duplicados na Configuração da Integração Contábil](https://ajuda.sankhya.com.br/hc/pt-br/articles/32853406492567)
*   [O evento 1901 - BASE INSS foi identificado como origem da divergência](https://ajuda.sankhya.com.br/hc/pt-br/articles/10621211915927)