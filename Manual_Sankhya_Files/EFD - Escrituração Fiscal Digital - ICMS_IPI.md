# EFD - Escrituração Fiscal Digital - ICMS/IPI

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607614-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607614-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI)

---

# EFD - Escrituração Fiscal Digital - ICMS/IPI

```auto
 Módulo: Livros Fiscais > Conexão            
```

---

A Escrituração Fiscal Digital - EFD é um arquivo digital, que se constitui de um conjunto de escriturações de documentos fiscais e de outras informações de interesse do fisco das Unidades Federadas e da Secretaria da Receita Federal do Brasil (RFB), bem como de registros de apuração de impostos referentes às operações e prestações praticadas pelo contribuinte.

<table style="margin-left: 0px; margin-right: auto;"><tbody><tr style="height: 23.8px;"><td style="height: 23px; width: 292.145px;"><a class="topiclink" href="#abaparmetros"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Aba Parâmetros</span></a><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;</span></td><td style="height: 23px; width: 10px;">&nbsp;</td><td style="height: 23px; width: 336.207px;"><a class="topiclink" href="#abaopes"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Aba Opções</span></a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 292.145px;"><a class="topiclink" href="#abarestitui%C3%A7%C3%A3o/complementa%C3%A7%C3%A3odeST"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Aba Restituição/Complementação de ST</span></a></td><td style="height: 22px; width: 10px;">&nbsp;</td><td style="height: 22px; width: 336.207px;"><a class="topiclink" href="#abaprodepe"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Aba Prodepe</span></a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 292.145px;"><a class="topiclink" href="#abasub-apuraoefd"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Aba Sub-Apuração EFD</span></a></td><td style="height: 22px; width: 10px;">&nbsp;</td><td style="height: 22px; width: 336.207px;"><a class="topiclink" href="#h_b208ab70-83d6-4499-813e-b043dc3f3f31" target="_self"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Aba Arquivos para Registro D695</span></a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 292.145px;"><a class="topiclink" href="#h_5bf78af1-86fd-4ca7-b0fd-db21f1358ff5" target="_self"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Aba Botões da tela</span></a></td><td style="height: 22px; width: 10px;">&nbsp;</td><td style="height: 22px; width: 336.207px;"><a class="topiclink" href="#geraodosregistros0450c110ec113"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Geração dos registros 0450, C110 e C113</span></a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 292.145px;"><a class="topiclink" href="#geraodoregistro1400"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Geração do registro 1400</span></a></td><td style="height: 22px; width: 10px;">&nbsp;</td><td style="height: 22px; width: 336.207px;"><a class="topiclink" href="#geraodacontacontbilparaoregistroh010"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Geração da Conta Contábil...</span></a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 292.145px;"><a class="topiclink" href="#registrosdoblocok"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Registros do Bloco K</span></a></td><td style="height: 22px; width: 10px;">&nbsp;</td><td style="height: 22px; width: 336.207px;"><a href="#registro0300eg125" target="_self"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Registro 0300 e G125</span></a></td></tr><tr><td><a href="#h_01KJG74H2C5GCWMWCJYZC2JPG6">Geração Consolidada da NFCom (Registros D750, D760 e D761)</a></td><td>&nbsp;</td><td>&nbsp;</td></tr></tbody></table>

![efd-aba-parametros.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/14300239485591)

A primeira informação a ser preenchida, é a **"Empresa"** da qual serão gerados os dados para escrituração. Ao manter o campo Empresa em branco, temos a possibilidade de previamente à geração dos dados, selecionar várias ou todas as empresas configuradas para gerar EFD - Escrituração Fiscal Digital.

Em seguida, defina a **"UF"** a ser considerada para geração do arquivo.

Em seguida, determine o **"Período****"** que irá abranger a geração do relatório; este período é informado quando uma Data Inicial e Final for definido para geração dos dados.

Aba Parâmetros

Nesta aba, são definidas as parametrizações necessárias para geração do arquivo EFD. Vejamos os dados a serem configurados:

Em **"Finalidade de Apresentação do Arquivo"**, será definido o objetivo da geração do arquivo. Nesta, você terá duas alternativas:

*   Remessa do arquivo original;
    
*   Remessa do arquivo substituto.
    

O campo **"Versão do Layout do Arquivo"** será apresentado com impossibilidade de edição e exibirá a versão do layout do arquivo que está sendo utilizada para geração da escrituração. As versões são utilizadas de acordo com o período inicialmente informado, sendo assim, teremos: 

![tabela\_vers\_o\_leiauti.png](https://ajuda.sankhya.com.br/hc/article_attachments/10892609031959)

Informe no campo **"Data do inventário"**, que o sistema irá considerar para a geração da escrituração.

O campo **"Data de Inventario em substituição ao Bloco K"** é destinado para geração do H005 na posição mensal em substituição ao Bloco K e será exibido quando o parâmetro **"Gerar Bloco H em substituição ao Bloco K - GERBLHSUBSK"** estiver ligado. Ao informar uma data nesse campo será gerado no arquivo do EFD, um Bloco H correspondente à cópia de estoque registrada na data informada em substituição ao Bloco K. E, sempre que houver um Bloco H para a data informada, o sistema deixará de gerar o Bloco K correspondente às informações provenientes desta cópia de estoque.

No campo **"Data da contagem p/ K200"**, você poderá inserir a data da contagem para a geração do registro na tela Dashboard auxiliar do BLOCO K após a execução da cópia e contagem de estoque no processo de inventário. Porém, para que o campo seja exibido, é preciso ligar o parâmetro **"GERARK200CTE"**, de forma que, com este desligado, será considerado o estoque que consta no último dia da geração do SPED Fiscal da referência em questão.

**Observação:** com os parâmetros Gerar Bloco H em substituição ao Bloco K - GERBLHSUBSK e GERAK200CTE habilitados, tem-se:

Que os campos Data de contagem p/ K200 e Data de Inventario em substituição ao Bloco K serão exibidos e, ao preenchê-los simultaneamente e processar o EFD, o sistema exibirá a seguinte mensagem:

_**"O campo “Data de contagem p/ K200” não pode estar preenchido se o campo “Data de Inventario em substituição ao Bloco K” também estiver preenchido. Defina qual data será utilizada para a geração do arquivo."**_

Porém, com o campo Data de contagem p/ K200 configurado e o Data de Inventario em substituição ao Bloco K vazio, o sistema realizará a geração do Bloco K na tela [Dashboard auxiliar do Bloco K](https://ajuda.sankhya.com.br/hc/pt-br/articles/4411588603159--Dashboard-auxiliar-do-BLOCO-K) após a execução da cópia e contagem de estoque no processo de inventário;

Ao preencher o campo Data de Inventario em substituição ao Bloco K e o campo Data de contagem p/ K200 ficar vazio, ao realizar o processamento do EFD, o sistema irá executar a geração do Bloco H de forma que irá substituir o Bloco K;

Por fim, com ambos os campos vazios, quando o processamento do EFD for realizado, o sistema exibirá a seguinte mensagem:

_**"O parâmetro GERAK200CTE está ligado, então a "Data da Contagem p/ K200" deve ser informada."**_

No campo **"Perfil EFD"** será apresentado o perfil no qual o arquivo será gerado.

Caso seja necessário, informe o **"Nro. Único Nota"** de modo que, o sistema irá gerar as informações da nota em questão.

**Observação:** desde 01/01/2019 não é mais aceito os seguintes modelos de documentos relacionados à conhecimentos de transporte:

*   07 - Nota Fiscal de Serviço de Transporte;
    
*   08 - Conhecimento de Transporte Rodoviário de Cargas;
    
*   09 - Conhecimento de Transporte Aquaviário de Cargas;
    
*   10 - Conhecimento Aéreo;
    
*   11 - Conhecimento de Transporte Ferroviário de Cargas;
    
*   26 - Conhecimento de Transporte Multimodal de Cargas;
    
*   27 - Nota Fiscal De Transporte Ferroviário De Carga;
    
*   8B - Conhecimento de Transporte de Cargas Avulso.
    

Desta forma, quando a Data de Negociação do documento for maior ou igual a 01/01/2019 (será utilizada a Versão do Layout do Arquivo = 013 - Versão 112 - Início 01/01/2019) e a TOP estiver utilizando algum dos modelos acima, será apresentada a mensagem a seguir:

_**"O modelo de documento X foi desativado pela Sefaz a partir de 01/01/2019, ou seja, para este modelo o EFD ICMS/IPI não aceita o registro D100 com o campo 11 - DT\_DOC maior ou igual a 01/01/2019".**_

[\[voltar ao topo\]](#top)

## Aba Opções

![efd-aba-opcoes.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/14300241637015)

Se a opção **"Tirar Serviços do valor contábil"** for marcada e a nota fiscal possuir serviços entre os itens da nota, os valores destes serviços não serão considerados.

Em **"Custo para o Inventário"**, determine o custo a ser considerado na geração do Bloco H (Inventário) no SPED Fiscal. Nesse caso, teremos as opções:

*   Médio com ICMS;
    
*   Médio sem ICMS;
    
*   Gerencial;
    
*   Reposição;
    
*   Usar maior custo.
    

**Observação:** ao definir este campo com a opção Usar maior custo, será habilitada a seção Maior Custo para valor do item, onde você informará os dois tipos de custo que terão seus valores comparados de modo que o resultado será apresentado na geração do Bloco H.

No campo **"Custo para Inventário/Efeitos IR (Campo 11/reg. H010)"** será determinado o custo a ser considerado na geração do Registro H010, mais precisamente, no campo 11 no SPEd Fiscal. Este campo será habilitado caso esteja-se trabalhando com um Período maior que 31/12/2014. Teremos as seguintes opções:

*   Médio Com ICMS;
    
*   Médio Sem ICMS;
    
*   Gerencial;
    
*   Reposição;
    
*   Usar maior custo.
    

**Observação:** quando este campo for definido com a opção Usar maior custo, será habilitada a seção Maior Custo para efeitos de IR, em que será informado os dois tipos de custo que terão seus valores comparados de modo que o resultado será apresentado na geração do campo 11, Registro H010.

O campo **"Substituir saldo credor sub-apuração ICMS"** possui duas opções disponíveis:

*   **Não substituir:** Ao escolher esta opção, caso exista valor de saldo para uma determinada sub-apuração, o mesmo não será substituído.
    
*   **De todas Sub-Apurações:** Selecionando esta opção, sempre será deletada cada sub-apuração quando o valor credor atual (do mês) for diferente do novo valor credor.
    

Quando a opção **"Gerar Registro C170/C173/C176 para NF-e de emissão própria"** for marcada, na geração do SPED FISCAL, serão apresentados os registros **C170, C173 e C176** para NF-e de emissão própria. Os outros tipos de notas já geram o C170 naturalmente.

**Observação:** por meio do parâmetro **"Conteúdo do campo DESCR\_COMPL do Reg. C170 - DESCPRODFORNEC"** você poderá definir o conteúdo do campo 04-DESCR\_COMPL (Descrição Complementar) do registro C170, de acordo com as seguintes alternativas:

*   **Padrão Complemento:** o sistema continuará utilizando a informação do campo Descrição Complementar do Produto (TGFPRO.COMPLDESC);
    
*   **Descrição do Produto Equivalente:** utiliza a informação do campo **"Descrição do Produto Equivalente"** localizado na aba [Produtos Equivalentes](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#abaprodutosequivalentes) da tela de [Cadastro de Produto](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113) (TGFPAP.DESCRPROPARC);
    
*   **A partir da função:** utiliza o retorno da função SNK\_GET\_DESCPROD\_PARC que deve ser personalizada pelo cliente.
    

Ao realizar a marcação **"Gerar o item da Nota com Unidade Comercializada"**, na geração do SPED Fiscal, será apresentado o registro **"0220 - FATORES DE CONVERSÃO DE UNIDADES"** com a unidade alternativa informada nos lançamentos (o registro C170 demonstra a movimentação dos itens/produtos). Caso a opção esteja desmarcada, apenas o Registro 0200 será gerado na Unidade Padrão.

Se a opção Gerar o Item da Nota com a Unidade Comercializada estiver marcada, e nas Preferências da Empresa, aba EFD - Escrituração Fiscal Digital, sub-aba Blocos e Registros, não tenha-se assinalado a geração do Registro 0220, será apresentado o seguinte aviso:

_**"Atenção: A opção "Gerar o Item da Nota com a Unidade Comercializada" será desmarcada porque o registro "0220" não está marcado para ser gerado."**_

Se o produto possuir mais de uma unidade alternativa para o mesmo volume, diferenciando-o pelo Controle, por exemplo, o primeiro volume alternativo encontrado na geração será o único gerado no registro 0220; os outros serão gerados com o volume padrão.

**Observação:** o item da nota será gerado na Unidade Padrão, se:

1) Nas Preferências da Empresa, aba EFD - Escrituração Fiscal Digital, sub-aba Blocos e Registros, a geração do Registro 0220 estiver desmarcada;

2) A Nota for uma NF-e de emissão própria e o parâmetro **"Usar a unidade padrão na NFe - USARUNIDPADNFE"** estiver ligado;

3) A Nota não for uma NF-e e a marcação Gerar o Item da Nota com a Unidade Comercializada não estiver realizada;

4) Quando o produto possuir duas unidades alternativas iguais, que são diferenciadas pelo campo Controle.

A respeito desta configuração, os seguintes registros envolvidos no SPED serão:

*   **REGISTRO 0190:** IDENTIFICAÇÃO DAS UNIDADES DE MEDIDA
    
*   **REGISTRO 0200:** TABELA DE IDENTIFICAÇÃO DO ITEM (PRODUTO E SERVIÇOS)
    
*   **REGISTRO 0220:** FATORES DE CONVERSÃO DE UNIDADES\*
    
*   **REGISTRO C170:** ITENS DO DOCUMENTO
    
*   **REGISTRO H010:** INVENTÁRIO
    

Esta marcação **"Item de cupom fiscal com 'Código do Produto para NF-e' vazio, usar o parâmetro IMPREFCUPOM"** deverá ser realizada, em casos em que o [Parceiro](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Parceiros) utilize a referência na impressão de cupons, e o [Produto](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Produtos-) em seu cadastro, na aba Impostos, não possua o campo Cód. Produto p/ NF-e preenchido.

A opção **"****Apresenta K200 estoque escriturado negativo para conferência****"** será utilizada apenas para conferência do estoque caso este tenha quantidades negativas, de modo que não será aceito pelo validador esta situação. Se esta marcação não for realizada, serão gerados apenas os produtos que possuem estoque positivo.

A marcação **"Incluir estoque de terceiro a partir das movimentações, no Registro H010?"**, deverá ser selecionada apenas quando existir controle de estoque envolvendo terceiros.

O **"****Gerar o registro H020 para inventário motivo 01****"** deverá ser marcado quando tratar-se de contribuintes do ICMS que necessitem gerar o inventário (final do período "Motivo = 01") com os campos pertinentes ao registro H020 na EFD - Escrituração Fiscal Digital - ICMS/IPI, conforme a legislação da SEFAZ do Rio Grande do Sul. Sendo que, juntamente com o acionamento da referida marcação, se faz necessário preencher o campo **"Data do inventário"** na aba [Parâmetros](#abaparmetros).

**Nota:** na geração do H020 para MOT\_INV, serão gerados apenas os motivos de 02 a 05 conforme o [Guia Prático EFD-ICMS/IPI](http://sped.rfb.gov.br/pasta/show/1573).

A marcação **"Conversão CST 090 Para CST 00 na geração do registro H020"** deve ser utilizada por contribuintes ICMS, quando for necessário converter o CST 090 em CST 00 na geração do registro H020.

**Observação:** para a geração do registro H020, inicialmente, você deve realizar a cópia e a contagem de estoque; após isso, configure a aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044597614-Produtos-com-Mudan%C3%A7a-de-Tributa%C3%A7%C3%A3o#abageral) dos [Produtos com Mudança de Tributação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044597614); ao realizar a importação e processamento dos produtos, verifique se existem registros com o CST 090, (pois somente estes serão gerados no registro H020) e libere-os para EFD. Assim, com os registros liberados, você poderá realizar a geração do EFD na tela EFD - Escrituração Fiscal Digital - ICMS/IPI, configurar a rotina com o período desejado e acionar a marcação Conversão CST 090 Para CST 00 na geração do registro H020 para converter o CST 090 para CST 00.

**Nota:** quando você acionar o botão **"Gerar Arquivo"**, poderá observar que o registro H020 foi gerado e o CST convertido.

A marcação **"****Gerar registros C110/C111/C112/C113/C114/C115 para NF-e de emissão própria****"** será destinada a empresas que têm a necessidade de gerar todos os registros filhos do registro C100, alguns por consequência de sua contabilidade externa, onde exportam o arquivo SPED e utilizam os dados das notas para fazer as conferências e contabilizações; em outras situações, é necessário gerar todos os registros filhos do C100, para fins fiscais, como o caso de demonstrar o local de entrega, no registro C115, por exemplo.

**Observação:** a partir de 01/01/2018, campo 17 (IND\_FRT) correspondente ao registro C100 será gerado com os seguintes códigos:

*   0 - Contratação do Frete por conta do Remetente (CIF);
    
*   1 - Contratação do Frete por conta do Destinatário (FOB);
    
*   2 - Contratação do Frete por conta de Terceiros;
    
*   3 - Transporte Próprio por conta do Remetente;
    
*   4 - Transporte Próprio por conta do Destinatário;
    
*   9 - Sem Ocorrência de Transporte.
    

Como mencionado acima, as seções Maior Custo para valor do item e Maior Custo para efeitos de IR serão habilitadas para uso, caso as marcações Custo para o Inventário e Custo para Inventário/Efeitos IR, respectivamente, estejam definidas com a opção Usar Maior Custo.

**Nota:** na geração do Registro D100, tem-se os campos **"24 - COD\_MUN\_ORIG"** e **"25 - COD\_MUN\_DEST"**, onde são apresentados os Códigos Município Domicílio Fiscal preenchidos anteriormente no [Cadastro de Cidades](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913), [aba Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913#abageral). Caso não exista informação, os campos serão gerados vazios.

**Observação:** ainda em relação à geração do Registro D100, para que o sistema valide a escrituração dos modelos 08 e 08B, o campo **"COD\_MOD"** deverá ser igual a 07, 09, 10, 11, 26 ou 27 e a data informada deverá ser menor que 01/01/2019.

**Nota:** para os Registros D100 e D200, será considerado na geração do arquivo o **"Modelo de Documento"** igual a **"63-Bilhete de Passagem Eletrônico"** (tela [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP), aba [Livro Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abalivrofiscal)).

**Observação:** vale informar que, ao término da geração do livro [ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045115953), as informações pertinentes ao valor calculado do IPI, serão modificadas em um ajuste, ou seja, será gerado um ajuste automático do IPI; esse fato irá ocorrer caso ao menos um parceiro do livro esteja com o campo **"Enquadro no Art. 227. para cálculo de IPI?"** assinalado (localizado na [aba Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Parceiros#abafiscal) do [Cadastro de Parceiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Parceiros)) e a marcação **"Gerar linhas da Nota separadamente no Livro Fiscal?"** estiver realizada (localizada na [aba Livros Fiscais](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Empresa#abalivrosfiscais) das [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Empresa)). Para que o crédito do IPI seja recebido, devem ser escriturados os documentos que comprovem esse benefício. Portanto, os dados serão enviados nos registros E530 e E531. No arquivo de escrituração do livro, a cada linha do E530 tem-se um ou mais registros do E531 para a geração do ajuste automático de IPI.

Quando a opção **"****Gera valores PIS/COFINS no EFD? (É dispensado para quem entrega EFD Contribuições)****"** é acionada, irá caracterizar a geração dos valores de PIS/COFINS no EFD. Sendo que, quando a empresa já realiza a entrega destes valores no EFD - Contribuições.  

Se a marcação **"****Gerar registro 1600 pelo Resumo de Operações com Cartão?****"** estiver selecionada, o sistema utilizará os dados inseridos na tela [Resumo de Operações com Cartão](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044595154) para tratar de forma manual as informações referentes ao Registro 1600 ao Gerar o arquivo. Por outro lado, estando desabilitada a marcação e gerando o arquivo, o sistema não utilizará os dados da referida tela.

De forma semelhante à opção anterior, quando a marcação **"Gerar registro 1601 pelo Resumo de Operações com Cartão?"** estiver habilitada, o sistema utilizará os dados inseridos na tela Resumo de Operações com Cartão para tratar de forma manual as informações referentes ao Registro 1601 ao Gerar o arquivo. Do contrário, estando desabilitada a marcação e gerando o arquivo, o sistema não utilizará os dados da tela Resumo de Operações com Cartão.

Ao acionar a marcação **"Gerar registro C191 mesmo que o ICMS/ST esteja majorando com o FCP?"**, mesmo que o FCP esteja junto ao ICMS/ST no registro C190, os valores do FCP serão gerados neste registro.

[\[voltar ao topo\]](#top)

## Aba Restituição/Complementação de ST

Por meio desta aba, você irá configurar as informações para cálculo dos valores médios de acordo com suas necessidades.

![efd-restituicao-complementacap-de-st.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/14300244593687)

Insira em **"Data do inventário"** a data a qual deseja-se realizar a geração.

No **"Tipo de inventário"** selecione dentre as opções **"Cópia"** e **"Contagem"** o tipo do inventário que será considerado na geração dos cálculos.

Referente aos campos **"Valor do ICMS da Operação"**, **"Base de ST"**, **"Valor de ST"**, **"Valor do FCP de ST" e "Filtro Personalizado"**, configure as fórmulas que desejar para os cálculos.

Nestes campos você terá disposto o botão ![image\_\_9\_.png](https://ajuda.sankhya.com.br/hc/article_attachments/360079273594) **"F(x) Construtor"** que por sua vez, irá o auxiliar na construção das fórmulas. Em relação ao campo ![image\_\_10\_.png](https://ajuda.sankhya.com.br/hc/article_attachments/360080391533) **"Utiliza padrão"**, ao clicar neste o sistema irá utilizar a fórmula padrão.

**Observação:** caso seja necessário realizar qualquer alteração nos campos Valor do ICMS da Operação, Base de ST, Valor de ST, Valor do FCP de ST e Filtro Personalizado, a fórmula utilizada anteriormente ficará gravada na rotina [Repositório de Arquivos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044596594) (aba Fórmula Sped, pasta EFD).

Acesse o artigo [Instruções para geração dos Registros EFD ICMS/IPI - Restituição/Ressarcimento ICMS ST Minas Gerais](https://ajuda.sankhya.com.br/hc/pt-br/articles/360057819854-Instru%C3%A7%C3%B5es-para-gera%C3%A7%C3%A3o-dos-Registros-EFD-ICMS-IPI-Restitui%C3%A7%C3%A3o-Ressarcimento-ICMS-ST-Minas-Gerais), para saber sobre as regras dispostas, às empresas estabelecidas em Minas Gerais.

[\[voltar ao topo\]](#top)

## Aba Prodepe

![efd-aba-prodepe.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/14300256218519)

Nesta aba poderão ser efetuadas as configurações e os cálculos referente ao Benefício PRODEPE.

**Nota:** esta aba servirá para que sejam realizadas as configurações pertinentes ao Registro C177 cadastrado nas Preferências da Empresa, aba EFD - Escrituração Fiscal Digital, sub-aba **"Blocos e Registros"**.

No campo **"Indicador de enquadramento"** informe o enquadramento do registro, de acordo com as opções abaixo:

*   0-Operações não incentivadas;
    
*   1-Indústria (crédito presumido);
    
*   3-Importação (diferimento/crédito presumido);
    
*   4-Central de distribuição (entradas/saídas);
    
*   5-Comércio atacadista - sistemática especial da Lei nº 14.721/2012
    

Selecione no campo **"Indicador de Sub-Apuração"** o tipo de sub-apuração que o registro pertence.

O campo **"Cód. do Produto Sem Incentivo"** desta aba será preenchido com o respectivo código Prodepe referente ao Registro C177 quando no [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Produtos-), aba [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Produtos-#abaimpostos), o campo **"Indicador Esp. Inc. PRODEPE/FUNCRESCE"** encontrar-se com a opção **"Sem incentivo"** selecionada.

[\[voltar ao topo\]](#top)

## Aba Sub-Apuração EFD

Nesta aba serão demonstradas as informações referentes ao valor do saldo credor no momento da geração do EFD, possuindo duas grades, onde uma irá representar informações sobre o saldo credor do mês anterior e a outra, sobre o mês atual.

![aba-sub-apuracao-efd.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/14300261110679)

[\[voltar ao topo\]](#top)

## Arquivos para Registro D695

Por meio desta aba, você poderá vincular os arquivos que as empresas que estão enquadradas no convênio 115/03 do ICMS entregam mensalmente, sendo que este arquivo alimenta os campos dos registros D695 e D696.

![efd-aba-arquivos-para-resgistro\_d695.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/14300333460119)

[\[voltar ao topo\]](#top)

## Botões da tela

No alto da tela, temos alguns botões de extrema importância para este procedimento. A saber:

O botão ![clip3995.bmp](https://ajuda.sankhya.com.br/hc/article_attachments/8767813866391)**"Gerar Arquivo"** quando acionado, realiza de acordo com as condições estabelecidas nas abas **"Parâmetros"** e **"Opções"**, a geração do arquivo de Escrituração.

![efd-pop-up-gerar-arquivo.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/14300353882391)

**Observação:** ao gerar os registros C100, C460, C500, C800, D100 e D500, as movimentações que estiverem com as situações de documento com os códigos abaixo, não serão apresentadas no arquivo TXT.

*    04 - NF-e, NFC-e ou CT-e - Denegado;
    
*    05 - NF-e, NFC-e ou CT-e - Numeração inutilizada.
    

Já através do botão ![clip3996.bmp](https://ajuda.sankhya.com.br/hc/article_attachments/8767814574359) **"Histórico de gerações"** o histórico das gerações de arquivo realizadas serão visualizadas; ao acioná-lo, será aberta a seguinte tela:

![efd-historico-de-geracoes.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/14300440229527)

O botão ![clip3997.bmp](https://ajuda.sankhya.com.br/hc/article_attachments/8767832219415) **"Consultar Nota Não Gerada"** quando acionado, permite a consulta de alguma nota que não tenha sido gerada no livro. Será aberta a seguinte tela para preenchimento dos dados da nota em questão:

![efd.png](https://ajuda.sankhya.com.br/hc/article_attachments/8767969322647)

Depois de informe algum dos dados necessários para pesquisa, ao clicar em **"Consultar"**, podem ser retornados os seguintes resultados:

*   Nota não existe no sistema;
    
*   Nota encontrada nos livros;
    
*   Nota não encontrada nos livros, mas existe no sistema;
    
*   Nota não encontrada nos livros, mas existe como cancelada.
    

[\[voltar ao topo\]](#top)

## Geração dos registros 0450, C110 e C113

Para geração dos registros 0450, C110 e C113, deve-se atentar para os seguintes detalhes:

Nas Preferências da Empresa, aba EFD - Escrituração Fiscal Digital, selecione no campo Tipo de Escrituração a opção **"EFD"**;

Nos quadrantes **"Blocos"** e **"Registros"**, tem-se:

*   Quadrante Blocos, selecione o **"Bloco 0"**;
    
*   Quadrante Registros, selecione o registro **"0450"** e faça a marcação da opção **"Gerar Registro"**;
    
*   Quadrante Blocos, selecione o **"Bloco C"**;
    
*   Quadrante Registros, seleciona-se o registro **"C110"** ou **"C113"**, marcando-se as opções **"Gerar Registro"**, **"Gerar Entrada"** ou **"Gerar Saída"**.
    

Uma vez configurados os blocos nas Preferências da Empresa, são requisitos para a geração dos registros:

*   A  nota possuir uma Observação Padrão (tela [Observações para Notas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044596474)) informada;
    
*    Na configuração da Observação Padrão, o campo Geração no EFD deve estar assinalado com a opção **"Informação Complementar do Documento Fiscal"**;
    
*   Caso seja necessário que o conteúdo do campo 03-TXT\_COMPL do registro C110 seja preenchido, é necessário marcar a opção Carrega Complemento p/EFD na configuração da Observação Padrão;
    
*   O [Tipo de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP) utilizado no lançamento do documento, deve possuir em sua configuração, a marcação **"Buscar NF de origem p/ referenciar"** realizada; esta se encontra presente na [aba Validações](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abavalidaes);
    
*   O Tipo de Operação - TOP utilizado no lançamento do documento de origem a ser gerado no registro C113 deve estar com o campo **"Atualização de Livro ICMS"** devidamente definido, ou seja, deve atualizar o livro correto.
    

Realizadas as configurações acima, automaticamente o sistema passa a gerar os registros 0450 e C110. O registro C113 será gerado apenas quando a nota estiver vinculada a sua origem; por exemplo, nota de devolução de compra vinculada a nota de compra, nota de retorno vinculada a nota de remessa ou nota de acompanhamento de cupom vinculada ao cupom fiscal.

Ao gerar o registro C113 serão apresentadas as chaves referenciadas salvas no campo **"Chave NFe Referenciada Inexistente"** do [Cabeçalho](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045106793-Central-de-Compras#gradecabealho) da tela [Central de Compras](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045106793-Central-de-Compras). Assim, não serão apresentadas chaves em duplicidade para a mesma Nota Origem. **{disponível na versão ≥ 4.27}**

**Importante:** o registro C113 é filho do registro C110 que por sua vez é filho do registro 0450, portanto, para gerar o C113 é preciso gerar o C110 e para gerar o C110 é preciso gerar o registro 0450.

**Observação:** na geração do Registro C100, campo 07 os **"Modelos de Documento"** (tela [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP), aba [Livro Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abalivrofiscal)) opções **"55 - Nota Fiscal Eletrônica"** e **"65 - Nota Fiscal de Venda a consumidor"** serão gerados com três casas decimais complementados com zeros à esquerda quando informado menos de três casas decimais. Para os demais Modelos de Documento previstos no Registro, a série será informada conforme consta no lançamento, em que você poderá inserir até três casas decimais.

**Nota:** quando o parâmetro **"Gerar os reg. C100 e C190 no SPED com os valores de ST? - GERARREGSPED"** estiver ligado, os valores dos campos (23) **"VL\_BC\_ICMS\_ST"** e (24) **"VL\_ICMS\_ST"** do Registro C100 e (08) **"VL\_BC\_ICMS\_ST"** e (09) **"VL\_ICMS\_ST"** do Registro C190, não serão considerados na somatória do Registro E210 quando houver a utilização dos CFOP's 1949 e 2949, visto que, os campos não serão validados devido à restrição de CFOP. E caso esteja desligado e o CFOP for fora do estado da empresa geradora do EFD, é necessário que este esteja com a **"Inscrição Estadual"** do Substituto Tributário cadastrado nas [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa), aba [Insc. Estadual Contribuinte ST no Estado Dest.](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abainsc.estadualcontribuintestnoestadodest.).

[\[voltar ao topo\]](#top)

## Geração do registro 1400

No momento da geração do Registro 1400, para gerar o município do fato gerador, quando o documento utilizado para compor tal informação for um [CT-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044596834), o município a ser considerado será o de origem do CT-e. Considerando todas as situações de geração do município do registro 1400, este somente será gerado quando ele fizer parte do estado da empresa geradora do EFD, por exemplo, se uma empresa estabelecida no estado de Minas Gerais prestar serviço de transporte começando no próprio estado de Minas, este documento irá compor o registro 1400; porém, caso a mesma empresa inicie o serviço de transporte no estado de São Paulo, o documento não irá integrar o registro 1400.

#### Regras para a Geração do registro 1400:

*   A nota deverá ter sido inserida no Registro C100;
    
*   Os parâmetros **"CFOPs que geram Não Dedutíveis no registro 1400 - CFOPNAODED1400"**, **"UFs que geram Não Dedutíveis no registro 1400 - UFSNAODED1400"** e **"UFs que geram NF-e de Venda no registro 1400 - UFSVENREG1400"** deverão estar configurados com as devidas UFs e CFOPs;
    
*   A nota deverá possuir o **"Modelo de Documento"** igual a **"55-Nota Fiscal Eletrônica"** na tela [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP), aba [Livro Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abalivrofiscal);
    
*   A nota deve tratar-se de uma saída, possuir o **"Tipo de Movimento"** igual a **"P-Pedido de venda"** ou **"V-Venda"** e apresentar o valor de frete igual a zero;
    
*   Além disto, a nota deverá encontrar-se com o campo **"Indicador de Presença para NF-e/NFC-e"** (tela Tipos de Operação - TOP, aba [Impressão](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abaimpresso)) com umas das opções seguintes selecionadas: **"0-Não se aplica"**, **"1-Operação presencial"** ou **"5-Presencial, fora do estabelecimento"**;
    
*   Além disto, ainda na tela Tipos de Operação - Top, na aba Livro Fiscal, a marcação **"Gerar Registro 1400 no SPED Fiscal ?"** deverá estar acionada.
    

**Observação:** a tela [Códigos de itens (IPM) por UF no registro 1400](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116093) também deverá ter seu devido registro para que o correto funcionamento do registro ocorra.

**Nota:** para que seja impresso no registro 1400 o Código do Item, deve-se realizar os cadastros das abas [Grupo de Produto, Produto e Tipos de Operação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116093#abasgrupodeprodutoprodutoetiposdeoperao) da tela acima mencionada.

**Observação:** insira no parâmetro **"UFs com cód.IBGE parceiro fornecedor p/ reg.1400 - IBGEPARC1400"** as UFs que serão utilizadas para que, na geração do registro 1400, seja considerado o código do município do Parceiro. Sendo que, o parâmetro citado serve para amparar a regra DIPAM do estado de SP e/ou outras UFs, se necessário.

**Nota:** ao incluir o modelo 04 (NF Produtor Rural) na geração do Registro 1400, o município do parceiro também será gerado, assim como nos modelos 01, 1A, 1B, 55 e 65.

**Configurações necessárias:**

*   Empresa do estado de SP;
*   Parceiro do estado de SP (não pode possuir inscrição estadual);
*   Nota de entrada nos modelos 01, 1A, 55 ou 65;
*   O Parceiro deve ser do mesmo estado da empresa e a UF deve ser preenchida no parâmetro.

Considere também que, para realizar a geração do Registro 1400 para movimentações de CT-e com origem em um estado diferente daquele da Empresa, insira sua UF no campo **"Texto"** do parâmetro **"UFs que geram CT-e Iniciados em Outro Estado no registro 1400 - UFSCTEOUTUF1400"**; sendo que, a UF informada influenciará somente nos registros de saída.

[\[voltar ao topo\]](#top)

## Geração da Conta Contábil para o registro H010

Vejamos abaixo a configuração necessária para geração da Conta Contábil para o registro do inventário H010:

1 - Três parâmetros influenciam a geração do registro H010 do EFD, são eles:

*   Conta p/inventário (H010) do EFD (SPED FISCAL) - EFDH010;
    
*   Conta p/inventário Prop. c/ Terc (H010) do EFD - EFDH010\_PRTER;
    
*   Conta p/inventário Terceiro (H010) do EFD - EFDH010\_TER.
    

Nestes parâmetros, informe contas contábeis fixas para o inventário, de modo que, a informação incluída nos parâmetros será utilizada para geração do Campo 10 (Conta Contábil) do EFD Registro H010.

Caso não seja inserida uma conta contábil fixa, poderão ser informados valores especiais, de forma que o sistema irá localizar a Conta Contábil conforme as regras abaixo:

No [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Produtos-), aba Impostos, se informada:

*   Conta Contábil 1 - O sistema busca a conta contábil 1;
    
*   Conta Contábil 2 - O sistema utiliza a conta contábil 2;
    
*   Conta Contábil 3 - O sistema emprega a conta contábil 3;
    
*   Conta Contábil 4 - O sistema procura a conta contábil 4.
    

O sistema irá utilizar uma destas quatro contas contábeis informadas.

2 - Abaixo, tem-se a configuração para informar a Conta Contábil que será gerada no H010 para empresas diferentes:

Esta situação é aplicada às empresas que geram o registro H010 com Plano de Contas diferentes. Na tela Preferências da Empresa, aba EFD - Escrituração Fiscal Digital, tem-se os campos:

*   **Conta p/inventário (H010) do EFD (SPED FISCAL)** **-** Mesma funcionalidade do parâmetro de chave EFDH010;
    
*   **Conta p/inventário Prop. c/ Terc (H010) do EFD** **\-** Mesma funcionalidade do parâmetro de chave EFDH010\_TER;
    
*   **Conta p/inventário Terceiro (H010) do EFD** **\-** Mesma funcionalidade do parâmetro de chave EFDH010\_PRTER.
    

3 - Ao realizar a geração do bloco H010, registro 010 (COD\_CTA), o sistema irá realizar as seguintes verificações para preencher o campo:

O sistema analisa primeiramente nas Preferências da Empresa, aba EFD - Escrituração Fiscal Digital, se para aquele item, para a empresa que está sendo gerada o SPED, existe alguma configuração para os campos:

*   Conta p/inventário (H010) do EFD (SPED FISCAL);
    
*   Conta p/inventário Prop. c/ Terc (H010) do EFD;
    
*   Conta p/inventário Terceiro (H010) do EFD.
    

Caso algum dos campos esteja definido, seu conteúdo será utilizado para alimentar a conta contábil. Caso não exista, serão utilizadas as configurações dos parâmetros de chave EFDH010, EFDH010\_PRTER e EFDH010\_TER mencionados acima.

A seleção da conta contábil nesses três campos (**Conta p/inventário (H010) do EFD**, **Conta p/inventário Prop. c/ Terc (H010) do EFD** e **Conta p/inventário Terceiro (H010) do EFD**) é feita por um campo de pesquisa com busca sob demanda: ao digitar o código ou a descrição da conta, o sistema retorna os resultados de forma paginada, exibindo código e descrição para seleção. A busca ocorre conforme a digitação de 2 ou mais caracteres, sem carregar toda a lista de contas de uma só vez, garantindo o desempenho da tela em bases com grande volume de registros. Apenas contas válidas do plano de contas podem ser selecionadas; valores livres não são aceitos.

[\[voltar ao topo\]](#top)

## Registros do Bloco K

O Bloco K trata-se de uma parte do SPED Fiscal que contém informações para controle da produção e dos estoques.

O Registro K280, refere-se à Correção de Apontamento do K200. Desta forma, o mesmo ajustará o que foi enviado no Registro K200, ou seja, o cliente após entregar o Registro K200, realizar a contagem do estoque e verificar a necessidade de corrigir o valor enviado neste registro, deverá emitir uma Nota de Ajuste de Estoque com as configurações abaixo devidamente realizadas, para que o Registro K280 possa ser enviado. Vejamos um exemplo:

Foi enviado o Registro K200 no mês de dezembro/2019, porém, em janeiro/2019 constatou-se a diferença no estoque. Assim, deve-se emitir a Nota de Ajuste de Estoque corrigindo esta diferença e, desta forma, quando for encaminhado o SPED em fevereiro/2019, será enviado o K280 com a quantidade ajustada e o K200 também será enviado normalmente com o valor do período.

**Observação:** quando a Nota de Ajuste for emitida, deve-se inserir a data de ajuste do estoque, ou seja, conforme o exemplo acima, a data de dezembro deverá ser informada para que o Registro K280 seja gerado.

Conforme a explicação acima, em relação ao Ajuste de Entrada = Ajuste Positivo de Estoque Próprio realiza-se as seguintes configurações:

*   Na TOP **"Nota de Ajuste de Entrada de Estoque"**, tela [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP), aba [Livro Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abalivrofiscal), a marcação **"Gerar Correção de Apontamento (K280)"** deverá encontrar-se selecionada;
    
*   Ainda na tela acima mencionada, aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abageral), o campo **"Atualização do Estoque"** deverá estar com a opção **"Entrar"** inserida;
    
*   Na aba [Estoque de Terceiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abaestoquedeterceiros) desta mesma tela, o campo **"Estoque com/de Terceiros"** deve possuir a opção **"Não controla"** selecionada;
    
*   Após realizar os ajustes acima, a Nota com as devidas entradas de produtos será criada;
    
*   Em seguida, gera-se o SPED Fiscal;
    
*   Assim, ao abrir o arquivo gerado, pode-se notar que o registro K280 foi gerado e validado no PVA sem erros e com a quantidade de produtos positiva.
    

Referente ao Ajuste de Saída = Ajuste Negativo de Estoque Próprio os ajustes seguintes deverão ser realizados:

*   Deve-se selecionar a TOP **"Nota de Ajuste de Saída de Estoque"** e realizar a marcação Gerar Correção de Apontamento (K280) na aba Livro Fiscal;
    
*   Na aba Geral da tela Tipos de Operação - TOP, o campo Atualização do Estoque deverá se encontrar com a opção **"Baixar"** selecionada;
    
*   O campo Estoque com/de Terceiros localizado na aba Estoque de Terceiros também deverá possuir a opção Não controla inserida;
    
*   Realizando os ajustes acima, cria-se uma Nota com a saída dos produtos;
    
*   Após isto, gera-se o SPED Fiscal e pode-se observar no arquivo a geração de uma correção negativa dos produtos.
    

Referente ao Ajuste de Entrada (positivo) ou Saída (negativo) de Estoque de Terceiro, deve-se realizar as configurações da seguinte forma:

*   Assim como nos ajustes acima, a marcação Gerar Correção de Apontamento (K280) deverá estar efetuada, tanto para ajuste de entrada quanto para o de saída;
    
*   O campo Atualização do Estoque necessita estar com a opção **"Nenhuma"** selecionada;
    
*   Para o Ajuste de Entrada, o campo Estoque com/de Terceiros deve possuir a opção **"Somar ao estoque próprio em poder de terceiro"** inserida e, para o Ajuste de Saída, deverá ser selecionada a opção **"Subtrair ao estoque próprio em poder de terceiro"**;
    
*   Realizadas as configurações acima, deve-se criar as notas (de entrada e saída de produtos);
    
*   Assim, poderá ser observado no arquivo após gerar o SPED Fiscal, a geração positiva e negativa dos produtos.
    

No que se refere ao Ajuste de Entrada ou Saída em Propriedade de Terceiro realize os ajustes abaixo:

*   Selecione a marcação Gerar Correção de Apontamento (K280);
    
*   Insere-se a opção Nenhuma no campo Atualização do Estoque (tanto para ajuste de Entrada quanto para Saída);
    
*   O campo Estoque com/de Terceiros deve possuir a opção **"Somar ao estoque de terceiros em poder da empresa"** para o Ajuste de Entrada e a opção **"Subtrair ao estoque de terceiros em poder da empresa"** para o Ajuste de Saída.
    

Após isto, realize os mesmos procedimentos dos ajustes anteriormente informados.

O Registro K210 (Desmontagem de mercadorias - Item de Origem) tem o objetivo de escriturar a desmontagem de mercadorias de tipos:

*   00 – Mercadoria para revenda;
    
*   01 – Matéria-Prima;
    
*   02 – Embalagem;
    
*   03 – Produtos em Processo;
    
*   04 – Produto Acabado;
    
*   05 – Subproduto;
    
*   10 – Outros Insumos.
    

Sendo que, a quantidade deve ser expressa, obrigatoriamente, na unidade de medida de controle de estoque constante no campo 06 do registro 0200 - UNID\_INV.

**Observação:** quando houver identificação da ordem de serviço, a chave desse registro será os campos **"COD\_DOC\_OS"** e **"COD\_ITEM\_ORI"**. Nos casos em que a ordem de serviço não for identificada, o campo chave passa a ser **"COD\_ITEM\_ORI"**.

Em relação ao Registro K215 (Desmontagem de mercadorias - Item de Destino), ele tem a finalidade de escriturar a desmontagem (com ou sem ordem de serviço) de mercadorias de tipos:

*   00 – Mercadoria para revenda;
    
*   01 – Matéria-Prima;
    
*   02 – Embalagem;
    
*   03 – Produtos em Processo;
    
*   04 – Produto Acabado;
    
*   05 – Subproduto;
    
*   10 – Outros Insumos.
    

**Nota:** o Registro K215 é obrigatório caso exista o registro-pai K210 e o controle da desmontagem não seja por ordem de serviço (campos **"DT\_INI\_OS"**, **"DT\_FIN\_OS"** e **"COD\_DOC\_OS"** do Registro K210 em branco). Nesse caso, a saída do estoque do item de origem e a entrada em estoque do item de destino tem que ocorrer no período de apuração do Registro K100.  
Quando o controle da desmontagem for por ordem de serviço, deverá existir o Registro K215 até o encerramento da ordem de serviço, que poderá ocorrer em outro período de apuração.

**Observação:** a quantidade deve ser expressa, obrigatoriamente, na unidade de medida de controle de estoque constante no campo 06 do registro 0200 - UNID\_INV.

**Nota:** a chave do Registro K215 é o campo **"COD\_ITEM\_DES"**.  

[\[voltar ao topo\]](#top)

## Registro 0300 e G125

Quando a marcação **"Gerar CIAP de componentes para SPED"** nas [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa), aba [Bens](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#ababens) estiver realizada, o sistema irá gerar o Registro 0300 considerando o preenchimento do campo 05 (COD\_PRNC), vinculando-o a um bem principal, gerando um Registro 0300 para o bem principal e, por fim, preenchendo o campo 03 (IDENT\_MERC) com a opção **"2 - componente"**.

**Observação:** para o Registro G125, o parâmetro **"Utiliza TIPOENTCIAP para geração do SPED - TIPOENTCIAPSPED"** já leva o EFD para todos os produtos, independentemente se são bens ou componentes, conforme a opção marcada no campo **"Tipo de Movimentação do Bem ou Componente"** da aba [Bens](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#ababens) do [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-).

Ao fazer o cadastro de um componente ou bem, marcando a opção **"IA-Imobilização em Andamento - Componente"**, o sistema levará esse código para o EFD. Assim, após processar o EFD na tela EFD - Fiscal ICMS/IPI, será possível validar que o campo 05 (COD\_PRNC) está vinculado a um bem principal e demonstrado nele, bem como verificar a marcação correta do campo 03 (IDENT\_MERC) como sendo um componente, uma vez que está vinculado a um bem principal. 

[\[voltar ao topo\]](#top)

### **Geração Consolidada da NFCom (Registros D750, D760 e D761)**

Para atender às legislações estaduais que exigem a escrituração consolidada de notas de telecomunicação (NFCom - Modelo 62), o sistema permite a geração dos registros **D750, D760 e D761**.

##### **1\. Como habilitar a consolidação**

Por padrão, o sistema gera os documentos da NFCom de forma individualizada no registro **D700**. Para alterar esse comportamento e passar a consolidar as notas de saída:

*   Acesse a tela **Comercial » Preferências »** [**Empresa**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa);
*   Na aba **EFD - Escrituração Fiscal Digital**, adicione o registro **D750**.

**Nota:** não é necessário remover o registro D700 da configuração, pois o sistema fará a separação automática dos documentos conforme as regras abaixo.

##### **2\. Regras de Separação (D750 vs D700)**

Ao habilitar o D750, o sistema divide a escrituração da seguinte forma:

**Irão para o Registro D750 (Consolidado):**

*   Apenas documentos NFCom (Modelo 62);
*   Apenas notas de **Saída**;
*   Apenas notas com Finalidade **Normal** (finNFCom = 0);
*   Documentos regulares (Autorizados).

**Continuarão no Registro D700 (Individualizado):**

*   Notas de **Entrada**;
*   Notas de **Ajuste** ou **Substituição** (finNFCom diferente de 0);
*   Notas que representem ajustes de apuração por documento.

**Importante****:** documentos **Cancelados** não são escriturados em nenhum dos registros e não são levados para o SPED. Além disso, notas emitidas **sem CST preenchido** impedirão a geração da escrituração, apresentando uma mensagem de alerta.

##### **3\. Estrutura dos Novos Registros**

O sistema fará o agrupamento das informações respeitando a seguinte hierarquia:

*   **Registro D750 (Consolidação):** Agrupa as notas de saída pela combinação de **Modelo, Série, Data de Emissão e Indicador de Pagamento**.
    *   _Particularidade:_ Como o sistema atualmente gera faturamentos normais, o indicador de pagamento será assumido por padrão como "1" (Pós-pago). O valor de deduções será preenchido quando o código de classificação do serviço (cClass) for 590.
*   **Registro D760 (Detalhamento):** É o registro "filho" do D750. Ele detalha os valores totais consolidados, quebrando-os pela combinação de **CFOP, Alíquota de ICMS e CST**. Não haverá linhas duplicadas com a mesma combinação para o mesmo dia/série.
*   **Registro D761 (Fundo de Combate à Pobreza):** Presta as informações referentes ao **FCP** constantes nas NFComs consolidadas. Seus valores são informativos.

[\[voltar ao topo\]](#top)