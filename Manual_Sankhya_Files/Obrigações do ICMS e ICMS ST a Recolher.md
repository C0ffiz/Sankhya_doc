# Obrigações do ICMS e ICMS ST a Recolher

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116133-Obriga%C3%A7%C3%B5es-do-ICMS-e-ICMS-ST-a-Recolher](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116133-Obriga%C3%A7%C3%B5es-do-ICMS-e-ICMS-ST-a-Recolher)

---

# Obrigações do ICMS e ICMS ST a Recolher

![Módulo 36x36 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313061307543) **Módulo:** Livros Fiscais > Avançado > Escrituração Fiscal Digital

---

Nesta tela, informe os dados referentes às obrigações a recolher, obrigações estas, referentes a ICMS ou ICMS ST. De acordo com o imposto que está sendo recolhido, teremos o seguinte comportamento:

*   Se o **"Tipo Apuração"** for igual a **"ICMS"**: Discrimina os pagamentos realizados ou a realizar, referentes à apuração do ICMS – Operações Próprias do Período. A soma do valor das obrigações deste registro deve ser igual à soma dos campos VL\_ICMS\_RECOLHER e DEB\_ESP, do Registro E110.
*   Se o **"Tipo Apuração"** for igual a **"ICMS ST"**: Discrimina os pagamentos realizados ou a realizar, referentes à apuração do ICMS devido por Substituição Tributária do Período, por UF. A soma do valor das obrigações deste registro deve ser igual ao campo VL\_ICMS\_RECOL\_ST somado ao campo DEB\_ESP\_ST, ambos do Registro E210.
*   Tipo o **"Tipo Apuração"** for igual a **"ICMS ST FCP"**:  Essa opção indicará que o ICMS-ST será somado ao ICMS FCP.

Os dados aqui informados, irão alimentar o Registro E116 do EFD se Tipo Apuração igual a ICMS ou para o Registro E250 do EFD se Tipo Apuração igual a ICMS ST.

**Nota:** esta rotina considera o período de geração do arquivo SPED Fiscal da tela [EFD - Escrituração Fiscal Digital - ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607614), ou seja, o valor informado no campo **"Período"** desta tela, será utilizado para buscar todos os registros de lançamento na tela Obrigações do ICMS e ICMS ST a Recolher. Assim, caso o sistema encontre lançamentos nesta que corresponda ao intervalo de dias informado na geração do SPED ICMS/IPI, será capturado os dados e informado os mesmos no Registro E116 do SPED Fiscal ICMS/IPI.

O sistema conta com um recurso que permite a alimentação automática da tela Obrigações do ICMS e ICMS ST a Recolher por meio dos procedimentos realizados na tela **"Geração de Lote GNRE"**. Para maiores detalhes sobre este processo, acesse o link [Geração Automática - Obrigações do ICMS e ICMS ST a Recolher](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045109513).

![obriga\_oes.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/4403007159447)

Informe no campo **"Empresa"**, a empresa a qual está sendo lançada a obrigação de recolhimento.

Preencha no campo **"Referência"** qualquer data de preferência para seu controle, como por exemplo, a data de referência do imposto.

Defina no campo **"Tipo Apuração"** qual o imposto que se está lançando o recolhimento; temos para escolha as opções:

*   ICMS;
*   ICMS ST;
*   ICMS DIFAL; 
*   ICMS FCP.

**Nota:** se o campo **"Tipo Apuração"** da aba [GNRE Unidade Federativa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601294-Estados#abagnreunidadefederativa) tela [Estados](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601294-Estados), estiver preenchido, o campo acima será configurado com a mesma opção.

No campo **"Desc. Processo"** informe neste campo o descritivo dos dados pertinentes à obrigação a recolher.

Defina no campo **"UF"**, o estado ao qual a empresa do recolhimento pertence.

O campo **"Código"** possui para escolha as opções referentes ao tipo de recolhimento que está sendo lançado. São elas:

*   Antecipação do diferencial de alíquotas do ICMS;
*   ICMS da substituição tributária pelas entradas;
*   ICMS resultante da alíquota adicional dos itens incluídos no Fundo de Combate a Pobreza;
*   Antecipação do ICMS da importação;
*   ICMS normal a recolher;
*   Outras obrigações do ICMS;
*   Antecipação tributária;
*   ICMS da substituição tributária pelas saídas para o Estado; 
*   ICMS da substituição tributária pelas saídas para outro Estado.

**Nota:** se o campo **"Código"** da aba [GNRE Unidade Federativa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601294-Estados#abagnreunidadefederativa) tela [Estados](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601294-Estados), estiver preenchido, o campo acima será configurado com a mesma opção.

No campo **"Código da Receita (DIME)"**, informe o código da receita DIME conforme Portaria 164 de 14/07/2004.

Em **"Código Classe Vencimento (DIME)"** insira a classe de vencimentos conforme Portaria 269 de até 20 caracteres.

Informe no campo **"Valor"**, o valor da obrigação a recolher.

No campo **"Data Vencimento"** preencha a data de vencimento da obrigação de recolhimento que está sendo lançada.

O campo **"Código Receita"** é preenchido de acordo com a Tabela de Códigos de Receita, definida pelas Secretarias de Fazenda dos Estados ou do Distrito Federal.

Informe no campo **"Nro. Processo"**, o número do processo ou auto de infração ao qual a obrigação está vinculada, se houver.

**Nota:** na geração dos registros do bloco E, bloco C, 1922 e 1926, este campo se comporta da seguinte maneira:

*   Arquivos gerados até o exercício 2022, o campo permite até 15 caracteres;
*   Arquivos gerados a partir do exercício 2023 poderão ter até 60 caracteres.

O campo **"Indicador"** possui como escolha os órgãos responsáveis pela origem do processo. E poderão ser:

*   Sefaz;
*   Justiça Federal;
*   Outro;
*   Justiça Estadual.

No campo **"Desc. Complementar"** informe o descritivo dos dados complementares pertinentes a obrigação à recolher.

Indique no campo **"Indicador de Sub-Apuração"** se a obrigação pertence ou não à uma sub-apuração.

Os campos Empresa, Referência e Tipo Apuração são chamados campos chave desta tela e, portanto, uma vez informados e confirmados, não poderão mais serem alterados. Caso alguma tentativa de alteração seja feita, é apresentada a mensagem abaixo:

_**"Não é possível alterar o valor de um campo chave do registro."**_

Na geração do GNRE, o sistema seguirá uma hierarquia para os financeiros nas Obrigações do ICMS e ICMS ST a Recolher, uma vez que estas ocorrerão por meio dos campos **"Código da Receita (DIME)"** e **"Código Classe de Vencimento (DIME)"**. Portanto, teremos:

**1.** Se os campos **"Código da Receita (DIME)"** e **"Código Classe de Vencimento (DIME)"** localizados na aba Geral do Cadastro de Estados estiverem preenchidos, o sistema utilizará as informações destes campos no financeiro;  
**2.** Porém, se os campos acima não possuírem dados, o sistema os buscará nos campos **"Código da Receita (DIME) p/ FCT ST"** e **"Código Classe Vencimento (DIME) p/ FCP ST"** na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601294-Estados#abageral) no [Cadastro de Estados](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601294-Estados);  
**3.** Porém, se os campos da aba Geral da tela informada acima não forem preenchidos, o sistema buscará os valores necessários nos campos Código da Receita (DIME) e Código Classe Vencimento (DIME) dessa tela.

[\[Voltar ao topo\]](#top)