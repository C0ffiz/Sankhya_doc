# Manual de Fluxo e Configurações do Pronta Entrega

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/7263209527703-Manual-de-Fluxo-e-Configura%C3%A7%C3%B5es-do-Pronta-Entrega](https://ajuda.sankhya.com.br/hc/pt-br/articles/7263209527703-Manual-de-Fluxo-e-Configura%C3%A7%C3%B5es-do-Pronta-Entrega)

---

# Manual de Fluxo e Configurações do Pronta Entrega

<table cellspacing="0,5" style="border-collapse: collapse; width: 100%; height: 58px;"><tbody><tr style="height: 58px;"><td class="wysiwyg-text-align-center" style="width: 100%; height: 58px;"><pre class="wysiwyg-text-align-justify"><span class="wysiwyg-font-size-medium"><strong><img alt="Módulo 36x36 FINAL.png" src="/hc/article_attachments/42312211475223"> Módulo: </strong>Comercial &gt; Relatórios       <strong>    <img alt="Versão - 32x32 FINAL.png" src="/hc/article_attachments/42312211476247"> Versão disponível: </strong>A partir da 4.11</span></pre></td></tr></tbody></table>

---

Pronta Entrega é uma rotina Sankhya, responsável por verificar as notas e cancelamentos pendentes provenientes dos aplicativos de mobilidade Landix, WMW e Máxima, realizando o seu devido processamento no ERP.

Independentemente do parceiro integrador, o fluxo de processo se mantém o mesmo:

<table style="border-collapse: collapse; width: 100%; height: 206px;"><tbody><tr style="height: 66px;"><td class="wysiwyg-text-align-center" style="width: 11.7143%; height: 66px;">&nbsp; &nbsp; &nbsp; &nbsp; <img alt="Marcador 1 FINAL.png" src="/hc/article_attachments/42312227999639"></td><td class="wysiwyg-text-align-justify" style="width: 88.2857%; height: 66px;"><p>O vendedor ao visitar o cliente, possui um smartphone com a solução da mobilidade instalada, possibilitando o lançamento de uma NF-e diretamente no banco de dados da <span class="wysiwyg-underline">Sankhya</span>;</p></td></tr><tr style="height: 96px;"><td class="wysiwyg-text-align-center" style="width: 11.7143%; height: 96px;">&nbsp; &nbsp; &nbsp; &nbsp;<img alt="Marcador 1 FINAL.png" src="/hc/article_attachments/42312227999639"></td><td class="wysiwyg-text-align-justify" style="width: 88.2857%; height: 96px;"><p>O <span class="wysiwyg-underline">Agendador Sankhya</span> (Pronta Entrega), varre o banco de tempos em tempos verificando se há novos registros que necessitam processamento. Caso exista, ele realiza o processamento deste registro e envia a NF-e para a SEFAZ a fim de buscar a sua aprovação;</p></td></tr><tr style="height: 44px;"><td class="wysiwyg-text-align-center" style="width: 11.7143%; height: 44px;">&nbsp; &nbsp; &nbsp; &nbsp;<img alt="Marcador 1 FINAL.png" src="/hc/article_attachments/42312227999639"></td><td class="wysiwyg-text-align-justify" style="width: 88.2857%; height: 44px;"><p>Após o retorno da SEFAZ, o agendador atualiza o status da nota no banco da Sankhya, possibilitando a mobilidade de pesquisar o seu resultado.</p></td></tr></tbody></table>

Além desse fluxo padrão, vale destacar que o processo também pode se deparar com o envio normal da NF-e ou com a necessidade de se trabalhar em contingência, ou seja, caso a NF-e tenha sido aprovada, a mobilidade automaticamente realiza a geração do DANFE a partir do XML da nota. 

Se a NF-e não tiver sido aprovada, a mobilidade automaticamente gera um novo registro em contingência, que no caso da Pronta Entrega é o FS-DA e o insere no banco da Sankhya. O agendador identifica o registro e busca a sua aprovação junto à SEFAZ.

Portanto, a diferença na Pronta Entrega na emissão da NF-e e da Contingência é que na contingência o vendedor não necessita esperar a SEFAZ aprovar a nota para realizar a impressão do Danfe, diferentemente da NF-e que só pode ser impressa após a sua aprovação. Abaixo um detalhamento especificado de todo o processo:

---

#### ![mceclip16.png](https://ajuda.sankhya.com.br/hc/article_attachments/42312211478679)

<table style="border-collapse: collapse; width: 100%; height: 872px;"><tbody><tr style="height: 44px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 44px;"><img alt="1 FINAL.png" src="/hc/article_attachments/42312228001431"></td><td style="width: 92%; height: 44px;"><p class="wysiwyg-text-align-justify">O <span class="wysiwyg-underline">PDA</span> (Assistente Pessoal Digital (Palm, Pocket)) descarrega a negociação e junto envia uma solicitação de autorização de NF-e;</p></td></tr><tr style="height: 44px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 44px;"><img alt="2 FINAL.png" src="/hc/article_attachments/42312228003351"></td><td style="width: 92%; height: 44px;"><p class="wysiwyg-text-align-justify">A descarga é feita através da internet e é recebida pelo <span class="wysiwyg-underline">LMMS</span> (Landix Mobile Middleware Server);</p></td></tr><tr style="height: 44px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 44px;"><img alt="3 FINAL.png" src="/hc/article_attachments/42312211483927"></td><td style="width: 92%; height: 44px;"><p class="wysiwyg-text-align-justify">O <span class="wysiwyg-underline">LMMS</span> aciona o <span class="wysiwyg-underline">Middleware</span> para processar a negociação e a solicitação de autorização de NF-e;</p></td></tr><tr style="height: 67px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 67px;"><img alt="4 FINAL.png" src="/hc/article_attachments/42312228006807"></td><td style="width: 92%; height: 67px;"><p class="wysiwyg-text-align-justify">O&nbsp;<span class="wysiwyg-underline">Middleware</span>&nbsp;grava a negociação com o estado&nbsp;<strong>"confirmada"</strong>&nbsp;nas tabelas do&nbsp;<span class="wysiwyg-underline">Sankhya Om</span>&nbsp;e grava um registro na tabela de integração para enfileirar as solicitações de autorização de NF-e;</p></td></tr><tr style="height: 36px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 36px;"><img alt="5 FINAL.png" src="/hc/article_attachments/42312211487383"></td><td style="width: 92%; height: 36px;"><p class="wysiwyg-text-align-justify">O&nbsp;<span class="wysiwyg-underline">Sankhya Om</span>&nbsp;indica para o&nbsp;<span class="wysiwyg-underline">Middleware</span>&nbsp;o NUNOTA referente à negociação gravada;</p></td></tr><tr style="height: 44px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 44px;"><img alt="6 FINAL.png" src="/hc/article_attachments/42312211488791"></td><td style="width: 92%; height: 44px;"><p class="wysiwyg-text-align-justify">O&nbsp;<span class="wysiwyg-underline">Middleware</span>&nbsp;devolve ao <span class="wysiwyg-underline">LMMS</span> o NUNOTA referente à negociação gravada no Sankhya/W;</p></td></tr><tr style="height: 36px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 36px;"><img alt="7 FINAL.png" src="/hc/article_attachments/42312211489687"></td><td style="width: 92%; height: 36px;"><p class="wysiwyg-text-align-justify">O&nbsp;<span class="wysiwyg-underline">LMMS</span>&nbsp;envia através da internet o NUNOTA referente à negociação descarregada;</p></td></tr><tr style="height: 44px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 44px;"><img alt="8 FINAL.png" src="/hc/article_attachments/42312211491095"></td><td style="width: 92%; height: 44px;"><p class="wysiwyg-text-align-justify">O&nbsp;<span class="wysiwyg-underline">PDA</span>&nbsp;recebe NUNOTA para futuramente verificar se a NF-e foi autorizada e assim concretizar a venda;</p></td></tr><tr style="height: 67px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 67px;"><img alt="9 FINAL.png" src="/hc/article_attachments/42312228015511"></td><td style="width: 92%; height: 67px;"><p class="wysiwyg-text-align-justify">De tempo em tempo um agendador NFe <span class="wysiwyg-underline">Pronta Entrega</span> se comunica com o web service da SEFAZ, verifica na tabela de integração se há solicitações de NF-e e monta um pacote com todas as solicitações de NF-e, que ainda não foram enviadas à SEFAZ;</p></td></tr><tr style="height: 44px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 44px;"><img alt="10 FINAL.png" src="/hc/article_attachments/42312228017175"></td><td style="width: 92%; height: 44px;"><p class="wysiwyg-text-align-justify">O agendador envia através da internet o pacote com as notas que necessitam de autorização da SEFAZ;</p></td></tr><tr style="height: 36px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 36px;"><img alt="11 FINAL.png" src="/hc/article_attachments/42312211495831"></td><td style="width: 92%; height: 36px;"><p class="wysiwyg-text-align-justify">A SEFAZ recebe as solicitações de autorização de NF-e;</p></td></tr><tr style="height: 36px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 36px;"><img alt="12 FINAL.png" src="/hc/article_attachments/42312228018583"></td><td style="width: 92%; height: 36px;"><p class="wysiwyg-text-align-justify">A SEFAZ devolve o protocolo de recebimento de solicitação;</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="13 FINAL.png" src="/hc/article_attachments/42312211497623"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">O agendador recebe o protocolo de recebimento da SEFAZ;</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="14 FINAL.png" src="/hc/article_attachments/42312228019991"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">O agendador grava no banco de dados do&nbsp;<span class="wysiwyg-underline">Sankhya Om</span>, o protocolo de recebimento das solicitações que foram recebidas;</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="15 FINAL.png" src="/hc/article_attachments/42312211499031"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">De tempo em tempo o agendador verifica no banco de dados, e monta um pacote com as solicitações que já foram enviadas para a SEFAZ e estão aguardando a resposta sobre a autorização;</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="16 FINAL.png" src="/hc/article_attachments/42312211500567"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">O agendador envia o pacote à SEFAZ para verificar se as notas foram autorizadas;</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="17 FINAL.png" src="/hc/article_attachments/42312228027159"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">A SEFAZ recebe o pacote e verifica se as solicitações de NF-e indicadas no pacote foram autorizadas;</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="18 FINAL.png" src="/hc/article_attachments/42312228029079"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">A SEFAZ monta um pacote indicando as solicitações de NF-e que foram aprovadas e indicando o código de autorização de cada NF-e;</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="19 FINAL.png" src="/hc/article_attachments/42312211503127"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">O agendador recebe o pacote com as solicitações autorizadas e os códigos de autorização da NF-e;</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="20 FINAL.png" src="/hc/article_attachments/42312228030487"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">O agendador grava no banco de dados do&nbsp;<span class="wysiwyg-underline">Sankhya Om</span>, a marcação das notas que foram autorizadas e os códigos das NF-e autorizadas;</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="21 FINAL.png" src="/hc/article_attachments/42312228030999"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">O&nbsp;<span class="wysiwyg-underline">PDA</span>&nbsp;descarrega as notas que estão aguardando autorização da SEFAZ e junto envia a solicitação de verificação de NF-e aprovada;</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="22 FINAL.png" src="/hc/article_attachments/42312228032023"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">A descarga é feita através da internet e é recebida pelo&nbsp;<span class="wysiwyg-underline">LMMS</span>&nbsp;(Landix Mobile Middleware Server);</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="23 FINAL.png" src="/hc/article_attachments/42312211507351"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">O&nbsp;<span class="wysiwyg-underline">LMMS</span>&nbsp;aciona o&nbsp;<span class="wysiwyg-underline">Middleware</span>&nbsp;para verificar se as notas descarregadas foram autorizadas;</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="24 FINAL.png" src="/hc/article_attachments/42312228033559"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">O&nbsp;<span class="wysiwyg-underline">Middleware</span>&nbsp;conecta ao banco de dados do&nbsp;<span class="wysiwyg-underline">Sankhya Om</span>&nbsp;e verifica quais notas já foram autorizadas pela SEFAZ</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="25 FINAL.png" src="/hc/article_attachments/42312211508887"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">O&nbsp;<span class="wysiwyg-underline">Middleware</span>&nbsp;copiá do banco do&nbsp;<span class="wysiwyg-underline">Sankhya Om</span>&nbsp;os XML das notas que foram autorizadas;</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="26 FINAL.png" src="/hc/article_attachments/42312211509015"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">O&nbsp;<span class="wysiwyg-underline">Middleware</span>&nbsp;monta um envelope onde são armazenados todos os XML&nbsp;copiados do banco do&nbsp;<span class="wysiwyg-underline">Sankhya Om</span>&nbsp;e disponibiliza o envelope para o&nbsp;<span class="wysiwyg-underline">LMMS</span>;</p></td></tr><tr style="height: 22px;"><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top; height: 22px;"><img alt="27 FINAL.png" src="/hc/article_attachments/42312211509911"></td><td style="width: 92%; height: 22px;"><p class="wysiwyg-text-align-justify">O&nbsp;<span class="wysiwyg-underline">LMMS</span>&nbsp;envia através da internet, o envelope com as XML das NF-e;</p></td></tr><tr><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: middle;"><img alt="28 FINAL.png" src="/hc/article_attachments/42312228041495"></td><td style="width: 92%;"><p class="wysiwyg-text-align-justify">O&nbsp;<span class="wysiwyg-underline">PDA</span>&nbsp;recebe o envelope, identifica através dos XML&nbsp;as notas que foram autorizadas;</p></td></tr><tr><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top;"><img alt="29 FINAL.png" src="/hc/article_attachments/42312211512599"></td><td style="width: 92%;"><p class="wysiwyg-text-align-justify">O&nbsp;<span class="wysiwyg-underline">PDA</span>&nbsp;interpreta o XML, monta o arquivo de DANFE simplificado&nbsp;e envia para a impressora;</p></td></tr><tr><td class="wysiwyg-text-align-center" style="width: 8%; vertical-align: top;"><img alt="30 FINAL.png" src="/hc/article_attachments/42312228042903"></td><td style="width: 92%;"><p class="wysiwyg-text-align-justify">A impressora imprime o DANFE simplificado.</p></td></tr></tbody></table>

---

#### **Requisitos** 

Para realizar as configurações da rotina Pronta Entrega, para o aplicativo da **"Máxima"** acesse o artigo [Integração Máxima Sankhya](https://ajuda.sankhya.com.br/hc/pt-br/articles/7893973086743).

Caso utilize aplicativos Landix e WMW, siga as instruções abaixo:

*   É necessário que o cliente tenha o produto Pronta Entrega em sua licença de uso, para ativá-lo no Sankhya Om;
*   **Usa Pronta Entrega NFe W? - USAPRONTENTW:** deve estar ligado;
*   **Int. de exec. Job Util. Pronta Entrega (min)-INTUTILPRONTENT:** deve possuir um valor preenchido. Recomendamos o padrão 15 minutos;
*   **Int. de exec. Job de Canc. Pronta Entrega (min)-INTCANCPRONTENT:** deve apresentar um valor preenchido. Recomendamos o padrão 30 minutos;
*   **Qtd. Notas Cancelamento Pronta Entrega NFe W-QNOTACPRONTENTW:** deve apresentar um valor preenchido. Recomendamos o padrão 10;
*   **Qtd. Notas Processamento Pronta Entrega NFe W-QNOTASPRONTENTW:** estar com um valor preenchido. Recomendamos o padrão, 50**;**
*   **TOP's excluídas do processamento pronta entrega-TOPSEXCPRONTENT:** neste parâmetro o implantador deve configurar os códigos das TOP's que não necessitam de processamento pelo Pronta Entrega.
*   **Gera Log Pronta Entrega NFe W?-LOGPRONTENTW:** orientamos que este parâmetro seja mantido ligado.

Após realizar as configurações acima, será disponibilizada a tela **"Painel Pronta Entrega"**, no Sankhya Om.

![Imagem1.png](https://ajuda.sankhya.com.br/hc/article_attachments/7318238122903)

[\[voltar ao topo\]](#top)

#### **Processos realizados pela agendador**

*   Aprovação de Notas Normal;
*   Aprovação de Notas Contingência;
*   Geração com erro de Correção;
*   Cancelamento Nota Aprovada;
*   Cancelamento Nota Não Aprovada - Inutiliza;
*   Cancelamento Nota Não Aprovada Nota Aguardando Correção - Inutiliza;
*   Cancelamento Nota Não Aprovada Nota Aguardando Validação - Inutiliza.

[\[voltar ao topo\]](#top)

### Configurações

Clique nos links a seguir para verificar as configurações necessárias em cada tela:

[Tipos de Operação-Top](#TiposdeOpera%C3%A7%C3%A3o-Top)                                                          [Tipos de Negociação](#TiposdeNegocia%C3%A7%C3%A3o)

[Contas](#Contas)

---

#### **Tipos de Operação-Top**

Sugerimos que o cadastro de [Tipos de operação-TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114) específicos para as movimentações de Pronta Entrega:

*   Remessa para venda fora do estabelecimento;
*   Venda fora do estabelecimento;
*   Retorno de mercadorias enviadas para venda fora do estabelecimento.

Dentre estas operações, a rotina do Pronta Entrega é responsável pelo envio e confirmação das movimentações de venda fora do estabelecimento, cujos detalhes serão apresentados a seguir:

**Aba Geral**

Nesta aba, configure o campo **"Financeiro"** com a opção **"Não atualizar"**. Além disso, mantenha a marcação **"Sempre exigir liberação"** desligada. 

![aba\_geral.gif](https://ajuda.sankhya.com.br/hc/article_attachments/7318773383959)

**Aba Impressão**

Selecione no campo **"Imprimir Pix/Boleto/Duplicata"** a opção **"Na confirmação".** 

![Imagens\_ksnip\_161\_.png](https://ajuda.sankhya.com.br/hc/article_attachments/7318783531671)

Para as empresas que emitem Nota Fiscal Eletrônica todas as TOP’s envolvidas no processo (Venda, Bonificação, Brinde e Devolução) deverão estar configuradas como:

**Aba NF-e/NFC-e/CF-e**

Informe no campo **"Tipo de Emissão"** a opção **"Normal"**. Além disso, no campo **"Modelo de documento"** selecione a opção **"55 - Nota Fiscal Eletrônica"**.

![aba\_NFe.gif](https://ajuda.sankhya.com.br/hc/article_attachments/7319142433175)

**Aba Impressão**

Os campos **"Imprimir"** e **"Imprimir Boleto/Duplicata"** devem ser configurados com a opção **"Manual"**.

![Imagens\_ksnip\_162\_.png](https://ajuda.sankhya.com.br/hc/article_attachments/7319263522967)

[\[voltar ao subtítulo\]](#Configura%C3%A7%C3%B5es) 

---

#### **Tipos de** **Negociação**

**Aba Características**

Configure o campo **"Subtipo"** com a opção **"A prazo"**, e selecione no campo **"Imprimir Pix/Boleto/Duplicata?"** a opção **"Na confirmação"**. 

![Imagens\_ksnip\_164\_.png](https://ajuda.sankhya.com.br/hc/article_attachments/7319452338071)

**Aba Parcelas**

Informe o campo **"Tipo de Empresa"** com a opção **"X - Constante Exclusiva"**.

![Imagens\_ksnip\_166\_.png](https://ajuda.sankhya.com.br/hc/article_attachments/7319567195799)

[\[voltar ao subtítulo\]](#Configura%C3%A7%C3%B5es) 

#### **Contas**

**Aba Boletos/Duplicatas**

Acione a marcação **"Emite"**. Busque no campo **"Modelo"** o modelo de boleto cadastrado. 

![Imagens\_ksnip\_167\_.png](https://ajuda.sankhya.com.br/hc/article_attachments/7320622103447)

**Observação:** O arquivo **"Modelo de Boleto"** deverá possuir uma marcação para realizar a impressão automaticamente. Caso não exista essa marcação, o sistema não realizará a impressão continua.

[\[voltar ao subtítulo\]](#Configura%C3%A7%C3%B5es) [\[voltar ao topo\]](#top)

---

#### **Configuração de Envio de DANFE por E-mail**

Para configurar o envio do Danfe por e-mail é necessário:

*   Habilitar o parâmetro **"Usa NF-e do SankhyaW-USANFESANKHYAW"**;
*   Configurar o parâmetro **"Remetente para pedidos- EMAILPED"** com a opção **"Empresa"**.
*   E caso tenha o parâmetro **"EMAILSENHA"**, é necessário configurar a senha do e-mail utilizado.

Feito isso, na tela [Parceiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494), nas abas **"NF-e/NFS-e/CT-e"** e **"Endereço"** cadastre um endereço de e-mail. Depois, na tela [Usuários](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044597874), por meio da aba **"SMTP"**, configure a conexão SMTP.

Em seguida, acesse a tela [Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112913-Cadastro-de-Empresas), aba [Endereço](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112913-Cadastro-de-Empresas#abaendereo) e registre um endereço de **"E-mail"**. 

[\[voltar ao topo\]](#top)

#### **Configuração de Vendedores e Regiões**

Recomendamos que seja criada uma empresa para cada vendedor que irá realizar vendas através dos aplicativos de mobilidade, para que o estoque seja controlado por empresa. Essa empresa pode conter os mesmos dados da matriz, porém a sua Descrição e Código poderá ter o Nome e o Código do Vendedor para facilitar a identificação do vendedor no momento da geração das notas.

Além disso, a tela [Regiões](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044599074) poderá ser configurada e parametrizada para a formação de sequência de visita e definição de áreas de atuação de cada vendedor.

[\[voltar ao topo\]](#top)

#### **Operação de Venda Externa x Pronta Entrega**

Após realizar as parametrizações acima, o fluxo a ser seguido para as operações de venda externa através de aplicativos de mobilidade, são descritas abaixo:

**1- Remessa de  estoque para o vendedor:**

**1.1** - Como o estoque é controlado por empresas, e cada vendedor é uma empresa, então para abastecermos o veículo do vendedor, é necessário realizar uma nota de transferência entre empresas, através do [Portal de Movimentações Internas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045109593);

**1.2** - O vendedor estará abastecido, caso necessário ele pode solicitar uma nova remessa para reposição de  itens;

**1.3** - A necessidade de reabastecimento de estoque do vendedor poderá ser solicitada através da rotina de Pedidos Web no ERP, onde será gerado um pedido que poderá ser reaproveitado para realizar a nova remessa;

**2-  Venda realizada através do app de mobilidade:**

**2.1** - O Estoque será  baixado na medida que as vendas ocorrerem durante o dia, com a sincronização de pedidos através do Pronta Entrega;

**2.2** - Quando o vendedor realiza a venda, na  nota gerada poderá ser informada a qual remessa pertenceu o estoque, para facilitar a identificação de qual remessa pertenceu o estoque da venda realizada (A identificação pode ser feita através de observação ou um campo adicional);

**2.3** \- Os impostos serão calculados pelo ERP;

**2.4** \- Boleto e XML serão enviados através do ERP;

**2.5** \- Financeiro será baixado através da [Movimentação Financeira](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114753).

**3 - Retorno da Remessa:**

**3.1** - O retorno da remessa, poderá ser feito diariamente de forma simbólica caso o vendedor e a empresa prefira;

**3.2** \- No retorno é feita a conferência e é gerada uma nova transferência entre empresas no [Portal de Movimentações Internas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045109593), para a geração de uma nova remessa no outro dia.

[\[voltar ao topo\]](#top)

#### **Detalhes da Tabela TGFPEL**

O campo **"STATUSNFE"** corresponde à situação da nota para processamento. Ele é preenchido quando o STATUS estiver diferente de 4 apenas quando é uma solicitação de cancelamento (TGFPEL.STATUSNFE = 'C'):

*   **A:** significa que a nota está autorizada.
*   **C:** significa que a nota deverá ser Cancelada.
*   **D:** significa que a nota foi Denegada.
*   **E:** significa que o Prazo regulamentar para o Cancelamento da NF-e está expirado.
*   **F:** significa erro pois a SEFAZ fora do ar.
*   **N:** Significa que a nota não será enviada à SEFAZ.

O campo **"STATUS"** se refere ao detalhamento do que já foi processado na nota. Nele é aceito os valores:

*   **\-1:** trata-se da inserção do registro na tabela TGFPEL. Indica que o registro precisa ser processado;
*   **0:** corresponde ao início do processamento do processador NFE. À partir deste momento, apenas a Sankhya pode manipular o registro;
*   **1:** refere-se ao início dos cálculos de PIS/COFINS efetuados pelo agendador;
*   **2:** corresponde aos cálculos de PIS/COFINS realizados com sucesso, a montagem da CHAVENFE e o envio da nota à SEFAZ;
*   **3:** trata-se à pesquisa do resultado do envio da nota à SEFAZ, isto é, se a nota foi aprovada, cancelada, rejeitada ou denegada;
*   **4:** refere-se ao resultado da consulta obtido com sucesso ou o fim do processamento devido à alguma adversidade.

[\[voltar ao topo\]](#top)

#### **Parâmetros que influenciam nessa rotina**

**Pront. Ent. WMW recalcula fianceiro e icms? - PRONTENTWMWRFI:** quando estiver ligado, irá refazer o ICMS do item e recalculará o financeiro da nota e, quando estiver desligado e o cliente for WMW, não será refeito o ICMS do item e nem recalculado o financeiro da nota.

**Aprova antes de cancelar Pronta Entrega NFe W - APRPCANPRENTSKW:** quando ligado, caso a nota já esteja numerada, será primeiramente realizada a aprovação desta nota e logo em seguida, o seu cancelamento. Se desligado, a nota que já estiver numerada, mas antes de sua aprovação for solicitado seu cancelamento, o sistema irá fazer uma requisição de inutilização da numeração e só depois excluir a nota.

[\[voltar ao topo\]](#top)

Relativo a

*   [APRPCANPRENTSKW](https://ajuda.sankhya.com.br/hc/pt-br/search?content_tags=01H7Z6YW8YPPCGA5GP8WRA67XC&utf8=%E2%9C%93 "Resultados da pesquisa")
*   [PRONTENTWMWRFI](https://ajuda.sankhya.com.br/hc/pt-br/search?content_tags=01H7Z6Z1R56Y3NH0VQ5BP5RXXK&utf8=%E2%9C%93 "Resultados da pesquisa")