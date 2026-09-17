# Tela EFD - Contribuições PIS/COFINS (Flex e HTML)

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/42347161661079-Tela-EFD-Contribui%C3%A7%C3%B5es-PIS-COFINS-Flex-e-HTML](https://ajuda.sankhya.com.br/hc/pt-br/articles/42347161661079-Tela-EFD-Contribui%C3%A7%C3%B5es-PIS-COFINS-Flex-e-HTML)

---

# Tela EFD - Contribuições PIS/COFINS (Flex e HTML)

**Módulo:** Livros Fiscais › Conexão

**Caminho de acesso:** Menu Principal › Livros Fiscais › Conexão › EFD - Contribuições PIS/COFINS

**Neste artigo**

*   [O que é e para que serve](#oque)
*   [Antes de começar](#antes)
*   [Diferenças entre as telas Flex](#diferencas)
*    [e HTML5](#diferencas)
*   [Como usar a tela](#como-usar)
*   [Aba Configurações](#aba-config)
*   [Demais abas da tela (Blocos](#demais-abas)
*    [0 a 9)](#demais-abas)
*   [Botões da tela](#botoes)
*   [Modalidades de Apuração](#modalidades) 
*   [das Contribuições](#modalidades)
*   [Regimes](#regimes)
*   [Geração do Bloco 0](#bloco0)
*   [Geração do Bloco C](#blococ)
*   [Geração do Bloco D](#blocod)
*   [Geração do Bloco F](#blocof)
*   [Geração do Bloco M](#blocom)
*   [Geração do Bloco P (descontinuado)](#blocop)
*   [Geração do Bloco 1](#bloco1)
*   [Processo Judicial](#processo-judicial)
*   [Configuração e Consolidação por Estabelecimentos](#consolidacao)
*   [Parâmetros que influenciam](#parametros) 
*   [a rotina](#parametros)

## O que é e para que serve

A **Tela EFD - Contribuições PIS/COFINS** gera o arquivo digital de Escrituração Fiscal Digital das Contribuições (EFD PIS/COFINS — Arquivo Digital de Escrituração da Contribuição para o PIS/PASEP e COFINS), conforme o art. 15 da Lei nº 9.779, de 19 de janeiro de 1999, para submissão ao programa validador da Receita Federal (assinatura digital, transmissão e visualização). A geração é centralizada pelo estabelecimento matriz da pessoa jurídica, e este artigo cobre as duas telas que coexistem hoje para essa geração: a tela **EFD - Contribuições** (Flex, anterior) e a tela **EFD - Contribuições PIS/COFINS** (HTML5, padrão desde a versão 4.19) — exceto onde uma tabela ou observação indicar explicitamente uma diferença de comportamento entre elas (veja [Diferenças entre as telas Flex e HTML5](#diferencas)). A tela não substitui a validação, assinatura digital e transmissão do arquivo, que continuam sendo feitas no PVA da Receita Federal, nem documenta campo a campo o leiaute oficial — para esse detalhamento, consulte o Guia Prático da EFD-Contribuições vigente, publicado pela Receita Federal.

**ℹ️ Nota**

Até a versão 4.18, era necessário habilitar o parâmetro `HABECONTLAYNOVO` (**Habilita geração novo layout EFD Contribuições?**) para acessar a tela HTML5. A partir da 4.19, ela ficou disponível sem esse parâmetro, e a tela Flex segue ativa em paralelo.

---

## Antes de começar

Antes de gerar a EFD-Contribuições pela primeira vez para uma empresa, confirme os pontos abaixo — a maior parte dos erros de geração vem de um deles não estar configurado.

*   Na aba **Regime de Apuração da Contribuição Social e de Apropriação de Crédito** ([Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa)), tenha um cadastro cobrindo o período que você vai gerar, com **Dt. Inicial** e **Dt. Final** do regime. Sem isso, o sistema recusa a geração. Essa aba afeta exclusivamente PIS/COFINS — não tem relação com ICMS/IPI, mesmo aparecendo também em telas de EFD Fiscal. Veja detalhes em [Geração do Bloco C](#blococ).
*   Em **Preferências da Empresa**, aba **EFD - Escrituração Fiscal Digital**, habilite os Blocos e Registros que devem entrar no arquivo — é esse cadastro, e não a **Aba Configurações** da tela de geração, que decide registro a registro o que efetivamente é gerado. Veja [Demais abas da tela](#demais-abas).
*   Configure a **Conta Contábil**, quando aplicável — ela alimenta o campo correspondente em vários registros (A170/C170, D100/D101/D105, F100/F500/F525, P100, 1900). Sem essa configuração, o registro continua sendo gerado normalmente; apenas esse campo específico fica sem preenchimento. Consulte o processo [Geração da Conta Contábil para EFD - Contribuições](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044599594-Gera%C3%A7%C3%A3o-da-Conta-Cont%C3%A1bil-para-EFD-Contribui%C3%A7%C3%B5es).
*   Cadastre corretamente a empresa como matriz, filial ou Sociedade em Conta de Participação (SCP), se o seu cenário envolver consolidação de estabelecimentos ou SCP — ver [Configuração e Consolidação por Estabelecimentos](#consolidacao) e a **Sub-aba Documentos para Receita de SCP** em [Aba Configurações](#aba-config).

Este artigo descreve o comportamento do sistema de forma macro. Para o significado de cada campo do leiaute oficial (posição, tamanho, obrigatoriedade), consulte o Guia Prático da EFD-Contribuições vigente, publicado pela Receita Federal, e as **Preferências da Empresa** (abas **Regime de Apuração** e **EFD - Escrituração Fiscal Digital**).

[↑ Voltar ao início](#sumario)

---

## Diferenças entre as telas Flex e HTML5

A tela HTML5 é a versão atual e ativamente desenvolvida; a tela Flex é a versão anterior, mantida em paralelo. A tabela abaixo reúne todas as diferenças de suporte confirmadas entre as duas — use-a como referência única em vez de notas espalhadas pelo restante do artigo.

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Recurso</strong></td><td style="border-color: #999; padding: 6px;"><strong>Tela EFD - Contribuições (Flex)</strong></td><td style="border-color: #999; padding: 6px;"><strong>Tela EFD - Contribuições PIS/COFINS (HTML5)</strong></td><td style="border-color: #999; padding: 6px;"><strong>Observação</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">Painel de Filtro Rápido (Empresa/Referência)</td><td style="border-color: #999; padding: 6px;">Não tem</td><td style="border-color: #999; padding: 6px;">Tem</td><td style="border-color: #999; padding: 6px;">Exclusivo da HTML5</td></tr><tr><td style="border-color: #999; padding: 6px;">Fluxo de geração</td><td style="border-color: #999; padding: 6px;">Um único botão <strong>Gerar Arquivo</strong> (processa e gera de uma vez)</td><td style="border-color: #999; padding: 6px;">Botões separados <strong>Processar</strong> e <strong>Gerar</strong></td><td style="border-color: #999; padding: 6px;">Ver <a href="#botoes">Botões da tela</a></td></tr><tr><td style="border-color: #999; padding: 6px;">Botão <strong>Consultar Nota Não Gerada</strong></td><td style="border-color: #999; padding: 6px;">Tem</td><td style="border-color: #999; padding: 6px;">Sem equivalente mapeado</td><td style="border-color: #999; padding: 6px;">—</td></tr><tr><td style="border-color: #999; padding: 6px;">Botão <strong>Reprocessar Registros Totalizadores</strong></td><td style="border-color: #999; padding: 6px;">Sem equivalente mapeado</td><td style="border-color: #999; padding: 6px;">Tem (menu <strong>Outras Opções</strong>)</td><td style="border-color: #999; padding: 6px;">—</td></tr><tr><td style="border-color: #999; padding: 6px;">Campos <strong>Período</strong> e <strong>UF</strong></td><td style="border-color: #999; padding: 6px;">Preenchidos nos campos iniciais da tela</td><td style="border-color: #999; padding: 6px;">Dentro da <strong>Aba Configurações</strong>; o preenchimento inicial pede apenas <strong>Data Referência</strong></td><td style="border-color: #999; padding: 6px;">—</td></tr><tr><td style="border-color: #999; padding: 6px;">Campo <strong>Empresa</strong> obrigatório</td><td style="border-color: #999; padding: 6px;">Não obrigatório — pode ficar em branco para selecionar várias ou todas as empresas</td><td style="border-color: #999; padding: 6px;">Obrigatório — é preciso selecionar uma empresa antes de gerar</td><td style="border-color: #999; padding: 6px;">Exigência exclusiva da HTML5</td></tr><tr><td style="border-color: #999; padding: 6px;">Abas de registro por Bloco (revisão antes da geração)</td><td style="border-color: #999; padding: 6px;">Não tem — o conteúdo é descarregado diretamente no arquivo gerado</td><td style="border-color: #999; padding: 6px;">Tem — uma aba por Bloco, para revisar os dados antes de gerar</td><td style="border-color: #999; padding: 6px;">Ver <a href="#demais-abas">Demais abas da tela</a></td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Sub-aba Documentos para Receita de SCP</strong></td><td style="border-color: #999; padding: 6px;">Não existe</td><td style="border-color: #999; padding: 6px;">Existe</td><td style="border-color: #999; padding: 6px;">Exclusiva da HTML5</td></tr><tr><td style="border-color: #999; padding: 6px;">Marcação <strong>Gerar os SAT CF-e Cancelados para o arquivo?</strong></td><td style="border-color: #999; padding: 6px;">Não existe</td><td style="border-color: #999; padding: 6px;">Existe</td><td style="border-color: #999; padding: 6px;">Exclusiva da HTML5</td></tr><tr><td style="border-color: #999; padding: 6px;">Marcação <strong>Gerar registro A010/C010/D010 para empresa sem movimento</strong></td><td style="border-color: #999; padding: 6px;">Não existe</td><td style="border-color: #999; padding: 6px;">Existe</td><td style="border-color: #999; padding: 6px;">Exclusiva da HTML5</td></tr><tr><td style="border-color: #999; padding: 6px;">Motivo do registro 0120 — opções 101/102/103 (PERSE)</td><td style="border-color: #999; padding: 6px;">Não existe</td><td style="border-color: #999; padding: 6px;">Existe</td><td style="border-color: #999; padding: 6px;">Legislação posterior à Flex</td></tr><tr><td style="border-color: #999; padding: 6px;">Configuração e Consolidação por Estabelecimentos</td><td style="border-color: #999; padding: 6px;">Não existe</td><td style="border-color: #999; padding: 6px;">Existe, a partir da versão 4.32</td><td style="border-color: #999; padding: 6px;">Único item com corte de versão confirmado</td></tr></tbody></table>

[↑ Voltar ao início](#sumario)

---

## Como usar a tela

### Painel de filtros (exclusivo da HTML5)

Use esse painel para buscar um ou mais registros específicos, preenchendo os campos **Empresa** e **Referência**. Se você clicar em **Aplicar** sem preencher esses campos, o sistema exibe o aviso _"Não foram preenchidos os campos da empresa e da referência no filtro rápido. A falta destas informações na consulta pode sobrecarregar o Sankhya Om e causar travamentos na rotina. Deseja prosseguir?"_ Respondendo **Não**, nada é carregado; respondendo **Sim**, todos os dados disponíveis são carregados, independentemente de **Empresa** e **Referência**.

### Preenchimentos iniciais

*   **Empresa** — empresa da qual serão gerados os dados. Na tela HTML5, este campo é obrigatório: é preciso selecionar uma empresa antes de processar ou gerar o arquivo.
*   **Data Referência** — recebe o primeiro dia do mês/ano do arquivo a gerar.
*   **Versão do Layout do Arquivo** — não editável; reflete a versão vigente para o período. Movimentação referente a 01/2019 em diante exige a versão **005 - Fatos geradores: Início 01/01/2019**. Confirme a versão de layout atual no Guia Prático vigente antes de tratar esta informação como definitiva, já que leiautes podem ser atualizados pela Receita Federal.
*   **Tipo escrituração** — só é preenchido depois de configurado previamente o campo **Tipo escrituração** na aba de registro 0000 (**Aba Configurações**).

Na tela **EFD - Contribuições** (Flex), o período é definido diretamente aqui por dois campos — **UF** e **Período** (Data Inicial/Final) — em vez de uma única **Data Referência**, e o campo **Empresa** pode ficar em branco para selecionar várias ou todas as empresas configuradas para EFD-Contribuições antes de gerar. Veja também o pré-requisito da aba **Regime de Apuração**: sem um cadastro de regime cobrindo o período, a geração é recusada em ambas as telas.

[↑ Voltar ao início](#sumario)

---

## Aba Configurações

Na tela **EFD - Contribuições** (Flex), esta aba se chama **Aba Parâmetros**. Nesta aba são definidas as especificidades do arquivo de escrituração; no Flex, o conteúdo que aqui está organizado na **Sub-aba Opções** aparece como uma seção dentro da própria **Aba Parâmetros**, e não como uma aba separada.

*   **Período** — abrange a geração do relatório, com base na **Data Referência** informada inicialmente.
*   **UF** — a ser considerada para geração do documento.
*   **Tipo de Escrituração** — **Original** (arquivo enviado conforme as regras/periodicidade da empresa) ou **Retificadora** (correções sobre um arquivo Original já enviado).
*   **Indicador de Situação Especial** — preenchido quando a escrituração se referir a **0-Abertura**, **1-Cisão**, **2-Fusão**, **3-Incorporação** ou **4-Encerramento** da pessoa jurídica.
*   **Nro. Único Nota** — para gerar a escrituração de apenas uma nota específica.
*   **Tributa PIS/COFINS Despesas Acessórias Separadamente no F100?** — quando marcada, habilita os campos **Cód.Sit.Tribut. PIS/COFINS**, **Alíquota de PIS** e **Alíquota de COFINS**, que passam a valer no registro F100 para essas despesas.
*   **Gerar registro F120 agrupado pela descrição do bem?** — agrupa a geração do F120 pela descrição do bem.
*   **Priorizar Número de NFS-e e não de RPS** — prioriza o número da NFS-e em vez do RPS na geração do documento.
*   **Gerar registro A010/C010/D010 para empresa sem movimento** (provavelmente exclusivo da HTML5) — gera A010, C010 e D010 mesmo sem movimentação da filial a escriturar no período.
*   **Gerar os SAT CF-e Cancelados para o arquivo?** (exclusivo da HTML5) — inclui os SAT's cancelados nos registros C010, C860 e C870.
*   **Recompor financeiro com retenções na nota de serviço (F500, F550)** — campo relacionado à consolidação de PJ no lucro presumido, com incidência de PIS/COFINS pelo regime de Caixa (F500) ou de Competência (F550). Recompõe o financeiro quando notas de serviço se enquadram nesse cenário.

### Sub-aba Opções

#### Compensar Crédito - Registro 1100/1500

**O que faz**

Habilita a compensação de créditos a partir da importação do arquivo gerado na EFD-Contribuições contendo os registros M100 calculados.

**Quando usar**

Use quando precisar compensar créditos apurados no bloco M em um ciclo de retransmissão do arquivo.

**Como funciona**

Marcado, o fluxo segue estas etapas:

1.  Gere o EFD-Contribuições sem a marcação.
2.  Importe no PVA.
3.  Gere o bloco M pelo validador do PVA.
4.  Exporte, ainda no PVA, o arquivo com o bloco M.
5.  Gere novamente o EFD-Contribuições com a marcação ativa, importando o arquivo pelo campo **Arquivo exportado pelo PVA**.
6.  Gere novamente o SPED.

**Impacto no sistema**

Se o arquivo tiver mais créditos que débitos, a tela [**Controle de Créditos PIS/COFINS**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044595794-Controle-de-Cr%C3%A9ditos-PIS-COFINS) é preenchida automaticamente; havendo mais débitos que créditos, usam-se os créditos disponíveis de meses anteriores. O Registro 1500 é gerado automaticamente, e saldos de períodos anteriores também podem ser importados para compor as tabelas dessa tela, habilitando a compensação e a geração dos valores dos registros 1100 e 1500.

#### Geração do Arquivo sem Dados a Escriturar (Registro 0120)

**O que faz**

Gera o Registro 0120 para pessoas jurídicas sem operações geradoras de receitas ou créditos, obrigatório em qualquer mês de referência mesmo sem movimento.

**Como funciona**

Selecione o motivo no campo **Motivo da Geração do Arquivo Sem Dados a Escriturar**:

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Código</strong></td><td style="border-color: #999; padding: 6px;"><strong>Motivo</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">01</td><td style="border-color: #999; padding: 6px;">Pessoa jurídica imune ou isenta do IRPJ</td></tr><tr><td style="border-color: #999; padding: 6px;">02</td><td style="border-color: #999; padding: 6px;">Órgãos públicos, autarquias e fundações públicas</td></tr><tr><td style="border-color: #999; padding: 6px;">03</td><td style="border-color: #999; padding: 6px;">Pessoa jurídica inativa</td></tr><tr><td style="border-color: #999; padding: 6px;">04</td><td style="border-color: #999; padding: 6px;">Pessoa jurídica em geral, sem operações geradoras de receitas (tributáveis ou não) ou de créditos</td></tr><tr><td style="border-color: #999; padding: 6px;">05</td><td style="border-color: #999; padding: 6px;">Sociedade em Conta de Participação (SCP), sem operações geradoras de receitas ou créditos</td></tr><tr><td style="border-color: #999; padding: 6px;">06</td><td style="border-color: #999; padding: 6px;">Sociedade Cooperativa, sem operações geradoras de receitas ou créditos</td></tr><tr><td style="border-color: #999; padding: 6px;">07</td><td style="border-color: #999; padding: 6px;">Escrituração decorrente de incorporação, fusão ou cisão, sem operações geradoras de receitas ou créditos</td></tr><tr><td style="border-color: #999; padding: 6px;">99</td><td style="border-color: #999; padding: 6px;">Demais hipóteses de dispensa de escrituração (art. 5º da IN RFB nº 1.252/2012)</td></tr><tr><td style="border-color: #999; padding: 6px;">101</td><td style="border-color: #999; padding: 6px;">PERSE — Transmissão por inconsistência cadastral na base da RFB (exclusivo HTML5)</td></tr><tr><td style="border-color: #999; padding: 6px;">102</td><td style="border-color: #999; padding: 6px;">PERSE — Transmissão por decisão judicial (exclusivo HTML5)</td></tr><tr><td style="border-color: #999; padding: 6px;">103</td><td style="border-color: #999; padding: 6px;">PERSE — Transmissão por decisão administrativa (exclusivo HTML5)</td></tr></tbody></table>

Se a **Dt. Referência** for dezembro, o campo **Meses para o registro 0120 sem dados a escriturar** libera a marcação de qualquer mês do ano; fora de dezembro, só o próprio mês de referência pode ser gerado. Empresas com filial sem movimento devem gerar o 0120 dessa filial separadamente, em dezembro, cobrindo os meses sem movimento.

**⚠️ Atenção**

Marcar um mês nesse campo com período fora de dezembro gera o erro _"Meses para o registro 0120, podem ser marcados somente quando informado o mês 12 no período (data inicial e final da geração)"_. O arquivo é gerado com sucesso quando o período está em dezembro, o motivo foi selecionado e ao menos um mês foi escolhido.

### Sub-aba Ajustes de Devoluções de Compras

Destinada à geração automática do detalhamento dos ajustes de devoluções de compras — redutores da receita na apuração via Bloco M. Registros gerados: M100, M110, M115 (PIS/PASEP) e M500, M510, M515 (COFINS). Marque **Gerar ajustes de devoluções de compras para o BLOCO M** para habilitar os demais campos e configure conforme as rotinas fiscais da empresa — recomenda-se acompanhamento de um contador. Ao clicar em **Gerar o Arquivo**, a grade é alimentada com as devoluções de compra enquadradas na rotina, gerando M100/M110/M115 e M500/M510/M515 apenas com os dados dessas devoluções; a apuração completa do Bloco M continua sendo feita pelo PVA.

### Sub-aba Documentos para Receita de SCP

Esta sub-aba não existe na tela Flex — é exclusiva da HTML5. Indica os documentos geradores de receita à SCP (Sociedade em Conta de Participação), para que sejam gerados em arquivos separados na EFD-Contribuições da Sócia Ostensiva.

Para configurar uma empresa como SCP de uma Sócia Ostensiva:

1.  Na tela [**Empresa**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607994-Empresa), selecione a empresa Ostensiva e, na aba **SCP - Sociedade em Conta de Participação**, marque **1 - Empresa participante de SCP como sócio ostensivo**. Vincule a SCP pelo botão **Cadastrar Sociedade em Conta de Participação \[F8\]**.
2.  Ainda na tela **Empresa**, selecione a empresa SCP e marque **2 - SCP** no mesmo campo.
3.  Na tela **Preferências da Empresa**, empresa Ostensiva, aba **EFD - Escrituração Fiscal Digital**, campo **Tipo de Escrituração**, selecione **EFD Contribuições**; no campo **Natureza da Pessoa Jurídica**, selecione **03 - Pessoa jurídica em geral participante de SCP como sócia ostensiva**.
4.  Na aba **Contabilidade**, campo **Tipo de Empresa**, selecione **1 - Empresa participante da SCP como sócio ostensivo** e vincule a SCP pelo botão **\[F8\]**.
5.  Repita para a empresa SCP: **05 - Sociedade em Conta de Participação - SCP** na **Natureza da Pessoa Jurídica**, e **2 - SCP** no **Tipo de Empresa** da aba **Contabilidade**.

No botão **Outras Opções...**, a opção **Seleção de documentos para Receita de SCP** abre um pop-up de mesmo nome, onde são selecionados os documentos a apresentar na sub-aba. Ao associar os documentos, as colunas **Cód. SCP** e **Nome Fantasia (SCP)** dos registros F500, F525 e F550 são preenchidas conforme o Critério de Apuração do Lucro Presumido, identificando quais receitas vão para o arquivo da Sócia Ostensiva e quais vão para o arquivo da SCP.

Ao gerar a EFD - Contribuições PIS/COFINS, o sistema cria os arquivos da Sócia Ostensiva e da SCP na mesma pasta ZIP, em arquivos separados. No arquivo da Sócia Ostensiva, o campo 13 do Registro 0000 traz a opção 03, e é exibido um registro 0035 para cada SCP vinculada. No arquivo da SCP, o registro 0000 traz os dados da Sócia Ostensiva, mas o campo 13 contém a opção **05 - Sociedade em Conta de Participação - SCP**; apenas um registro 0035 é apresentado, referente à SCP.

Com **Regime de Caixa - Escrituração consolidada (Registro F500)** definido no campo **Lucro Presumido/Critério Apuração** (aba **Regime de Apuração da Contrib. Social e Aprop. Crédito**): o arquivo da Sócia Ostensiva não considera os documentos desta sub-aba nos registros F500/F525; o arquivo da SCP usa apenas os documentos indicados aqui para compor F500/F525, um arquivo por SCP. Com **Regime de Competência - Escrituração consolidada (Registro F550)** selecionado, o mesmo padrão se aplica ao registro F550.

**ℹ️ Nota**

Se esta sub-aba não for configurada e não houver documentos de SCP vinculados, a geração da Sócia Ostensiva ainda cria — mesmo sem movimentação — o arquivo TXT da SCP, preenchendo automaticamente o Registro 0120 com o motivo _"05-Sociedade em Conta de Participação - SCP, que não realizou operações geradoras de receitas (tributáveis ou não) ou de créditos"_, independentemente do que estava selecionado antes.

[↑ Voltar ao início](#sumario)

---

## Demais abas da tela (Blocos 0 a 9)

As demais abas — exclusivas da tela HTML5 — representam os Blocos do arquivo, na estrutura do Guia Prático da EFD-Contribuições (IN RFB nº 1.252/2012), permitindo revisar os dados de cada bloco antes da geração definitiva. Cada bloco reúne um tipo de documento ou apuração — abaixo, o resumo de cada um e os registros que o Sankhya Om gera. Na tela **EFD - Contribuições** (Flex) não existe essa divisão por abas de registro: o conteúdo é descarregado diretamente no arquivo gerado, sem uma etapa própria de revisão por bloco.

**ℹ️ Nota**

Cada bloco termina com um registro de totalização própria (0990, A990, C990, D990, F990, M990, P990, 1990) e o arquivo inteiro fecha com o Bloco 9 (9001, 9900, 9990, 9999). Esses registros são gerados automaticamente pelo sistema em todo arquivo, sem opção de tela para habilitá-los ou desabilitá-los — por isso não aparecem como aba/opção selecionável. O conteúdo campo a campo deles está no Guia Prático oficial.

### Bloco 0 — Abertura, Identificação e Referências

Abre a escrituração e reúne dados cadastrais da pessoa jurídica, o período de apuração e tabelas de referência (produtos, unidades de medida, plano de contas, centros de custo, naturezas de operação) usadas pelos demais blocos. Regras de geração detalhadas em [Geração do Bloco 0](#bloco0).

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Registro</strong></td><td style="border-color: #999; padding: 6px;"><strong>Descrição</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">0000</td><td style="border-color: #999; padding: 6px;">Abertura do Arquivo Digital e Identificação da Pessoa Jurídica</td></tr><tr><td style="border-color: #999; padding: 6px;">0001</td><td style="border-color: #999; padding: 6px;">Abertura do Bloco 0</td></tr><tr><td style="border-color: #999; padding: 6px;">0035</td><td style="border-color: #999; padding: 6px;">Identificação da Sociedade em Conta de Participação - SCP</td></tr><tr><td style="border-color: #999; padding: 6px;">0100</td><td style="border-color: #999; padding: 6px;">Dados do Contabilista</td></tr><tr><td style="border-color: #999; padding: 6px;">0110</td><td style="border-color: #999; padding: 6px;">Regimes de Apuração da Contribuição Social e de Apropriação de Crédito</td></tr><tr><td style="border-color: #999; padding: 6px;">0111</td><td style="border-color: #999; padding: 6px;">Tabela de Receita Bruta Mensal para Fins de Rateio de Créditos Comuns</td></tr><tr><td style="border-color: #999; padding: 6px;">0120</td><td style="border-color: #999; padding: 6px;">Identificação de EFD-Contribuições sem Dados a Escriturar</td></tr><tr><td style="border-color: #999; padding: 6px;">0140</td><td style="border-color: #999; padding: 6px;">Tabela de Cadastro de Estabelecimento</td></tr><tr><td style="border-color: #999; padding: 6px;">0145</td><td style="border-color: #999; padding: 6px;">Regime de Apuração da Contribuição Previdenciária sobre a Receita Bruta (ver nota de descontinuação em <a href="#blocop">Geração do Bloco P</a>)</td></tr><tr><td style="border-color: #999; padding: 6px;">0150</td><td style="border-color: #999; padding: 6px;">Tabela de Cadastro do Participante</td></tr><tr><td style="border-color: #999; padding: 6px;">0190</td><td style="border-color: #999; padding: 6px;">Identificação das Unidades de Medida</td></tr><tr><td style="border-color: #999; padding: 6px;">0200</td><td style="border-color: #999; padding: 6px;">Tabela de Identificação do Item (Produtos e Serviços)</td></tr><tr><td style="border-color: #999; padding: 6px;">0205</td><td style="border-color: #999; padding: 6px;">Alteração do Item</td></tr><tr><td style="border-color: #999; padding: 6px;">0206</td><td style="border-color: #999; padding: 6px;">Código de Produto conforme Tabela ANP (Combustíveis)</td></tr><tr><td style="border-color: #999; padding: 6px;">0208</td><td style="border-color: #999; padding: 6px;">Registro complementar ao 0200/0206 no leiaute atual</td></tr><tr><td style="border-color: #999; padding: 6px;">0400</td><td style="border-color: #999; padding: 6px;">Tabela de Natureza da Operação/Prestação</td></tr><tr><td style="border-color: #999; padding: 6px;">0450</td><td style="border-color: #999; padding: 6px;">Tabela de Informação Complementar do Documento Fiscal — ver <a href="#bloco0">Geração do Bloco 0</a></td></tr><tr><td style="border-color: #999; padding: 6px;">0500</td><td style="border-color: #999; padding: 6px;">Plano de Contas Contábeis – Contas Informadas</td></tr><tr><td style="border-color: #999; padding: 6px;">0600</td><td style="border-color: #999; padding: 6px;">Centro de Custos</td></tr><tr><td style="border-color: #999; padding: 6px;">0900</td><td style="border-color: #999; padding: 6px;">Composição das Receitas do Período – Receita Bruta e Demais Receitas</td></tr></tbody></table>

Consulte também [Campos do registro 0111](https://ajuda.sankhya.com.br/hc/pt-br/articles/15743203960599-Campos-do-registro-0111-EFD-Contribui%C3%A7%C3%B5es) e **Preferências da Empresa** (abas **Regime de Apuração**, **EFD - Escrituração Fiscal Digital**) para o detalhamento de rateio de créditos comuns e habilitação de registros por empresa.

### Bloco A — Documentos Fiscais - Serviços (Sujeitos ao ISS)

Reúne documentos fiscais de prestação de serviços sujeitos ao ISS, para apurar PIS/PASEP e COFINS sobre essas receitas.

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Registro</strong></td><td style="border-color: #999; padding: 6px;"><strong>Descrição</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">A001</td><td style="border-color: #999; padding: 6px;">Abertura do Bloco A</td></tr><tr><td style="border-color: #999; padding: 6px;">A010</td><td style="border-color: #999; padding: 6px;">Identificação do Estabelecimento</td></tr><tr><td style="border-color: #999; padding: 6px;">A100</td><td style="border-color: #999; padding: 6px;">Documento – Nota Fiscal de Serviço</td></tr><tr><td style="border-color: #999; padding: 6px;">A110</td><td style="border-color: #999; padding: 6px;">Complemento de Documento – Informação Complementar da NF</td></tr><tr><td style="border-color: #999; padding: 6px;">A111</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">A120</td><td style="border-color: #999; padding: 6px;">Informação Complementar – Operações de Importação</td></tr><tr><td style="border-color: #999; padding: 6px;">A170</td><td style="border-color: #999; padding: 6px;">Complemento de Documento – Itens do Documento</td></tr></tbody></table>

### Bloco C — Documentos Fiscais I – Mercadorias (ICMS/IPI)

Reúne documentos fiscais de circulação de mercadorias sujeitas ao ICMS/IPI — notas de entrada/saída, cupons fiscais e documentos eletrônicos. Regras de configuração em [Geração do Bloco C](#blococ).

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Registro</strong></td><td style="border-color: #999; padding: 6px;"><strong>Descrição</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">C001</td><td style="border-color: #999; padding: 6px;">Abertura do Bloco C</td></tr><tr><td style="border-color: #999; padding: 6px;">C010</td><td style="border-color: #999; padding: 6px;">Identificação do Estabelecimento</td></tr><tr><td style="border-color: #999; padding: 6px;">C100</td><td style="border-color: #999; padding: 6px;">Documento – NF (código 01), NF Avulsa (1B), NF de Produtor (04) e NF-e (55)</td></tr><tr><td style="border-color: #999; padding: 6px;">C110</td><td style="border-color: #999; padding: 6px;">Complemento de Documento – Informação Complementar da Nota Fiscal (01, 1B, 04, 55)</td></tr><tr><td style="border-color: #999; padding: 6px;">C111</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">C120</td><td style="border-color: #999; padding: 6px;">Complemento de Documento – Operações de Importação (01)</td></tr><tr><td style="border-color: #999; padding: 6px;">C170</td><td style="border-color: #999; padding: 6px;">Complemento de Documento – Itens do Documento (01, 1B, 04, 55)</td></tr><tr><td style="border-color: #999; padding: 6px;">C175</td><td style="border-color: #999; padding: 6px;">Registro Analítico do Documento (65)</td></tr><tr><td style="border-color: #999; padding: 6px;">C180</td><td style="border-color: #999; padding: 6px;">Consolidação de NF-e (55) – Operações de Vendas</td></tr><tr><td style="border-color: #999; padding: 6px;">C181 / C185</td><td style="border-color: #999; padding: 6px;">Detalhamento da Consolidação – Vendas – PIS/PASEP / COFINS</td></tr><tr><td style="border-color: #999; padding: 6px;">C188</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">C190</td><td style="border-color: #999; padding: 6px;">Consolidação de NF-e (55) – Aquisição com Crédito e Devolução de Compras/Vendas</td></tr><tr><td style="border-color: #999; padding: 6px;">C191 / C195</td><td style="border-color: #999; padding: 6px;">Detalhamento – Aquisição com Crédito / Devolução – PIS/PASEP / COFINS</td></tr><tr><td style="border-color: #999; padding: 6px;">C198</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">C199</td><td style="border-color: #999; padding: 6px;">Complemento de Documento – Operações de Importação (55)</td></tr><tr><td style="border-color: #999; padding: 6px;">C380</td><td style="border-color: #999; padding: 6px;">Complemento de Documento – Operações de Importação (55)</td></tr><tr><td style="border-color: #999; padding: 6px;">C381 / C385</td><td style="border-color: #999; padding: 6px;">Detalhamento da Consolidação – PIS/PASEP / COFINS</td></tr><tr><td style="border-color: #999; padding: 6px;">C395 / C396</td><td style="border-color: #999; padding: 6px;">Notas de Venda a Consumidor (02, 2D, 2E, 59) – Aquisições/Entradas com Crédito, e Itens</td></tr><tr><td style="border-color: #999; padding: 6px;">C400</td><td style="border-color: #999; padding: 6px;">Equipamento ECF (02, 2D)</td></tr><tr><td style="border-color: #999; padding: 6px;">C405</td><td style="border-color: #999; padding: 6px;">Redução Z (02, 2D)</td></tr><tr><td style="border-color: #999; padding: 6px;">C481 / C485</td><td style="border-color: #999; padding: 6px;">Resumo Diário ECF – PIS/PASEP / COFINS (02, 2D)</td></tr><tr><td style="border-color: #999; padding: 6px;">C489</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">C490</td><td style="border-color: #999; padding: 6px;">Consolidação de Documentos Emitidos por ECF (02, 2D, 59, 60)</td></tr><tr><td style="border-color: #999; padding: 6px;">C491 / C495</td><td style="border-color: #999; padding: 6px;">Detalhamento da Consolidação ECF – PIS/PASEP / COFINS</td></tr><tr><td style="border-color: #999; padding: 6px;">C499</td><td style="border-color: #999; padding: 6px;">Processo Referenciado – Documentos Emitidos por ECF</td></tr><tr><td style="border-color: #999; padding: 6px;">C500</td><td style="border-color: #999; padding: 6px;">NF/Conta de Energia Elétrica (06), NF3e (66), Água Canalizada (29), Gás (28) e NF-e (55) – Entrada/Aquisição com Crédito</td></tr><tr><td style="border-color: #999; padding: 6px;">C501 / C505</td><td style="border-color: #999; padding: 6px;">Complemento da operação (06, 28, 29) – PIS/PASEP / COFINS</td></tr><tr><td style="border-color: #999; padding: 6px;">C509</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">C600</td><td style="border-color: #999; padding: 6px;">Consolidação das Notas Fiscais/Contas de Energia Elétrica, Gás Canalizado e Água Canalizada emitidas pela empresa (concessionárias)</td></tr><tr><td style="border-color: #999; padding: 6px;">C601 / C605</td><td style="border-color: #999; padding: 6px;">Complemento da Consolidação – PIS/PASEP / COFINS</td></tr><tr><td style="border-color: #999; padding: 6px;">C609</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">C800</td><td style="border-color: #999; padding: 6px;">Cupom Fiscal Eletrônico – CF-e (59)</td></tr><tr><td style="border-color: #999; padding: 6px;">C810</td><td style="border-color: #999; padding: 6px;">Detalhamento do CF-e (59) – PIS/PASEP e COFINS</td></tr><tr><td style="border-color: #999; padding: 6px;">C860</td><td style="border-color: #999; padding: 6px;">Identificação do Equipamento SAT CF-e (59)</td></tr><tr><td style="border-color: #999; padding: 6px;">C870</td><td style="border-color: #999; padding: 6px;">Detalhamento do Cupom Fiscal Eletrônico (59) – PIS/PASEP e COFINS</td></tr></tbody></table>

Os registros C600/C601/C605/C609 dependem de lançamento manual dos dados na grade própria desta aba — não são derivados automaticamente de notas fiscais de energia/água/gás lançadas no sistema. Os campos **Alíq. PIS/PASEP** e **Alíq. do COFINS** dos registros A170 e C170 são preenchidos com a mesma quantidade de casas decimais do cadastro de alíquotas e do cálculo da nota, refletida tanto na tela quanto no arquivo TXT. Consulte também as validações para geração do C100 e o detalhamento de C180/C190 e seus registros filhos em [Geração do Bloco C](#blococ).

### Bloco D — Documentos Fiscais II – Serviços (ICMS)

Reúne documentos fiscais de transporte e comunicação/telecomunicação sujeitos ao ICMS. Regras de configuração em [Geração do Bloco D](#blocod).

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Registro</strong></td><td style="border-color: #999; padding: 6px;"><strong>Descrição</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">D001</td><td style="border-color: #999; padding: 6px;">Abertura do Bloco D</td></tr><tr><td style="border-color: #999; padding: 6px;">D010</td><td style="border-color: #999; padding: 6px;">Identificação do Estabelecimento</td></tr><tr><td style="border-color: #999; padding: 6px;">D100</td><td style="border-color: #999; padding: 6px;">Aquisição de Serviços de Transportes (07, 08, 8B, 09, 10, 11, 26, 27, 57, 63, 67)</td></tr><tr><td style="border-color: #999; padding: 6px;">D101 / D105</td><td style="border-color: #999; padding: 6px;">Complemento do Documento de Transporte – PIS/PASEP / COFINS</td></tr><tr><td style="border-color: #999; padding: 6px;">D111</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">D200</td><td style="border-color: #999; padding: 6px;">Resumo da Escrituração Diária – Transportes</td></tr><tr><td style="border-color: #999; padding: 6px;">D201 / D205</td><td style="border-color: #999; padding: 6px;">Totalização do Resumo Diário – PIS/PASEP / COFINS</td></tr><tr><td style="border-color: #999; padding: 6px;">D209</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">D500</td><td style="border-color: #999; padding: 6px;">NF de Serviço de Comunicação (21) e Telecomunicação (22) – Aquisição com Crédito</td></tr><tr><td style="border-color: #999; padding: 6px;">D501 / D505</td><td style="border-color: #999; padding: 6px;">Complemento da Operação – PIS/PASEP / COFINS</td></tr><tr><td style="border-color: #999; padding: 6px;">D509</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">D600</td><td style="border-color: #999; padding: 6px;">Consolidação da Prestação de Serviços – Comunicação (21) e Telecomunicação (22)</td></tr><tr><td style="border-color: #999; padding: 6px;">D601 / D605</td><td style="border-color: #999; padding: 6px;">Complemento da Consolidação – PIS/PASEP / COFINS</td></tr></tbody></table>

### Bloco F — Demais Documentos e Operações

Reúne documentos e operações geradoras de receitas ou créditos fora dos blocos A, C ou D — lucro presumido, retenções na fonte, atividade imobiliária. Regras de configuração em [Geração do Bloco F](#blocof).

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Registro</strong></td><td style="border-color: #999; padding: 6px;"><strong>Descrição</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">F001</td><td style="border-color: #999; padding: 6px;">Abertura do Bloco F</td></tr><tr><td style="border-color: #999; padding: 6px;">F010</td><td style="border-color: #999; padding: 6px;">Identificação do Estabelecimento</td></tr><tr><td style="border-color: #999; padding: 6px;">F100</td><td style="border-color: #999; padding: 6px;">Demais Documentos e Operações Geradoras de Contribuição e Créditos</td></tr><tr><td style="border-color: #999; padding: 6px;">F111</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">F120</td><td style="border-color: #999; padding: 6px;">Bens Incorporados ao Ativo Imobilizado – Créditos com Base nos Encargos de Depreciação/Amortização</td></tr><tr><td style="border-color: #999; padding: 6px;">F129</td><td style="border-color: #999; padding: 6px;">Detalhamento dos ajustes de crédito informado no F120</td></tr><tr><td style="border-color: #999; padding: 6px;">F130</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">F139</td><td style="border-color: #999; padding: 6px;">Detalhamento dos ajustes de crédito informado no F130</td></tr><tr><td style="border-color: #999; padding: 6px;">F200</td><td style="border-color: #999; padding: 6px;">Operações da Atividade Imobiliária – Unidade Imobiliária Vendida</td></tr><tr><td style="border-color: #999; padding: 6px;">F205</td><td style="border-color: #999; padding: 6px;">Operações da Atividade Imobiliária – Custo Incorrido da Unidade Imobiliária</td></tr><tr><td style="border-color: #999; padding: 6px;">F210</td><td style="border-color: #999; padding: 6px;">Operações da Atividade Imobiliária – Custo Orçado da Unidade Imobiliária Vendida</td></tr><tr><td style="border-color: #999; padding: 6px;">F500</td><td style="border-color: #999; padding: 6px;">Consolidação das Operações – Lucro Presumido, Regime de Caixa</td></tr><tr><td style="border-color: #999; padding: 6px;">F509</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">F510</td><td style="border-color: #999; padding: 6px;">Consolidação das Operações – Lucro Presumido, Regime de Caixa (por Unidade de Medida)</td></tr><tr><td style="border-color: #999; padding: 6px;">F525</td><td style="border-color: #999; padding: 6px;">Composição da Receita Escriturada no Período – Detalhamento da Receita Recebida no Regime de Caixa</td></tr><tr><td style="border-color: #999; padding: 6px;">F550</td><td style="border-color: #999; padding: 6px;">Consolidação das Operações – Lucro Presumido, Regime de Competência</td></tr><tr><td style="border-color: #999; padding: 6px;">F559</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">F560</td><td style="border-color: #999; padding: 6px;">Consolidação das Operações – Lucro Presumido, Regime de Competência (por Unidade de Medida)</td></tr><tr><td style="border-color: #999; padding: 6px;">F600</td><td style="border-color: #999; padding: 6px;">Contribuição Retida na Fonte</td></tr></tbody></table>

### Bloco I — Instituições Financeiras, Seguradoras, Entidades de Previdência Privada e Operadoras de Planos de Saúde

O Bloco I não possui nenhum registro gerado pelo sistema Sankhya Om.

### Bloco M — Apuração da Contribuição e Crédito do PIS/Pasep e da Cofins

Consolida a apuração da contribuição devida e dos créditos de PIS/PASEP e COFINS do período, a partir dos blocos A, C, D e F. Regras de configuração em [Geração do Bloco M](#blocom).

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Registro</strong></td><td style="border-color: #999; padding: 6px;"><strong>Descrição</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">M001</td><td style="border-color: #999; padding: 6px;">Abertura do Bloco M</td></tr><tr><td style="border-color: #999; padding: 6px;">M100 / M110 / M115</td><td style="border-color: #999; padding: 6px;">Crédito de PIS/PASEP do Período, Ajustes e Detalhamento dos Ajustes</td></tr><tr><td style="border-color: #999; padding: 6px;">M200</td><td style="border-color: #999; padding: 6px;">Consolidação da Contribuição para o PIS/PASEP do Período</td></tr><tr><td style="border-color: #999; padding: 6px;">M400 / M410</td><td style="border-color: #999; padding: 6px;">Receitas Isentas/Não Alcançadas/Alíquota Zero/Suspensão – PIS/PASEP, e Detalhamento</td></tr><tr><td style="border-color: #999; padding: 6px;">M500 / M510 / M515</td><td style="border-color: #999; padding: 6px;">Crédito de COFINS do Período, Ajustes e Detalhamento dos Ajustes</td></tr><tr><td style="border-color: #999; padding: 6px;">M600</td><td style="border-color: #999; padding: 6px;">Consolidação da Contribuição para a Seguridade Social - COFINS do Período</td></tr><tr><td style="border-color: #999; padding: 6px;">M800 / M810</td><td style="border-color: #999; padding: 6px;">Receitas Isentas/Não Alcançadas/Alíquota Zero/Suspensão – COFINS, e Detalhamento</td></tr></tbody></table>

Consulte também [Registros M200 e M600 - EFD Contribuições](https://ajuda.sankhya.com.br/hc/pt-br/articles/25870502453783-Registros-M200-e-M600-EFD-Contribui%C3%A7%C3%B5es) para o detalhamento da consolidação da contribuição do período.

### Bloco P — Apuração da CPRB (descontinuado)

Ver aviso de descontinuação em [Geração do Bloco P](#blocop).

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Registro</strong></td><td style="border-color: #999; padding: 6px;"><strong>Descrição</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">P001</td><td style="border-color: #999; padding: 6px;">Abertura do Bloco P</td></tr><tr><td style="border-color: #999; padding: 6px;">P010</td><td style="border-color: #999; padding: 6px;">Identificação do Estabelecimento</td></tr><tr><td style="border-color: #999; padding: 6px;">P100</td><td style="border-color: #999; padding: 6px;">Contribuição Previdenciária sobre a Receita Bruta</td></tr><tr><td style="border-color: #999; padding: 6px;">P199</td><td style="border-color: #999; padding: 6px;">Processo Referenciado</td></tr><tr><td style="border-color: #999; padding: 6px;">P200</td><td style="border-color: #999; padding: 6px;">Consolidação da Contribuição Previdenciária sobre a Receita Bruta</td></tr></tbody></table>

Consulte também [Registro P100 do EFD Contribuições](https://ajuda.sankhya.com.br/hc/pt-br/articles/26555446175639-Registro-P100-do-EFD-Contribui%C3%A7%C3%B5es) e [Registro P200 do EFD Contribuições](https://ajuda.sankhya.com.br/hc/pt-br/articles/26584002832535-Registro-P200-do-EFD-Contribui%C3%A7%C3%B5es).

### Bloco 1 — Complemento da Escrituração

Reúne informações complementares — processos judiciais/administrativos referenciados, controle de créditos fiscais e valores retidos na fonte, e consolidação de documentos no regime de lucro presumido. Regras de configuração em [Geração do Bloco 1](#bloco1).

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Registro</strong></td><td style="border-color: #999; padding: 6px;"><strong>Descrição</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">1001</td><td style="border-color: #999; padding: 6px;">Abertura do Bloco 1</td></tr><tr><td style="border-color: #999; padding: 6px;">1010</td><td style="border-color: #999; padding: 6px;">Processo Referenciado – Ação Judicial</td></tr><tr><td style="border-color: #999; padding: 6px;">1011</td><td style="border-color: #999; padding: 6px;">Detalhamento das Contribuições com Exigibilidade Suspensa</td></tr><tr><td style="border-color: #999; padding: 6px;">1020</td><td style="border-color: #999; padding: 6px;">Processo Referenciado – Processo Administrativo</td></tr><tr><td style="border-color: #999; padding: 6px;">1100 / 1300</td><td style="border-color: #999; padding: 6px;">Controle de Créditos Fiscais / Valores Retidos na Fonte – PIS/PASEP</td></tr><tr><td style="border-color: #999; padding: 6px;">1500 / 1700</td><td style="border-color: #999; padding: 6px;">Controle de Créditos Fiscais / Valores Retidos na Fonte – COFINS</td></tr><tr><td style="border-color: #999; padding: 6px;">1900</td><td style="border-color: #999; padding: 6px;">Consolidação dos Documentos Emitidos – Lucro Presumido, Regime de Caixa ou Competência</td></tr></tbody></table>

### Bloco 9 — Controle e Encerramento do Arquivo Digital

Bloco de controle técnico: contabiliza a quantidade de registros gerados em cada bloco e encerra a escrituração. Gerado automaticamente, sem opção de tela para habilitar ou desabilitar (ver nota no início desta seção).

[↑ Voltar ao início](#sumario)

---

## Botões da tela

**Processar** (HTML5) — realiza, de acordo com a **Aba Configurações**, a geração e o preenchimento das guias referentes aos registros do arquivo, trazendo os dados para revisão em tela antes da geração definitiva. Após processar um período, se precisar alterar alguma configuração, processe novamente para que o sistema salve as modificações.

**⚠️ Atenção**

Se o arquivo já estiver com a marcação **Arquivo Confirmado** ativa, o botão **Processar** é bloqueado, com mensagem informando que é necessário desmarcar essa opção (em **Outras Opções**) antes de reprocessar. Depois de confirmado, o arquivo é imutável — por isso a etapa **Processar** existe separadamente de **Gerar**: ela permite revisar e corrigir dados antes dessa confirmação, que depois não pode mais ser desfeita.

**Gerar** (HTML5) — realiza, de acordo com as abas **Configurações** e **Opções**, a geração do arquivo de escrituração.

**Histórico de Gerações** — exibe o histórico das gerações de arquivo realizadas.

**Outras Opções › Reprocessar Registros Totalizadores** — recalcula e atualiza, nas tabelas de banco, a quantidade de linhas dos totalizadores de cada bloco (campo **Qtd. total linhas Bloco (x)**). Esta ação não gera nem altera o arquivo TXT — ela só corrige os contadores em banco/tela quando um registro de alguma aba de bloco foi excluído; para que a mudança apareça no arquivo, gere-o novamente pelo botão **Gerar**.

Na tela **EFD - Contribuições** (Flex), o fluxo é diferente: um único botão principal, **Gerar Arquivo** (acumula Processar + Gerar desta tela, com uma única tela de confirmação), um botão próprio de **Histórico de gerações**, e um botão **Consultar Nota Não Gerada** — que permite consultar uma nota não gerada no livro, filtrando por **Nro. Nota**, **Série**, **Data de Negociação** e **Empresa**. Não há confirmação de equivalente desses dois últimos itens (Histórico e Consultar Nota) na tela HTML5, além do próprio **Histórico de Gerações** listado acima.

[↑ Voltar ao início](#sumario)

---

## Modalidades de Apuração das Contribuições

A contribuição para o PIS/PASEP compreende três modalidades: sobre o Faturamento, sobre a Folha de Pagamento (não gerado no SPED Contribuições) e sobre Importação. Na modalidade Faturamento, contribuem as pessoas jurídicas de direito privado e equiparadas; na modalidade Folha de Pagamento, contribuem as entidades sem fins lucrativos com empregados. A COFINS existe nas modalidades Faturamento e Importação.

[↑ Voltar ao início](#sumario)

---

## Regimes

Existem dois regimes para PIS/PASEP e COFINS incidentes sobre o faturamento.

*   **Regime Cumulativo** — incide sobre o faturamento total, sem direito a deduções de créditos; percentual fixo recolhido mensalmente.
*   **Regime Não-cumulativo** — criado em dezembro/2002 (PIS/PASEP) e fevereiro/2004 (COFINS); sistema de créditos e débitos que se compensam. Alíquota maior, mas reduz a carga tributária de empresas que utilizam insumos e matéria-prima, permitindo que estes gerem créditos abatidos do valor final devido.

[↑ Voltar ao início](#sumario)

---

## Geração do Bloco 0

O Bloco 0 é o último a ser processado internamente pelo sistema — ele depende dos totalizadores acumulados pelos demais blocos (A, C, D, F, M, P, 1) para fechar corretamente.

### Regra de habilitação

A geração de cada registro do Bloco 0 (0000, 0001, 0035, 0100 até 0900) não é incondicional: cada um tem seu próprio "interruptor", controlado pelo mesmo cadastro de Blocos e Registros habilitados em **Preferências da Empresa** (aba **EFD - Escrituração Fiscal Digital**) citado em [Antes de começar](#antes) — por empresa e tipo de escrituração. Os registros 0000/0001 também são gerados em modo "geração sem dados" (Registro 0120), independentemente dessa marcação.

### Observações de nota → registro 0450

O registro 0450 (Tabela de Informação Complementar do Documento Fiscal) é alimentado pelo mesmo cadastro de **Observação** vinculado à nota fiscal que também alimenta os registros de informação complementar de documento — A110, C110, C500, D100 e D500 — em todos os blocos. Ou seja: a mesma observação cadastrada e vinculada ao cabeçalho da nota serve, ao mesmo tempo, para compor a informação complementar do documento (nos blocos A/C/D) e o registro 0450 do Bloco 0. Duas marcações no cadastro da observação controlam esse comportamento: uma flag que habilita a geração dessa observação no EFD (sem ela marcada, a observação não entra no arquivo, em nenhum dos dois lugares), e uma flag que decide se o texto livre digitado na nota — não apenas a observação padrão — deve compor o campo de texto complementar do registro. Esse mesmo mecanismo também é a base do parâmetro `ADDOBSERVALIQ` (ver [Parâmetros que influenciam a rotina](#parametros)), que controla se uma observação vinculada à alíquota de ICMS do item é considerada na geração do registro C110. Consulte também [Observações para Notas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044596474-Observa%C3%A7%C3%B5es-para-Notas).

**⚠️ Atenção**

O registro 0400 (Tabela de Natureza da Operação/Prestação) não tem relação com observações de nota — ele é preenchido a partir do cadastro de [Tipo de Operação (TOP)](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP) e não deve ser confundido com o 0450.

[↑ Voltar ao início](#sumario)

---

## Geração do Bloco C

A **Conta Contábil** configurada alimenta um campo específico de determinados registros deste bloco (como A170 e C170) — veja o processo Geração da Conta Contábil para EFD - Contribuições.

É necessário preencher adequadamente a aba **Regime de Apuração da Contribuição Social e de Apropriação de Crédito** (Preferências da Empresa), cobrindo o intervalo do período a gerar — por exemplo, para gerar o período de 01/04/2017 a 30/04/2017, esse intervalo precisa estar cadastrado ali.

**⚠️ Atenção**

Sem cadastro para o período, o sistema recusa a geração com a mensagem _"Empresa X Preferências da Empresa, aba 'Regime de Apuração da Contribuição Social e de Apropriação de Crédito' não foi encontrado o cadastro para a data inicial do período informado."_ Com datas intercaladas (mais de um cadastro cobrindo a mesma data inicial), a mensagem é _"...foram encontrados mais de um cadastro para a data inicial do período informado e isto não pode."_

O valor do ICMS que não entra na base do PIS/COFINS vai no campo **Vlr. desc. com./excl. base cálc. PIS/PASEP e COFINS** (campo 15). Para isso, selecione **Deduz para NF-e** no campo **Deduzir valor do ICMS na BC do PIS e COFINS?** (aba **Propriedades**, Preferências da Empresa) e ligue o parâmetro `REDICMSBCPISCOF` (Redução do ICMS da BC do PIS e COFINS).

O registro C100 de notas com CST 98/99 de Devolução de Vendas de PIS/COFINS é gerado quando o parâmetro `OENSEMCREDEFDCT` (Gerar reg. sem créd. PIS/COFINS no EFD Out. Entr.) está ligado.

O parâmetro `UFEFDVLMERC` (UF que soma valor não apropriado ao VLR\_MERC) garante a consistência de valores entre o EFD Contribuições e o EFD ICMS/IPI nos registros C100 e C170.

*   **Como funciona:** se a UF da empresa estiver informada no parâmetro e a operação **não** tiver direito a crédito, o sistema soma automaticamente os valores de IPI e ICMS-ST ao campo **VLR\_MERC** (Registro C100) e **VL\_ITEM** (Registro C170).
*   **Comportamento padrão:** se a UF não estiver no parâmetro ou a operação tiver direito a crédito, o sistema mantém o comportamento padrão e considera apenas o valor do item, sem somar IPI e ICMS-ST.

[↑ Voltar ao início](#sumario)

---

## Geração do Bloco D

A **Conta Contábil** configurada alimenta um campo específico de registros como D100, D101 e D105 — veja o processo Geração da Conta Contábil para EFD - Contribuições.

### Indicador de Frete no registro D100

O sistema usa o tomador do serviço de frete e seu valor para preencher o campo **Indicador do tipo do frete** no registro D100, conforme o Manual do Layout 1.05 / Código 006 do SPED Fiscal, para os modelos CT-e 57 e 67.

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Indicador</strong></td><td style="border-color: #999; padding: 6px;"><strong>Significado</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">0</td><td style="border-color: #999; padding: 6px;">Por conta do emitente</td></tr><tr><td style="border-color: #999; padding: 6px;">1</td><td style="border-color: #999; padding: 6px;">Por conta do destinatário/remetente</td></tr><tr><td style="border-color: #999; padding: 6px;">2</td><td style="border-color: #999; padding: 6px;">Por conta de terceiros</td></tr><tr><td style="border-color: #999; padding: 6px;">9</td><td style="border-color: #999; padding: 6px;">Sem cobrança de frete</td></tr></tbody></table>

*   **Lançamento pela Movimentação Financeira** — frete registrado com tomador = empresa e valor > 0 gera indicador automaticamente **1 - Por conta do destinatário/remetente**.
*   **Lançamento pelo Portal de Compras** — mesmo comportamento nas mesmas condições.

Nesses casos não é necessário configurar manualmente o indicador — basta lançar normalmente e gerar o Livro PIS/COFINS e a EFD-Contribuições. Consulte também [Como realizar o cálculo proporcional de PIS/COFINS para Frete](https://ajuda.sankhya.com.br/hc/pt-br/articles/26556855929495-Como-realizar-o-c%C3%A1lculo-proporcional-de-PIS-COFINS-para-Frete).

### Geração dos registros D600, D601 e D605

Em **Preferências da Empresa**, aba **EFD - Escrituração Fiscal Digital**, selecione o **Bloco D** e, para cada um dos três registros (D600, D601, D605), marque **Gerar Registro**.

Pré-requisitos adicionais:

1.  Na TOP usada no lançamento (aba **Impostos**), o campo **Indicador do Tipo de Receita** deve estar preenchido.
2.  Crie os códigos de Classificação de Serviços de Comunicação/Telecomunicação na tela [**Lista de Serviços de Telecomunicação**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112193-Lista-de-Servi%C3%A7os-de-Telecomunica%C3%A7%C3%A3o).
3.  Vincule, no [**Cadastro de Serviço**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Cadastro-de-Servi%C3%A7o) (aba **Impostos**), o campo **Cód. Serviço de Telecomunicação** ao código de Classificação criado.

[↑ Voltar ao início](#sumario)

---

## Geração do Bloco F

A **Conta Contábil** configurada alimenta um campo específico de registros como F100, F500 e F525 — veja o processo Geração da Conta Contábil para EFD - Contribuições. Consulte também [Geração Registro F100 EFD Contribuições](https://ajuda.sankhya.com.br/hc/pt-br/articles/4404590165911-Gera%C3%A7%C3%A3o-Registo-F100-EFD-Contribui%C3%A7%C3%B5es-Saiba-mais) e [Geração do Registro F550 - EFD Contribuições](https://ajuda.sankhya.com.br/hc/pt-br/articles/7066461017239-Gera%C3%A7%C3%A3o-do-Registro-F550-EFD-Contribui%C3%A7%C3%B5es).

### Registro F500

Detalha a base de cálculo e os valores apurados de PIS/PASEP e COFINS sobre a receita bruta. Está diretamente relacionado ao F525 (composição das receitas), considerando a marcação **Considera Valores de Juros e Multa na Geração do F525** (aba **Regime de Apuração da Contrib. Social e Aprop. Crédito**, Preferências da Empresa). Campos preenchidos: **Vlr. base cálc. do PIS/PASEP**, **Vlr. do PIS/PASEP**, **Vlr. base cálc. da COFINS**, **Vlr. da COFINS** — extraídos conforme as regras fiscais, garantindo que só receitas tributáveis componham a base.

### Registro F525

Relaciona a composição de todas as receitas recebidas no período, sujeitas ou não à contribuição.

*   Com **Desconsidera Itens com/de Terceiros no F525** ativada, só entram as CST's de Serviços de Industrialização (desconsiderando Matéria-Prima). Exemplo: numa movimentação com Produto Acabado CST 01 e Retorno MP CST 08, só a CST 01 é exibida.
*   Com a marcação desligada, entram tanto Serviços de Industrialização quanto Matéria-Prima — no mesmo exemplo, as CST's 01 e 08 aparecem separadamente.
*   Com **Considera Valores de Juros e Multa na Geração do F525** ativada, a soma do desdobramento + juros + multa aparece nos campos de valor total da receita recebida e valor da receita detalhada do TXT, evitando inconsistências em documentos com múltiplos CFOPs.

### Registro F550

Os campos **05 - VL\_BC\_PIS** e **10 - VL\_BC\_COFINS** devem desconsiderar valores de Devoluções de Venda. Para identificar a linha a deduzir, o sistema identifica as NF's de Venda correspondentes, usando CST, % Alíquota e CFOP (campos 03-CST\_PIS, 06-ALIQ\_PIS, 08-CST\_COFINS, 11-ALIQ\_COFINS, 14-CFOP).

[↑ Voltar ao início](#sumario)

---

## Geração do Bloco M

Para o detalhamento das receitas não tributadas (registros M400/M410/M800/M810), preencha manualmente o campo **Cód. Natureza (PIS/COFINS M410/M800)** no [**Cadastro de Produtos**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos), aba **Impostos** (vazio por padrão), conforme as tabelas de natureza do manual do SPED Contribuições. Até que essa configuração esteja completa em todos os produtos, desmarque em **Preferências da Empresa** a geração dos registros M400, M410, M800 e M810.

### Regras de acumulação

*   Acumulam no M410: A170, C170, C181, C381, C481, C491, D201.
*   Acumulam no M810: A170, C170, C185, C385, C485, C495, D205.
*   Sem regra de acumulação em M410/M810: F100, F510, F550, F560.
*   Ainda não gerados (e, portanto, não acumulam M410/M810): C601, D601, D300, D350, F200, I100.

Itens com código de natureza inválido são registrados no log de geração ao final do procedimento, com mensagem semelhante a _"O Código da Natureza (0) para o M410 cadastrado no produto (YYY) é inválido"_. Depois de gerado o EFD Contribuições com M400/M410 e M800/M810, use a funcionalidade do validador do PVA para gerar apurações — ele não sobrepõe os valores já gerados desses registros, apenas completa as demais informações do bloco M.

Informações adicionais sobre o M410: deduza os valores de Devoluções de Vendas (retirados do campo 03-VL\_REC, com base na CST do campo 02 da venda), identificando as NF's de Venda correspondentes (CST, % Alíquota, CFOP). Não é obrigatório ter as NF's de Venda na movimentação para esse processo.

[↑ Voltar ao início](#sumario)

---

## Geração do Bloco P (descontinuado)

**⚠️ Atenção**

Bloco P descontinuado a partir dos fatos geradores de 01/01/2025. A Contribuição Previdenciária sobre a Receita Bruta (CPRB) migrou para a EFD-Reinf, conforme a Nota Técnica 07/2018 da Receita Federal. Desde então, não é mais possível escriturar o registro 0145 nem nenhum registro do Bloco P no validador (PVA) da EFD-Contribuições — o arquivo seria rejeitado. Esta seção é mantida apenas como referência histórica, para consulta de períodos anteriores a essa data. Para apuração de CPRB atual, veja a documentação de [EFD-Reinf](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116553-EFD-Reinf) (Ajustes e Códigos de Atividade CPRB). Para saber mais sobre a migração, acesse [Descontinuação do Bloco P - EFD Contribuições](https://ajuda.sankhya.com.br/hc/pt-br/articles/29596723199127-Descontinua%C3%A7%C3%A3o-do-Bloco-P-EFD-Contribui%C3%A7%C3%B5es).

A geração do registro P100 depende da configuração da **Conta Contábil** — veja o processo Geração da Conta Contábil para EFD - Contribuições.

Para períodos anteriores a 01/01/2025: em **Preferências da Empresa**, aba **EFD - Escrituração Fiscal Digital**, selecione o **Bloco P** e marque **Gerar Registro** no P100. Pré-requisitos:

1.  No **Cadastro de Produtos** (aba **Impostos**), marque **Enquadrado no Reintegra/Prev.**.
2.  Preencha o campo **Cód. Atividade CPRB (Reintegra/Prev.)** — quando preenchido, usa os dados da tela [**Cód. Atividades Produtos e Serviços p/ CPRB**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044608314-C%C3%B3d-Atividades-Produtos-e-Servi%C3%A7os-p-CPRB). Se vazio, o sistema busca o código de atividade em **Preferências da Empresa**, aba **Reintegra Previdência**.
3.  O mesmo procedimento vale no **Cadastro de Serviços** (aba **Impostos**); sem a marcação **Enquadrado no Reintegra/Prev.**, nenhuma informação é gerada para o Bloco P.

[↑ Voltar ao início](#sumario)

---

## Geração do Bloco 1

A **Conta Contábil** configurada alimenta um campo específico do registro 1900 — veja o processo Geração da Conta Contábil para EFD - Contribuições.

### Registro 1900

Para o Registro 1900 (Consolidação dos Documentos Emitidos no Período por PJ no Lucro Presumido – Regime de Caixa ou Competência), deduza os valores de Devoluções de Vendas — retirados do campo 07-VL\_TOT\_REC, com base nas CST's (campos 09 e 10) e CFOP (campo 11) da venda. Identifique as NF's de Venda correspondentes (CST, % Alíquota, CFOP) para o processo de dedução; não é obrigatório ter as NF's de Venda na movimentação.

[↑ Voltar ao início](#sumario)

---

## Processo Judicial

Na geração do EFD-Contribuições, é obrigatório informar o processo judicial quando houver dedução/exclusão na base de cálculo do PIS/COFINS. Os registros envolvidos, quando há processo judicial vinculado, são:

*   A170 › A111
*   C170, C175
*   C181/C185, C381/C385
*   C481/C485 › C489
*   C499 (Documentos Emitidos por ECF)
*   C870 › C890
*   D201/D205 › D209
*   F100 › F111
*   F500 › F509
*   F550 › F559
*   P100 › P199

**⚠️ Atenção**

Se a exclusão da base de cálculo decorrer de decisão judicial favorável e já aplicável ao período desta escrituração, é obrigatório escriturar o Registro C111 - Processo Referenciado (ou o processo referenciado equivalente do bloco correspondente), além do detalhamento no Registro 1010 - Processo Referenciado – Ação Judicial. Isso vale para a pessoa jurídica beneficiária ou autora da ação, com sentença favorável à exclusão de impostos incidentes na venda de bens/serviços na determinação da base de cálculo do PIS/PASEP, da COFINS e/ou da CPRB — desde que não haja limitação temporal dos efeitos da sentença em relação ao período escriturado.

Os registros 1010/1011 só são gerados quando existe, na tela de cadastro de [Processos Administrativos/Judiciais](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044608094-Processos-Administrativos-Judiciais), um processo cadastrado com o mesmo número/sequencial referenciado no documento fiscal (incluindo a sub-aba de Suspensão de Exigibilidade do Tributo). Sem esse cadastro correspondente, nenhuma informação de processo é escriturada — mesmo que o documento tenha sido lançado com indicação de origem judicial.

São gerados também os registros C180 e C190 de consolidação das NF-e, correspondentes ao complemento das instruções de preenchimento do campo 06 (COD\_NCM).

[↑ Voltar ao início](#sumario)

---

## Configuração e Consolidação por Estabelecimentos

**ℹ️ Nota**

Exclusivo da tela HTML5, a partir da versão 4.32. Não existe na tela Flex. Aplica-se exclusivamente à geração do SPED Consolidado, quando há estabelecimentos cadastrados como empresas usando o CNPJ da matriz ou de filiais, com ou sem inscrição estadual distinta.

### Configuração

Em **Preferências da Empresa**, aba **Propriedades**, preencha o campo **Empresa Matriz (EFD)**. No cadastro da matriz, o campo **Indicador da apuração das contribuições e créditos** (aba **EFD - Escrituração Fiscal Digital**) deve estar como **2 - Apuração com base nos registros individualizados de NF-e e ECF**.

### Consolidação

Na geração do arquivo, o sistema agrupa os movimentos por CNPJ distinto do grupo, seguindo o Guia Prático do EFD. O comportamento depende do parâmetro `GERREGORDEFD` (Gera registros ordenados no EFD consolidado):

*   **Registro 0140** — com o parâmetro ligado, é gerado separadamente por matriz/filial/estabelecimento (mesmo com CNPJ igual) quando os livros são gerados individualmente; se consolidados, unifica por CNPJ. Desligado, sempre consolida por CNPJ, independentemente da forma de geração.
*   **Registro A010** — mesmo padrão do 0140.
*   **Registro C010** — mesmo padrão do 0140.
*   **Registro D010** — com o parâmetro ligado, gerado separadamente por unidade (mesmo com CNPJ igual) quando individualizado; consolidado, unifica por CNPJ — e o 0140 acompanha essa mesma lógica. Os registros derivados (D100, D101, D105, D500, D501, D505) seguem essa mesma individualização/consolidação por CNPJ. Desligado, tudo consolida pelo CNPJ da empresa geradora dos livros (normalmente a matriz).
*   **Registro F010** — mesmo padrão do 0140/A010/C010. Registros derivados: F100 (um por CNPJ), F111 (detalha por transação), F120 (pode sair em três formatos: lotes individuais por empresa; lotes consolidados matriz+estabelecimentos com filial individual; ou um único lote consolidando tudo), F130 (por CNPJ).

O parâmetro `SPEDC500SEPA` (Gera bloco C100 e C500 ordenados do EFD para consolidados) ajusta a ordem de C100/filhos antes de C500/filhos em empresas consolidadas com mesmo CNPJ. `GERREGORDEFD` tem prioridade sobre ele: ligado, sobrepõe; desligado, prevalece o `SPEDC500SEPA`. Com os dois ligados, todo o Bloco C (C010, C100, C170, C175, C500, C501, C505) sai em ordem, evitando erros de validação no PVA.

[↑ Voltar ao início](#sumario)

---

## Parâmetros que influenciam a rotina

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Parâmetro</strong></td><td style="border-color: #999; padding: 6px;"><strong>Efeito</strong></td></tr><tr><td style="border-color: #999; padding: 6px;"><code>MASCTGFLST</code> (Máscara para Lista de Serviços)</td><td style="border-color: #999; padding: 6px;">O campo COD_LST do registro 0200 tem no máximo 4 caracteres — se a máscara configurada for maior, o sistema usa só os 4 primeiros caracteres (esquerda→direita).</td></tr><tr><td style="border-color: #999; padding: 6px;"><code>USADTENTSAISERV</code> (Usa DTENTSAI para data execução do serviço)</td><td style="border-color: #999; padding: 6px;">Ligado: o campo 11 do registro A100 usa a Data Entrada/Saída da nota (exclusivo para escrituração de Serviços). Desligado: mantém a Data de Negociação da nota.</td></tr><tr><td style="border-color: #999; padding: 6px;"><code>F600RETDHBAIXA</code> (Usar a dt. da baixa como dt. de retenção do F600)</td><td style="border-color: #999; padding: 6px;">Ligado: usa a data da baixa financeira da nota como filtro para gerar o registro F600. Se a retenção de PIS/COFINS estiver configurada para ocorrer no lançamento da nota (não na baixa), o sistema alerta que a(s) nota(s) não foram incluídas no F600 e não o gera para elas. Consulte também <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360047215514-Como-gerar-o-Registro-F600-Contribui%C3%A7%C3%A3o-Retida-na-Fonte-no-EFD-Contribui%C3%A7%C3%B5es">Como gerar o Registro F600: Contribuição Retida na Fonte</a>.</td></tr><tr><td style="border-color: #999; padding: 6px;"><code>DESCOPERDESCNAT</code> (Usa a descrição da operação com a descrição da nat.)</td><td style="border-color: #999; padding: 6px;">Na geração do F100, usa a descrição da natureza vinculada à movimentação financeira para preencher o campo 19 (Descrição do Documento/Operação).</td></tr><tr><td style="border-color: #999; padding: 6px;"><code>ADDOBSERVALIQ</code> (Adicionar observação Alíq. ICMS no C110)</td><td style="border-color: #999; padding: 6px;">Habilita, no registro C110, a geração de uma observação vinculada ao Cód. Alíq. ICMS do item (tela de <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360044602934-Al%C3%ADquotas-de-ICMS">Alíquota de ICMS</a>) — além da observação padrão do cabeçalho da nota. Ver o mesmo mecanismo de observações em <a href="#bloco0">Geração do Bloco 0</a> (registro 0450).</td></tr><tr><td style="border-color: #999; padding: 6px;"><code>SPEDC500SEPA</code> (Gera bloco C100 e C500 ordenados do EFD para consolidados)</td><td style="border-color: #999; padding: 6px;">Ver <a href="#consolidacao">Configuração e Consolidação por Estabelecimentos</a>.</td></tr><tr><td style="border-color: #999; padding: 6px;"><code>GERREGORDEFD</code> (Gera registros ordenados no EFD consolidado)</td><td style="border-color: #999; padding: 6px;">Ver <a href="#consolidacao">Configuração e Consolidação por Estabelecimentos</a>.</td></tr><tr><td style="border-color: #999; padding: 6px;"><code>GERBLCDALIQFIL</code> (Gera bloco D101 e D105 com alíquotas das filiais no consolidado)</td><td style="border-color: #999; padding: 6px;">Ligado: usa as alíquotas da empresa de origem da movimentação na geração de D101/D105.</td></tr><tr><td style="border-color: #999; padding: 6px;"><code>GERAF100JMSPARC</code> (Gera F100 de Juros/Multa sem identificar Parceiro Padrão NFCe)</td><td style="border-color: #999; padding: 6px;">Ligado: o campo 03 (COD_PART) do F100 referente a juros/multas de NFCe é gerado em branco, e o registro 0150 do Parceiro Padrão da NFCe não é gerado (um Parceiro usual, se utilizado, continua sendo gerado normalmente).</td></tr><tr><td style="border-color: #999; padding: 6px;"><code>CONSCABLIVEFD</code> (Considera o valor da CAB no Livro e no EFD)</td><td style="border-color: #999; padding: 6px;">Ligue caso seja necessário ajustar os valores da CAB no Livro Fiscal e no EFD.</td></tr><tr><td style="border-color: #999; padding: 6px;"><code>EXCOMDEVRF525</code> (Excluir Compensações Devolução dos registros F500/F525)</td><td style="border-color: #999; padding: 6px;">Ligado: desconsidera compensações de devoluções nos registros F500 e F525.</td></tr></tbody></table>