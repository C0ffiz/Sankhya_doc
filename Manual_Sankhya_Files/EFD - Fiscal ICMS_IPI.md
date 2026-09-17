# EFD - Fiscal ICMS/IPI

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/7267044122263-EFD-Fiscal-ICMS-IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/7267044122263-EFD-Fiscal-ICMS-IPI)

---

# EFD - Fiscal ICMS/IPI

```auto
 Módulo: Livros Fiscais > Conexão
```

---

![essencial FINAL (1).png](https://ajuda.sankhya.com.br/hc/article_attachments/19035987846167) Esta tela está disponível somente em HTML5.

**Importante:** para que você consiga acessar essa tela, habilite o parâmetro **"Habilita geração novo layout EFD Fiscal? - HABEFISLAYNOVO"**.

A Escrituração Fiscal Digital - EFD é um arquivo digital, que se constitui de um conjunto de escriturações de documentos fiscais e de outras informações de interesse do fisco das Unidades Federadas e da Secretaria da Receita Federal do Brasil (RFB), bem como, de registros Gerar registro 1600 pelo Resumo de Operações com Cartão e apuração de impostos referentes às operações e prestações praticadas pelo contribuinte.

<table style="border-collapse: collapse;"><tbody><tr style="height: 24px;"><td style="height: 24px; width: 100%;"><h4 class="wysiwyg-text-align-center" id="h_01HY38V75XZNRAZ4W6ZT6KJ6GT"><span style="color: #4D4D4D;"><strong>Funcionalidades da tela</strong></span></h4></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 100%;"><a href="#Preenchimentos%20Iniciais">Preenchimentos iniciais</a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 100%;"><a class="topiclink" href="#abaconfigura%C3%A7%C3%B5es" target="_self" rel="undefined"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Aba Configurações</span></a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 100%;"><a href="#demaisabasdatela" target="_self"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Demais abas da tela</span></a><span style="font-family: Verdana,Geneva,Arial,sans-serif;"> &nbsp;</span></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 100%;"><a class="topiclink" href="#botoesdatela"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Botões da tela</span></a><br>&nbsp;</td></tr><tr style="height: 22px;"><td style="height: 22px; width: 100%;"><a href="#gera%C3%A7%C3%A3odosregistros0450,C110eC113" target="_self" rel="undefined">Geração dos registros 0450, C110 e C113</a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 100%;"><a href="#registroc173" target="_self">Registro C173</a></td></tr><tr><td style="width: 100%;"><a href="#RegistroC177">Registro C177</a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 100%;"><a href="#registroc180" target="_self">Registro C180</a></td></tr><tr><td style="width: 100%;"><a href="#IndicadordeFretenoregistroD100">Indicador de Frete no registro D100</a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 100%;"><a href="#gera%C3%A7%C3%A3odacontacont%C3%A1bilparaoregistroh010" target="_self">Geração da Conta Contábil para o Registro H010</a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 100%;"><a href="#registros0300eg125" target="_self">Registros 0300 e G125</a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 100%;"><a href="#gera%C3%A7%C3%A3odoregistro1400" target="_self">Geração do registro 1400</a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 100%;"><a href="#Gera%C3%A7%C3%A3odoregistro0205">Geração do registro 0205</a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 100%;"><a href="#0221">Geração do registro 0221</a></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 100%;"><a href="#registrosdoblocok" target="_self">Registros do bloco K</a></td></tr><tr><td><a href="#h_01KC1G55KVG8A1JNY56E8STQED">Adequação do ERP ao SPED Fiscal (EFD-ICMS/IPI) 3.1.9 e 3.2.0</a></td></tr></tbody></table>

---

### **Preenchimentos Iniciais**

![aba\_op\_\_es.png](https://ajuda.sankhya.com.br/hc/article_attachments/8114763780375)  
No **"Painel Principal"** dessa tela, a primeira informação a ser preenchida, é a **"Empresa"** da qual serão gerados os dados para escrituração. Ao manter o campo Empresa em branco, temos a possibilidade de realizar a geração prévia de dados, selecionar várias ou todas as empresas configuradas para gerar o EFD - Escrituração Fiscal Digital.

No campo **"Referência"**, você deve informar o primeiro dia do mês/ano a que o arquivo será gerado.

**Observação:** quando informada a mesma Empresa em uma Referência posterior a uma que já tenha realizado o EFD - Fiscal, se houver dados na sub-aba [Restituição/Complementação de ST](#sub-abaRestitui%C3%A7%C3%A3o/Complementa%C3%A7%C3%A3odeST) estes serão copiados da última Referência. Além disso, ao excluí-la, suas movimentações e registros também serão excluídos das tabelas e bancos de dados do sistema. 

O campo **"Versão do Layout"** será apresentado com impossibilidade de edição e exibirá a versão do layout do arquivo que está sendo utilizada para a geração da escrituração. As versões são utilizadas de acordo com o período inicialmente informado. Sendo assim, teremos:

<table style="border-collapse: collapse;"><tbody><tr style="background-color: #90ee90; height: 22px;"><td style="height: 22px; text-align: center; width: 25.0001%;"><span style="color: #4D4D4D;"><strong>CÓDIGO</strong></span></td><td style="height: 22px; text-align: center; width: 25.6428%;"><strong>VERSÃO</strong></td><td style="height: 22px; text-align: center; width: 23.3213%;"><span style="color: #4D4D4D;"><strong>LEIAUTE</strong></span></td><td style="height: 22px; text-align: center; width: 26.0357%;"><p><span style="color: #4D4D4D;"><strong>OBRIGATORIEDADE</strong></span></p><p><span style="color: #4D4D4D;"><strong>(INÍCIO)</strong></span></p></td></tr><tr style="height: 22px;"><td style="height: 22px; text-align: center; width: 25.0001%;"><span style="color: #4D4D4D;">&nbsp;015</span></td><td style="height: 22px; text-align: center; width: 25.6428%;">114</td><td style="height: 22px; text-align: center; width: 23.3213%;"><span style="color: #4D4D4D;">Ato COTEPE</span></td><td style="height: 22px; text-align: center; width: 26.0357%;">01/01/2021</td></tr><tr style="height: 22px;"><td style="height: 22px; text-align: center; width: 25.0001%;"><span style="color: #4D4D4D;">&nbsp;016</span></td><td style="height: 22px; text-align: center; width: 25.6428%;">115</td><td style="height: 22px; text-align: center; width: 23.3213%;"><span style="color: #4D4D4D;">Ato COTEPE</span></td><td style="height: 22px; text-align: center; width: 26.0357%;"><span style="color: #4D4D4D;">01/01/2022</span></td></tr><tr style="height: 22px;"><td style="height: 22px; text-align: center; width: 25.0001%;">017</td><td style="height: 22px; text-align: center; width: 25.6428%;">116</td><td style="height: 22px; text-align: center; width: 23.3213%;"><span style="color: #4D4D4D;">Ato COTEPE</span></td><td style="height: 22px; text-align: center; width: 26.0357%;"><span style="color: #4D4D4D;">01/01/2023</span></td></tr><tr style="height: 22px;"><td style="height: 22px; text-align: center; width: 25.0001%;"><span style="color: #4D4D4D;">018</span></td><td style="height: 22px; text-align: center; width: 25.6428%;">117</td><td style="height: 22px; text-align: center; width: 23.3213%;"><span style="color: #4D4D4D;">Ato COTEPE</span><br>&nbsp;</td><td style="height: 22px; text-align: center; width: 26.0357%;"><span style="color: #4D4D4D;">01/01/2024</span></td></tr><tr style="height: 22px;"><td style="height: 22px; text-align: center; width: 25.0001%;"><span style="color: #4D4D4D;">019</span></td><td style="height: 22px; text-align: center; width: 25.6428%;">118</td><td style="height: 22px; text-align: center; width: 23.3213%;"><span style="color: #4D4D4D;">Ato COTEPE</span></td><td style="height: 22px; text-align: center; width: 26.0357%;"><span style="color: #4D4D4D;">01/01/2025</span></td></tr></tbody></table>

**Importante:** nessa tela será possível gerar apenas os layout's a partir dos exercícios 2021 (Layout 015/Versão114). Caso você tente gerar os layout's anteriores, será exibida a mensagem abaixo:

_**"Prezado usuário, para geração de arquivos em layout's anteriores ao exercício 2021 (Layout 015/Versão114), acessar a rotina:**_ [_**EFD - Escrituração Fiscal Digital ICMS/IPI**_](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607614-EFD-Escritura%C3%A7%C3%A3o-Fiscal-Digital-ICMS-IPI) _**em (Livros Fiscais » Conexão » EFD - Escrituração Fiscal Digital - ICMS/IPI)."**_ 

---

 **![informações adicionais FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16310089145751) Informações adicionais acerca da opção 017 - Versão 116 - Início 01/01/2023:**

Ao processar o [EFD Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607614) utilizando a opção 017 - Versão 116 - Início 01/01/2023, o sistema irá gerar na tela e no arquivo TXT os registros abaixo:

*   C855 e C857 para o perfil A, buscando as notas de Modelo 59 que possuem as informações registradas nesta aba. Lembrando que, estes registros devem estar devidamente preenchidos/associados nas Preferências da Empresa, aba [EFD - Escrituração Fiscal Digital](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893#abaefdescrituraofiscaldigital), juntamente com os demais registros do Bloco C, seguindo a hierarquia definida no Layout EFD.
    

Na hierarquia do Bloco C, os registros C855 e C857 se encontram na hierarquia 3 e 4 respectivamente, abaixo do registro C800 de hierarquia 2.

*   C895 e C897 para o perfil B e C, buscando as notas de Modelo 59 que possuem as informações registradas nesta aba. Lembrando que, estes registros devem estar devidamente preenchidos/associados nas Preferências da Empresa, aba EFD - Escrituração Fiscal Digital, juntamente com os demais registros do Bloco C, seguindo a hierarquia definida no Layout EFD.
    

Na hierarquia do Bloco C, os registros C895 e C897 se encontram na hierarquia 3 e 4 respectivamente, abaixo do registro C860 de hierarquia 2.

---

 **![informações adicionais FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16310089145751) Informações adicionais acerca da opção 019 - Versão 118 - Início 01/01/2025:** 

Ao processar o [EFD Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607614) utilizando a opção 019 - Versão 118 - Início 01/01/2025, o sistema irá gerar na tela e no arquivo TXT os registros abaixo:

*   **E113:**  ao processar esse registro, o campo **"Parceiro"** presente na aba E113 será preenchido conforme o modelo definido.
    

Caso o modelo seja igual a 59 (CF-e SAT), 63 (BP-e) ou 65 (NFC-e), o campo 02 do TXT será gerado vazio, ou seja, deve desconsiderar o código do parceiro do documento.

Se o modelo de documento for igual a 06 (NF/CEE) ou 66 (NF3e), o campo não será obrigatório, podendo estar vazio ou com conteúdo, a considerar o código do parceiro do documento.

Para os demais modelos de documento, por exemplo: 55 (NF-e) o campo é obrigatório, e deve ser gerado com o código do parceiro do documento.

*   **D100:** ao processar esse registro, o campo **"Chave do Bilhete de Passagem Eletrônico substituído"** da aba **"D100"**, sub-aba **"Geral"** do Bloco D deve ser preenchido com o conteúdo do campo **"Chave CT-e referenciada"** na grade de [Cabeçalho](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045106793-Central-de-Compras#gradecabealho) da [Central de Compras](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045106793-Central-de-Compras) ou na aba [Principal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601874-Movimenta%C3%A7%C3%A3o-Financeira-Atributos-da-Tela#Principal) da [Movimentação Financeira](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601874-Movimenta%C3%A7%C3%A3o-Financeira-Atributos-da-Tela) se o tipo do CT-e for igual a 3 ou a 6. O preenchimento desse campo, reflete na geração do campo 14 do TXT.
    

Ainda, com relação ao registro D100, o campo 24 preenchido conforme o conteúdo do campo **"Código do município IBGE de origem"**, e o campo 25  preenchido conforme o conteúdo do campo **"Código do município IBGE de destino"** todos da aba D100 do Bloco D, sendo que no registro do CTe Simplificado (Tipos de emissão igual a 5 - CT-e Simplificado e 6 - Substituição de CT-e), estes campos serão preenchidos de forma fixa com o conteúdo 9999998 para operações nacional e 9999999 para operações com o exterior, enquanto que na ótica do CT-e normal, estes campos serão preenchidos com o código IBGE da empresa e do parceiro da nota para operações nacional e 9999999 para operações com o exterior.

---

Quando a marcação **"Arquivo confirmado"** for efetuada, efetuará o bloqueio da possibilidade de reprocessamento do arquivo. 

 [\[voltar ao topo\]](#top)

### **Aba Configurações**

Nessa aba serão definidas as parametrizações necessárias para geração do arquivo EFD. 

<table style="border-collapse: collapse;"><tbody><tr><td style="width: 100%;"><h4 id="h_01HY3G53B0MESXY608W40APVH1"><strong>Sub-abas</strong>&nbsp;</h4></td></tr><tr><td class="wysiwyg-text-align-justify" style="width: 100%;"><a href="#sub-abaop%C3%A7%C3%B5es" target="_self">Sub-aba Opções</a></td></tr><tr><td class="wysiwyg-text-align-justify" style="width: 100%;"><a href="#sub-abaprodepe" target="_self" rel="undefined">Sub-aba Prodepe</a></td></tr><tr><td class="wysiwyg-text-align-justify" style="width: 100%;"><a href="#sub-abasub-apura%C3%A7%C3%A3oefd" target="_self">Sub-aba Sub-Apuração EFD</a></td></tr><tr><td class="wysiwyg-text-align-justify" style="width: 100%;"><a href="#sub-abaRestitui%C3%A7%C3%A3o/Complementa%C3%A7%C3%A3odeST" target="_self">Sub-aba Restituição/Complementação de ST</a></td></tr><tr><td class="wysiwyg-text-align-justify" style="width: 100%;"><a href="#sub-abaarquivosregistrosd695" target="_self">Sub-aba Arquivos Registros D695</a></td></tr></tbody></table>

Assim, observe os dados que serão configurados aqui:

Preencha do campo **"Período"**, o intervalo de tempo definido conforme o campo Data Referência do Painel Principal dessa tela. Uma vez que, o Período irá abranger a geração do relatório.

Em **"UF"**, informe a uf a ser considerada para a geração do arquivo.

Na **"Finalidade de Apresentação do Arquivo"**, será definido o objetivo da geração do arquivo. Nesta, você terá duas alternativas, sendo elas **"****Remessa do arquivo original"** e **"****Remessa do arquivo substituto"**.

Informe no campo **"Data do inventário"**, a data que o sistema irá considerar para a geração da escrituração.

O campo **"Data de Inventario em substituição ao Bloco K"** é destinado para geração do H005 na posição mensal em substituição ao Bloco K e será exibido quando o parâmetro **"Gerar Bloco H em substituição ao Bloco K - GERBLHSUBSK"** estiver ligado. Ao informar uma data nesse campo será gerado no arquivo do EFD, um Bloco H correspondente à cópia de estoque registrada na data informada em substituição ao Bloco K. E, sempre que houver um Bloco H para a data informada, o sistema deixará de gerar o Bloco K correspondente às informações provenientes desta cópia de estoque.

**Observação:** havendo as duas informações, um pop-up será apresentado para que a posição do estoque que será utilizada no EFD seja definida por meio do campo **"Utilizar dados do inventário mensal"** conforme as opções:

*   **Pela cópia**: o sistema considera para a geração do H005, os saldos da cópia de estoque da data informada;
    
*   **Pela contagem**: o sistema considera para a geração do H005, os saldos da contagem de estoque da data informada.
    

![dados\_inventario.png](https://ajuda.sankhya.com.br/hc/article_attachments/13057090156439)

No campo **"Data da contagem p/ K200"**, você poderá inserir a data da contagem para a geração do registro na tela [Dashboard auxiliar do BLOCO K](https://ajuda.sankhya.com.br/hc/pt-br/articles/4411588603159--Dashboard-auxiliar-do-BLOCO-K) após a execução da cópia e contagem de estoque no processo de inventário. Porém, para que o campo seja exibido, é preciso ligar o parâmetro **"GERARK200CTE"**, de forma que, com este desligado, será considerado o estoque que consta no último dia da geração do SPED Fiscal da referência em questão.

**Observação:** com os parâmetros Gerar Bloco H em substituição ao Bloco K - GERBLHSUBSK e GERAK200CTE habilitados, tem-se: 

Que os campos Data de contagem p/ K200 e Data de Inventario em substituição ao Bloco K serão exibidos e, ao preenchê-los simultaneamente e processar o EFD, o sistema exibirá a seguinte mensagem:

_**"O campo “Data de contagem p/ K200” não pode estar preenchido se o campo “Data de Inventario em substituição ao Bloco K” também estiver preenchido. Defina qual data será utilizada para a geração do arquivo."**_

Porém, com o campo Data de contagem p/ K200 configurado e o Data de Inventario em substituição ao Bloco K vazio, o sistema realizará a geração do Bloco K na tela [Dashboard auxiliar do Bloco K](https://ajuda.sankhya.com.br/hc/pt-br/articles/4411588603159--Dashboard-auxiliar-do-BLOCO-K) após a execução da cópia e contagem de estoque no processo de inventário;

Ao preencher o campo Data de Inventario em substituição ao Bloco K e o campo Data de contagem p/ K200 ficar vazio, ao realizar o processamento do EFD, o sistema irá executar a geração do Bloco H de forma que irá substituir o Bloco K;

Por fim, com ambos os campos vazios, quando o processamento do EFD for realizado, o sistema exibirá a seguinte mensagem:

_**"O parâmetro GERAK200CTE está ligado, então a "Data da Contagem p/ K200" deve ser informada."**_

No campo **"Perfil EFD"** será apresentado o perfil no qual o arquivo será gerado.

Se necessário, informe o **"Nro. Único Nota"** de modo que, o sistema irá gerar as informações da nota em questão.

**Observação:** desde 01/01/2019 não é mais aceito os seguintes modelos de documentos relacionados à conhecimentos de transporte:

*   07 - Nota Fiscal de Serviço de Transporte;
    
*   08 - Conhecimento de Transporte Rodoviário de Cargas;
    
*   09 - Conhecimento de Transporte Aquaviário de Cargas;
    
*   10 - Conhecimento Aéreo;
    
*   11 - Conhecimento de Transporte Ferroviário de Cargas;
    
*   26 - Conhecimento de Transporte Multimodal de Cargas;
    
*   27 - Nota Fiscal De Transporte Ferroviário De Carga;
    
*   8B - Conhecimento de Transporte de Cargas Avulso.
    

Dessa forma, quando a Data de Negociação do documento for maior ou igual a 01/01/2019 (será utilizada a Versão do Layout do Arquivo = 013 - Versão 112 - Início 01/01/2019) e a TOP estiver utilizando algum dos modelos acima, será apresentada a seguinte mensagem:

_**"O modelo de documento X foi desativado pela Sefaz a partir de 01/01/2019, ou seja, para este modelo o EFD ICMS/IPI não aceita o registro D100 com o campo 11 - DT\_DOC maior ou igual a 01/01/2019"**._

[\[voltar ao topo\]](#top)

---

#### **Sub-aba Opções**

Essa sub-aba dispõe dos seguintes campos:

Quando a marcação **"Tirar Serviços do valor contábil"** for acionada, e a nota fiscal possuir serviços entre os itens da nota, os valores desses serviços não serão considerados.

Em **"Custo para o Inventário"**, determine o custo a ser considerado na geração do Bloco H (Inventário) no SPED Fiscal. Nesse caso, teremos as opções:

*   Médio com ICMS;
    
*   Médio sem ICMS;
    
*   Gerencial;
    
*   Reposição;
    
*   Usar maior custo.
    

**Observação:** quando a opção Usar maior custo for definida no campo acima, será a seção **"****Maior Custo para valor do item"** será habilitada, dessa forma, você informará os tipos de custos que terão seus valores comparados de modo que, o resultado será apresentado na geração do Bloco H. 

No campo **"Custo para Inventário/Efeitos IR (Campo 11/reg. H010)"**, será determinado o custo a ser considerado na geração do Registro H010, mais precisamente, no campo 11 no SPEd Fiscal. Esse campo será habilitado caso você estiver trabalhando com um Período maior que 31/12/2014. Assim, teremos as opções:

*   Médio Com ICMS;
    
*   Médio Sem ICMS;
    
*   Gerencial;
    
*   Reposição;
    
*   Usar maior custo.
    

**Observação:** quando esse campo for definido com a opção Usar maior custo, será habilitada a seção **"****Maior Custo para efeitos de IR"**, em que, será informado os tipos de custos que terão seus valores comparados de modo que o resultado será apresentado na geração do campo 11 do Registro H010. 

O campo **"Substituir saldo credor sub-apuração ICMS"** possui duas opções:

*   **Não substituir:** Ao escolher essa opção, caso exista valor de saldo para uma determinada sub-apuração, o mesmo não será substituído.
    
*   **De todas Sub-Apurações:** Selecionando essa opção, sempre será deletada cada sub-apuração quando o valor credor atual (do mês) for diferente do novo valor credor.
    

Quando a opção **"Gerar Registro C170/C173/C176 para NF-e de emissão própria"** for marcada, na geração do SPED FISCAL, serão apresentados os registros **C170, C173 e C176** para NF-e de emissão própria. Os outros tipos de notas já geram o C170 naturalmente.

**Observação:** por meio do parâmetro **"Conteúdo do campo DESCR\_COMPL do Reg. C170 - DESCPRODFORNEC"** pode-se definir o conteúdo do campo 04-DESCR\_COMPL (Descrição Complementar) do registro C170, de acordo com as seguintes alternativas:

*   **Padrão Complemento:** o sistema continuará utilizando a informação do campo Descrição Complementar do Produto (TGFPRO.COMPLDESC);
    
*   **Descrição do Produto Equivalente:** utiliza a informação do campo **"Descrição do Produto Equivalente"** localizado na aba [Produtos Equivalentes](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#abaprodutosequivalentes) da tela de [Cadastro de Produto](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113) (TGFPAP.DESCRPROPARC);
    
*   **A partir da função:** utiliza o retorno da função SNK\_GET\_DESCPROD\_PARC que deve ser personalizada pelo cliente.
    

Ao realizar a marcação **"Gerar o item da Nota com Unidade Comercializada"**, na geração do SPED Fiscal, será apresentado o registro **"0220 - FATORES DE CONVERSÃO DE UNIDADES"** com a unidade alternativa informada nos lançamentos (o registro C170 demonstra a movimentação dos itens/produtos). Se esta não for acionada, apenas o Registro 0200 será gerado na Unidade Padrão.

**Observação:** o parâmetro **"Cod. Cont. Origem no Reg C170 Contabil. por Matriz - LIVCODCONTAMAT"** deve ser habilitado quando houver transferência entre empresas que utilizam o mesmo plano de contas, sendo que a contabilização será feita na empresa matriz e não nas empresas filiais. Caso contrário, o código da conta analítica contábil debitada/creditada aparecerá apenas se a empresa responsável pelo registro do C170 do EFD - Fiscal ICMS/IPI for a mesma que gerou a contabilidade ou a empresa de origem.

Ao habilitar a marcação Gerar o Item da Nota com a Unidade Comercializada, e nas [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa), aba [EFD - Escrituração Fiscal Digital](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#se%C3%A7%C3%A3oefdcontribui%C3%A7%C3%B5es), sub-aba **"****Blocos e Registros"**, a marcação **"Gerar Registro"** para a geração do Registro 0220, será apresentado o seguinte aviso:

_**"Atenção: A opção "Gerar o Item da Nota com a Unidade Comercializada" será desmarcada porque o registro "0220" não está marcado para ser gerado."**_

Se o produto possuir mais de uma unidade alternativa para o mesmo volume, diferenciando-o pelo Controle, por exemplo, o primeiro volume alternativo encontrado na geração será o único gerado no registro 0220; os outros serão gerados com o volume padrão.

**Observações:** o item da nota será gerado na Unidade Padrão, se:

1\. Nas Preferências da Empresa, aba EFD - Escrituração Fiscal Digital, sub-aba Blocos e Registros, a geração do Registro 0220 estiver desmarcada;

2\. A Nota for uma NF-e de emissão própria e o parâmetro **"Usar a unidade padrão na NFe - USARUNIDPADNFE"** estiver ligado;

3\. A Nota não for uma NF-e e a marcação Gerar o Item da Nota com a Unidade Comercializada não estiver realizada;

4\. Quando o produto possuir duas unidades alternativas iguais, que são diferenciadas pelo campo Controle.

Referente a essa configuração, os seguintes registros envolvidos no SPED serão:

*   **REGISTRO 0190:** IDENTIFICAÇÃO DAS UNIDADES DE MEDIDA
    
*   **REGISTRO 0200:** TABELA DE IDENTIFICAÇÃO DO ITEM (PRODUTO E SERVIÇOS)
    
*   **REGISTRO 0220:** FATORES DE CONVERSÃO DE UNIDADES\*
    
*   **REGISTRO C170:** ITENS DO DOCUMENTO
    
*   **REGISTRO H010:** INVENTÁRIO
    

A marcação **"Item de cupom fiscal com 'Código do Produto para NF-e' vazio, usar o parâmetro IMPREFCUPOM"**, deverá ser realizada em casos em que o [Parceiro](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Parceiros) utilize a referência na impressão de cupons, e o [Produto](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Produtos-) em seu cadastro, na aba Impostos, não possua o campo Cód. Produto p/ NF-e preenchido.

Considere que a marcação **"****Apresenta K200 estoque escriturado negativo para conferência****"**, será acionada apenas para conferência do estoque caso este tenha quantidades negativas. Se essa marcação não for realizada, serão gerados apenas os produtos que possuem estoque positivo.

A marcação **"Incluir estoque de terceiro a partir das movimentações, no Registro H010?"**, deverá ser selecionada apenas quando existir controle de estoque envolvendo terceiros.

A marcação **"****Gerar registro H020 para inventário motivo 01****"**, deverá ser marcada quando tratar-se de contribuintes do ICMS que necessitem gerar o inventário (final do período "Motivo = 01") com os campos pertinentes ao registro H020 na EFD - Escrituração Fiscal Digital - ICMS/IPI, conforme a legislação da SEFAZ do Rio Grande do Sul. Sendo que, juntamente com o acionamento da referida marcação, será necessário preencher o campo **"Data do inventário"** na aba [Parâmetros](#abaparmetros).

A marcação **"Gerar BC e ICMS no H020 para Inventário Motivo 01"** será liberada somente quando a marcação **"Gerar registro H020 para Inventário Motivo 01"** estiver habilitada. 

Neste caso, quando ambas as marcações forem ativadas e o CST do item for igual a 000, ao processar o arquivo o sistema irá gerar na aba H001, um registro H020 para cada registro H010, desde que o registro H005 seja igual a 01. Além disso, serão preenchidos automaticamente os campos **"Base de cálculo do ICMS"** e **"Valor do ICMS a ser debitado ou creditado"** na sub-aba H020. 

A opção **"Considera valor unitário para os campos BC\_ICMS e VL\_ICMS do registro H020"** deve ser ativada junto com as seguintes configurações:

*   **Gerar registro H020 para Inventário Motivo 01**
    
*   **Gerar BC e ICMS no H020 para Inventário Motivo 01**
    

Quando habilitada, essa opção garante que o registro H020 utilize corretamente o valor unitário. Caso esteja desativada, o sistema mantém o comportamento padrão, onde a marcação **"Gerar BC e ICMS no H020 para Inventário Motivo 01"** só será liberada se a opção **"Gerar registro H020 para Inventário Motivo 01"** estiver ativada.

A marcação **"Conversão CST 090 Para CST 00 na geração do registro H020"** deve ser utilizada por contribuintes ICMS quando for necessário converter o CST 090 em CST 00 na geração do registro H020. 

**Observação:** para a geração do registro H020, inicialmente, você deve realizar a cópia e a contagem de estoque; após isso, configure a aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044597614-Produtos-com-Mudan%C3%A7a-de-Tributa%C3%A7%C3%A3o#abageral) dos [Produtos com Mudança de Tributação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044597614) e, ao realizar a importação e o processamento dos produtos, verifique se existem registros com o CST 090 (pois somente estes serão gerados no registro H020) e libere-os para EFD. Assim, com os registros liberados, você poderá realizar a geração do EFD na tela EFD - Escrituração Fiscal Digital - ICMS/IPI, configurar a rotina com o período desejado e acionar a marcação Conversão CST 090 Para CST 00 na geração do registro H020 para converter o CST 090 para CST 00.

**Nota:** quando você acionar o botão **"Gerar Arquivo"**, observe que o registro H020 foi gerado e o CST convertido.

A marcação **"****Gerar registros C110/C111/C112/C113/C114/C115 para NF-e de emissão própria****"** será destinada a empresas que têm a necessidade de gerar todos os registros filhos do registro C100, alguns por consequência de sua contabilidade externa, onde exportam o arquivo SPED e utilizam os dados das notas para fazer as conferências e contabilizações; em outras situações, é necessário gerar todos os registros filhos do C100, para fins fiscais, como o caso de demonstrar o local de entrega, no registro C115, por exemplo. 

**Observação:** a partir de 01/01/2018, campo 17 (IND\_FRT) correspondente ao registro C100 será gerado com os seguintes códigos:

*   0 - Contratação do Frete por conta do Remetente (CIF);
    
*   1 - Contratação do Frete por conta do Destinatário (FOB);
    
*   2 - Contratação do Frete por conta de Terceiros;
    
*   3 - Transporte Próprio por conta do Remetente;
    
*   4 - Transporte Próprio por conta do Destinatário;
    
*   9 - Sem Ocorrência de Transporte.
    

Ao acionar a marcação **"****Gera valores PIS/COFINS no EFD? (É dispensado para quem entrega EFD Contribuições)****"**, a geração dos valores de PIS/COFINS no EFD serão caracterizados, quando a empresa já realiza a entrega desses valores no EFD - Contribuições.  

Se a marcação **"****Gerar registro 1600 pelo Resumo de Operações com Cartão?****"**, estiver selecionada, o sistema utilizará os dados inseridos na tela [Resumo de Operações com Cartão](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044595154-Resumo-de-Opera%C3%A7%C3%B5es-com-Cart%C3%A3o) para tratar de forma manual as informações referentes ao Registro 1600 ao gerar o arquivo. Por outro lado, ao desabilitá-la e gerar o arquivo, o sistema não utilizará os dados da tela Resumo de Operações com Cartão.

Ao acionar a marcação **"Gerar registro C191 mesmo que o ICMS/ST esteja majorando com o FCP?"**, mesmo que o FCP esteja junto ao ICMS/ST no registro C190, os valores do FCP serão gerados neste registro.

Como mencionado acima, as seções Maior Custo para valor do item e Maior Custo para efeitos de IR serão habilitadas para uso, caso as marcações Custo para o Inventário e Custo para Inventário/Efeitos IR, respectivamente, estejam definidas com a opção Usar Maior Custo. Nestas seções, temos os seguintes tipos de custos:

*   Médio Gerencial; 
    
*   Médio com ICMS;
    
*   Médio sem ICMS;
    
*   Gerencial;
    
*   Reposição.
    

**Nota:** na geração do Registro D100, teremos os campos **"24 - COD\_MUN\_ORIG"** e **"25 - COD\_MUN\_DEST"**, onde são apresentados os Códigos Município Domicílio Fiscal preenchidos anteriormente na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades#abageral) do [Cadastro de Cidades](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110913-Cidades). Caso não exista informação, os campos serão gerados vazios.

**Observação:** ainda em relação à geração do Registro D100, para que o sistema valide a escrituração dos modelos 08 e 08B, o campo **"COD\_MOD"** deverá ser igual a 07, 09, 10, 11, 26 ou 27 e a data informada deverá ser menor que 01/01/2019.

**Nota:** no campo **"Indicador do tipo do frete"** da sub-aba D100 pode ser definida uma das opções **"Por conta do emitente"**, **"Por conta de terceiros"**, **"Sem cobrança de frete"** e **"Por conta do destinatário/remetente"** para definir o tipo de frete na emissão do CT-e.

**Nota:** para os Registros D100 e D200, será considerado na geração do arquivo o **"Modelo de Documento"** igual a **"63-Bilhete de Passagem Eletrônico"** (tela [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP), aba [Livro Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abalivrofiscal)).

**Observação:** considere ainda que, ao término da geração do livro [ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045115953-Gera%C3%A7%C3%A3o-ICMS-IPI), as informações pertinentes ao valor calculado do IPI, serão modificadas em um ajuste, ou seja, será gerado um ajuste automático do IPI; esse fato irá ocorrer caso ao menos um parceiro do livro esteja com o campo **"Enquadro no Art. 227. para cálculo de IPI?"** assinalado (localizado na aba [Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros#abafiscal) do [Cadastro de Parceiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros)) e a marcação **"Gerar linhas da Nota separadamente no Livro Fiscal?"** estiver habilitada (localizada na aba [Livros Fiscais](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abalivrosfiscais) das [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa)). Para que o crédito do IPI seja recebido, devem ser escriturados os documentos que comprovem esse benefício. Portanto, os dados serão enviados nos registros E530 e E531. No arquivo de escrituração do livro, a cada linha do E530 tem-se um ou mais registros do E531 para a geração do ajuste automático de IPI.

Com a marcação **"Gerar registro H020 do CST anterior a mudança de tributação?"** habilitada, será efetuada a geração do registro H020 demonstrando as informações de antes e depois de efetuar o processo de mudança de tributação, ou seja, será gerado o registro H020 duas vezes para o produto que teve mudança de tributação, sendo uma linha com a CST e BC e Vlr. do ICMS Normal e a segunda linha com a CST e BC e Vlr. do ICMS/ST. 

**Observação:** as marcações Gerar registro H020 do CST anterior a mudança de tributação? e Conversão CST 090 Para CST 00 na geração do registro H020 dessa aba não podem ser habilitadas de forma conjunta. Caso você tente realizar essas marcações, o sistema apresentará uma mensagem bloqueando a ação e irá salvar apenas a primeira marcação habilitada.

Quando a marcação **"Gerar registro D190 pela Escrituração Fiscal"** estiver habilitada, as informações registradas no Livro Fiscal, no formato de geração do D190, serão priorizadas. Caso contrário, as informações inseridas na [Central](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110973-Central-Compras-Vendas-Mov-Internas) serão consideradas.

[\[voltar ao subtítulo\]](#abaconfigura%C3%A7%C3%B5es)

---

#### **Sub-aba Restituição/Complementação de ST**

Nessa aba você poderá configurar as informações para o cálculo dos valores médios conforme necessário.

![aba\_restitui\_\_o.png](https://ajuda.sankhya.com.br/hc/article_attachments/8114579386647)

Insira em **"Data do inventário"** a data a qual deseja realizar a geração.

No **"Tipo de inventário"** selecione dentre as opções **"Cópia"** e **"Contagem"** o tipo do inventário que será considerado na geração dos cálculos.

Referente aos campos **"Valor do ICMS da Operação"**, **"Base de ST"**, **"Valor de ST"**, **"Valor do FCP de ST" e "Filtro Personalizado"**, configure as fórmulas que desejar para os cálculos.

Nos campos mencionados acima, você terá disposto os botões ![construtor.png](https://ajuda.sankhya.com.br/hc/article_attachments/8114610491927) **"Construtor"** e ![utilizar\_padr\_o.png](https://ajuda.sankhya.com.br/hc/article_attachments/8114672134935) **"Utilizar padrão"**, que o auxiliará na construção das fórmulas, e utilizará a fórmula padrão do sistema, respectivamente.

**Observação:** caso seja necessário realizar qualquer alteração nos campos Valor do ICMS da Operação, Base de ST, Valor de ST, Valor do FCP de ST e Filtro Personalizado, a fórmula utilizada anteriormente ficará gravada na rotina [Repositório de Arquivos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044596594) (aba Fórmula Sped, pasta EFD).

Acesse o artigo [Instruções para geração dos Registros EFD ICMS/IPI - Restituição/Ressarcimento ICMS ST Minas Gerais](https://ajuda.sankhya.com.br/hc/pt-br/articles/360057819854-Instru%C3%A7%C3%B5es-para-gera%C3%A7%C3%A3o-dos-Registros-EFD-ICMS-IPI-Restitui%C3%A7%C3%A3o-Ressarcimento-ICMS-ST-Minas-Gerais) para saber sobre as regras dispostas às empresas estabelecidas em Minas Gerais.

![essencial FINAL (1).png](https://ajuda.sankhya.com.br/hc/article_attachments/19035987846167) Caso haja uma nova inclusão e essa aba possuir preenchimento, o processo de cópia não será efetuado. 

[\[voltar ao subtítulo\]](#abaconfigura%C3%A7%C3%B5es)

---

#### **Sub-aba Prodepe**

Aqui, poderão ser efetuadas as configurações e os cálculos referente ao Benefício PRODEPE.

**Nota:** essa aba servirá para que sejam realizadas as configurações pertinentes ao Registro C177, sendo este cadastrado nas Preferências da Empresa, aba EFD - Escrituração Fiscal Digital, sub-aba **"Blocos e Registros"**.

![aba\_prodepe.png](https://ajuda.sankhya.com.br/hc/article_attachments/8114765240855)

No campo **"Indicador de enquadramento"** informe o enquadramento do registro, de acordo com as opções abaixo:

*   0-Operações não incentivadas;
    
*   1-Indústria (crédito presumido);
    
*   3-Importação (diferimento/crédito presumido);
    
*   4-Central de distribuição (entradas/saídas);
    
*   5-Comércio atacadista - sistemática especial da Lei nº 14.721/2012
    

Selecione no campo **"Indicador de Sub-Apuração"** o tipo de sub-apuração que o registro pertence.

O campo **"Cód. do Produto Sem Incentivo"** dessa aba, será preenchido com o respectivo código Prodepe referente ao Registro C177 quando no [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-), aba [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#abaimpostos%20), o campo **"Indicador Esp. Inc. PRODEPE/FUNCRESCE"** estiver com a marcação **"Sem incentivo"** selecionada.

[\[voltar ao subtítulo\]](#abaconfigura%C3%A7%C3%B5es)

---

#### **Sub-aba Sub-Apuração EFD**

Nessa aba serão demonstradas as informações referentes ao valor do saldo credor no momento da geração do EFD. Esta possui duas grades, onde uma irá representar informações sobre o saldo credor do mês anterior e a outra, sobre o mês atual.

![sub-aba\_apura\_\_o.png](https://ajuda.sankhya.com.br/hc/article_attachments/8114766546455)

[\[voltar ao subtítulo\]](#abaconfigura%C3%A7%C3%B5es)

---

#### **Sub-aba Arquivos para Registro D695**

Por meio desta aba, você poderá vincular os arquivos que as empresas que estão enquadradas no convênio 115/03 do ICMS entregam mensalmente, sendo que este arquivo alimenta os campos dos registros D695 e D696.

![aba\_apura\_\_o\_d695.png](https://ajuda.sankhya.com.br/hc/article_attachments/8114759415191)

[\[voltar ao subtítulo\]](#abaconfigura%C3%A7%C3%B5es)

#### **Demais abas da tela**

**Observação:** referente às abas **"0000"**, **"0001"**, **"B001"**, **"C001"**,  **"D001"**, **"E001"**, **"G001"**, **"H001"**, **"K001"**, **"1001"**, **"9001"** e **"9999"** dessa tela, estas estão inclusas nos registros de arquivos com base no layout disponibilizado pela Receita Federal.

Os dados referente a cada Registro poderão ser gerados pela movimentação ou de forma manual respeitando a hierarquia de seu respectivo Bloco, dessa forma, temos em cada aba os seguintes Blocos e seus registros:

*   **Aba 0000;**
    
*   **Aba 0001 -** Registros do Bloco 0 (0002, 0005, 0015, 0100, 0150, 0175, 0190, 0200, 0205, 0206, 0210, 0220, 0300, 0305, 0400, 0450, 0460, 0500 e 0600);
    
*   **Aba B001** - Registros do Bloco B (B020, B025, B420, B440, B460 e B470);
    
*   **Aba C001** - Registros do Bloco C (C100, C101, C110, C120, C130, C140, C141, C160, C170, C172, C173, C176, C177, C178, C180, C181, C185, C186, C190, C191, C195, C197, C300, C310, C320, C321, C350, C370, C390, C400, C405, C410, C420, C425, C460, C470, C490, C495, C500, C590, C591, C595, C597, C800, C850, C855, C857, C860, C890, C895 e C897);
    

**Observação:** o campo **"CNPJ ou CPF"** do Registro C800 será preenchido automaticamente com a informação contida no campo **"CNPJ/CPF"** da aba [Identificação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros#abaidentificao) do cadastro de Parceiros.

*   **Aba D001** - Registros do Bloco D (D100, D101, D110, D120, D130, D160, D161, D190, D195, D197 e D500);
    
*   **Aba E001** - Registros do Bloco E (E100, E110, E111, E115, E116, E200, E210, E220, E230, E240, E250, E300, E310, E311, E312, E313, E316, E500, E510, E520, E530 e E531);
    
*   **Aba G001** - Registros do Bloco G (G110, G125, G126, G130 e G140);
    
*   **Aba H001** - Registros do Bloco H (H005, H010, H020 e H030);
    

**Nota:** ao ligar o parâmetro **"Gerar H030 para estoque zerado? - GERH30EST0"**, os valores zerados no Registro H030 também serão gerados.

*   **Aba K001** - Registros do Bloco K (K010, K100, K200, K210, K215, K220, K230, K235, K250, K255, K260, K265, K280, K290, K291 e K292);
    

**Observação:** o Registro K010 estará disponível apenas para os exercícios de 2023, portanto, não será gerado com os demais registros do Bloco K para períodos anteriores. Além disso, este registro será gerado de acordo com o layout definido no campo **"Indicador de tipo de Layout (Registro K010)"** das [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#se%C3%A7%C3%A3oefd).

*   **Aba 1001** - Registros do Bloco 1 (1010, 1100, 1105, 1110, 1200, 1210, 1250, 1255, 1400, 1600, 1601, 1900, 1910, 1920, 1921, 1922, 1923, 1925, 1926, 1960, 1970, 1975 e 1980);
    
*   **Aba 9001** - Registros do Bloco 9 (9900);
    
*   **Aba 9999** - Registro 9999.
    

**Nota:** para a geração do Registro 1960, o benefício cadastrado desse registro deve possuir a opção **"1-Indústria (crédito presumido)"** do campo **"Indicador de Enquadramento"** da tela [Cadastro Incentivos Fiscais/Financeiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360052979134-Cadastro-Incentivos-Fiscais-Financeiros) selecionado.

![acesse também FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16310089141399) Acesse os artigos abaixo para conferir as configurações necessárias para gerar os Registros 1970 e 1980:

*   [Saiba como gerar o registro 1970 no EFD ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/12262170274711-Saiba-como-gerar-o-registro-1970-no-EFD-ICMS-IPI)
    
*   [Saiba como gerar o registro 1980 no EFD ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/12267173392919-Saiba-como-gerar-o-registro-1980-no-EFD-ICMS-IPI-)
    

**Observação:** para considerar os cálculos de médias diárias de impostos de ICMS/ST na tela [Consultar a Média Diária dos Impostos ICMS/ST](https://ajuda.sankhya.com.br/hc/pt-br/articles/7053152322839) dos registros H005, H010 e H030, deve-se realizar as seguintes ações. Observe: 

*   Preencha os campos da sub-aba Restituição/Complementação de ST presentes na aba Configurações da tela EFD - Fiscal ICMS/IPI e clique no botão ![Botão\_Processar\_FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/18048121729687) **"Processar"** e, em seguida ![gerar EFD. FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/18048154044439) **"Gerar"** para que seja gerado o arquivo txt com os registros.
    
*   Após isso, com exceção da aba H001 que contém os dados para os registros H010, H030 e H990, exclua os registros da sub-aba C100 e sub-aba **"1250"** (aba **"1001"**) da tela EFD - Fiscal ICMS/IPI.
    

[\[voltar ao topo\]](#top)

#### **Botões da tela**

No topo da tela, temos alguns botões de extrema importância para a geração do arquivo EFD. Observe:

O botão ![Botão remover FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/18920037631127) **"Excluir"** deleta um registro de cada vez, ou seja, não permite a exclusão múltipla de registros.

Ao acionar o botão ![processar.png](https://ajuda.sankhya.com.br/hc/article_attachments/7266438182423) **"Processar"**, o sistema realizará a geração e preenchimento das abas referentes aos registros do arquivo de Escrituração conforme as condições estabelecidas nas abas Parâmetros e Opções dessa tela.

![efd\_5.png](https://ajuda.sankhya.com.br/hc/article_attachments/7266636117527)

**Nota:** após o processamento de um período do arquivo, caso seja necessário alterar alguma configuração no registro, para que o sistema salve essas modificações processe novamente o registro por meio do botão Processar. 

**Nota:** ao processar os Registros C111, E112, E116, E230, E250, E312, E316, 1922 e 1926 selecionando períodos até 2022, o campo **"Número do processo"** só comporta até 15 caracteres. Quando o período for igual ou maior que 2023, este campo suportará até 60 caracteres.

Caso houver uma ou mais divergências de escrituração no período da geração informado, uma mensagem será exibida o questionando se deseja ou não visualizá-las, se sim, o sistema será direcionado a tela [Divergências de Escrituração](https://ajuda.sankhya.com.br/hc/pt-br/articles/15370034234775) para as devidas análises. Lembre-se ainda que, para a exibição da referida mensagem, a marcação **"Verificar divergências?"** da aba [Parâmetros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045115953-Gera%C3%A7%C3%A3o-ICMS-IPI#abaparmetros) (tela [Geração ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045115953-Gera%C3%A7%C3%A3o-ICMS-IPI)) deve ser habilitada. 

O botão ![gerar.png](https://ajuda.sankhya.com.br/hc/article_attachments/7266655626519) **"Gerar"**, realizará a geração do arquivo de Escrituração conforme as abas Parâmetros e Opções.

**Observação:** ao gerar os registros C100, C460, C500, C800, D100 e D500 selecionando uma **"****Data Referência"** igual ou superior a **01/01/2023**, as movimentações que estiverem com as situações de documento com os códigos abaixo, não serão apresentadas no arquivo TXT:

*    04 - NF-e, NFC-e ou CT-e - Denegado;
    
*    05 - NF-e, NFC-e ou CT-e - Numeração inutilizada.
    

Por meio do botão ![efd\_6.png](https://ajuda.sankhya.com.br/hc/article_attachments/7266729462679) **"Histórico de Gerações"**, o histórico das gerações de arquivo realizadas serão visualizadas; ao acioná-lo, o pop-up **"Processos"** será exibido na tela:

![efd\_7.png](https://ajuda.sankhya.com.br/hc/article_attachments/7266750423191)

Após informar algum dos dados necessários para pesquisa, ao clicar em **"Consultar"**, podem ser retornados os seguintes resultados:

*   Nota não existe no sistema;
    
*   Nota encontrada nos livros;
    
*   Nota não encontrada nos livros, mas existe no sistema;
    
*   Nota não encontrada nos livros, mas existe como cancelada.
    

[\[voltar ao topo\]](#top)

#### **Geração dos registros 0450, C110 e C113**

Para geração dos registros 0450, C110 e C113, atente-se para os seguintes detalhes:

Nas Preferências da Empresa, aba EFD - Escrituração Fiscal Digital, selecione no campo Tipo de Escrituração a opção **"EFD"**.

Nos painéis **"Blocos"** e **"Registros"**, teremos:

*   No painel Blocos, selecione o **"Bloco 0"**;
    
*   Realize a seleção do registro **"0450"** e faça a marcação da opção **"Gerar Registro"** no painel  Registros;
    
*   No painel Blocos, selecione o **"Bloco C"**;
    
*   Por último, no painel Registros, seleciona-se o registro **"C110"** ou **"C113"**, marcando as opções **"Gerar Registro"**, **"Gerar Entrada"** ou **"Gerar Saída"**.
    

Uma vez que os blocos foram configurados nas Preferências da Empresa, são requisitos para a geração dos registros:

*   A  nota possuir uma Observação Padrão (tela [Observações para Notas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044596474)) informada;
    
*    Na configuração da Observação Padrão, o campo Geração no EFD deve estar assinalado com a opção **"Informação Complementar do Documento Fiscal"**;
    
*   Caso seja necessário que o conteúdo do campo 03-TXT\_COMPL do registro C110 seja preenchido, é preciso marcar a opção Carrega Complemento p/EFD na configuração da Observação Padrão;
    
*   O [Tipo de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP) utilizado no lançamento do documento, deve possuir em sua configuração, a marcação **"Buscar NF de origem p/ referenciar"** realizada na aba [NF-e/NFC-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abanfe/nfce);
    
*   O Tipo de Operação - TOP utilizado no lançamento do documento de origem a ser gerado no registro C113 deve estar com o campo **"Atualização de Livro ICMS"** da aba [Livros fiscais](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abalivrofiscal) devidamente definido, ou seja, deve atualizar o livro correto.
    

Realizadas as configurações acima, automaticamente o sistema realizará a geração dos registros 0450 e C110. O registro C113 será gerado apenas quando a nota estiver vinculada a sua origem; por exemplo, nota de devolução de compra vinculada a nota de compra, nota de retorno vinculada a nota de remessa ou nota de acompanhamento de cupom vinculada ao cupom fiscal.

**Importante:** o registro C113 é filho do registro C110 que por sua vez é filho do registro 0450, portanto, para gerar o C113 é preciso gerar o C110 e para gerar o C110 é preciso gerar o registro 0450.

**Observação:** na geração do Registro C100, campo 07 os **"Modelos de Documento"** da tela Tipos de Operação - TOP, aba Livro Fiscal, as opções **"55 - Nota Fiscal Eletrônica"** e **"65 - Nota Fiscal de Venda a consumidor"**, serão gerados com três casas decimais complementados com zeros à esquerda quando informado menos de três casas decimais. Para os demais Modelos de Documento previstos no registro, a série será informada conforme consta no lançamento, em que, você poderá inserir até três casas decimais.

**Nota:** quando o parâmetro **"Gerar os reg. C100 e C190 no SPED com os valores de ST? - GERARREGSPED"** estiver ligado, os valores dos campos (23) **"VL\_BC\_ICMS\_ST"** e (24) **"VL\_ICMS\_ST"** do Registro C100 e (08) **"VL\_BC\_ICMS\_ST"** e (09) **"VL\_ICMS\_ST"** do registro C190, não serão considerados na somatória do registro **"E210"** quando houver a utilização dos CFOP's 1949 e 2949, visto que, os campos não serão validados devido à restrição de CFOP. E caso esteja desligado e o CFOP for fora do estado da empresa geradora do EFD, é necessário que este esteja com a **"Inscrição Estadual"** do Substituto Tributário cadastrado nas [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa), aba [Insc. Estadual Contribuinte ST no Estado Dest.](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abainsc.estadualcontribuintestnoestadodest.).

**Nota:** no parâmetro **"UF que soma valor não apropriado ao VLRMERC (EFD) - UFEFDVLMERC"** adicione a UF da empresa no campo **"Texto"** para gerar o arquivo sped do registro C100, assim o sistema somará os valores do IPI e ICMS-ST ao valor da mercadoria.

[\[voltar ao topo\]](#top)

#### **Registro C173**

Para que o Preço Máximo ao Consumidor (PMC) ou Preço de Fábrica (PF) sejam gerados corretamente no Registro C173 da EFD ICMS/IPI, é necessário que você realize as configurações abaixo: 

1.  Cadastre as Tabelas de Preço PMC e PF para Estados diferentes;
2.  Informe na tela de [Estados](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601294-Estados), aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601294-Estados#abageral) as tabelas que foram cadastradas. Sendo que, no campo **"Tabela de Preço PMC"** deve ser inserida a tabela que representará o Preço Máximo do Consumidor, e no campo **"Tabela de Preço PF"** insira o código da tabela de Preço de Fábrica.

Realizadas as configurações acima, o sistema validará as tabelas da seguinte forma:

*   Na UF de Destino, valida se o produto medicamento consta na tabela PMC com data de vigor menor ou igual à data do documento; se sim e o preço for maior do que zero, assumirá esse valor para o preenchimento do campo 08 do Registro C173; se não, passa para a validação abaixo.
*   Na UF de Destino, verifica se o produto medicamento consta na tabela PF com data de vigor menor ou igual à data do documento; se sim e o preço for maior do que zero, utilizará esse valor para o preenchimento do campo 08 do Registro C173; se o produto não estiver cadastrado em nenhuma das duas tabelas (PMC e PF), o sistema retornará uma mensagem informando que o valor do preço máximo não foi encontrado no momento da geração do arquivo.

**Observação:** se os campos Tabela de Preço PMC e Tabela de Preço PF da tela Estados, aba Geral não estiverem preenchidos, o sistema validará a tabela configurada no parâmetro **"Tabela de Preço PMC - CODTABPMC"** para gerar o Registro.

**Importante:** caso não haja nenhuma das configurações acima (nos campos e parâmetro), o Registro C173 não será gerado.

Se os campos Tabela Preço PMC e Tabela Preço PF forem configurados de forma inadequada, teremos os seguintes comportamentos:

*   Caso os campos estiverem preenchidos mas o Produto não for encontrado em nenhuma das tabelas, será exibida a mensagem _**"Nota de número único: ? Tabela Preço PMC: ? ou Tabela Preço PF: ? do cadastro de Estados Produto: ? Local: ? Controle: ? Valor do preço máximo não foi encontrado."**_.
*   Considerando que se esteja utilizando o parâmetro CODTABPMC para tal operação, se o produto não for encontrado na tabela ali informada, a seguinte mensagem é apresentada: _**"Nota de número único: ? Parâmetro CODTABPMC: ? Produto: ? Local: ? Controle: ? Valor do preço máximo não foi encontrado."**_. 

[\[voltar ao topo\]](#top)

#### **Registro C177**

Para garantir que o sistema processe corretamente os registros fiscais vinculados ao PRODEPE, siga as etapas abaixo:

#### **Configuração da empresa**

1.  Acesse **Comercial » Preferências »** [**Empresa**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa).
2.  Na aba [**EFD - Escrituração Fiscal Digital**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaefdescrituraofiscaldigital), sub-aba **Bloco e Registro**, ative a geração do **Registro C177**.
3.  Ainda em **nessa tela**, acesse a aba [**Livros Fiscais**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abalivrosfiscais) e marque a opção **"Beneficiário de Incentivo PRODEPE/FUNCRESCE?"**.

#### **Cadastro de incentivos fiscais**

1.  Acesse **Livros Fiscais » Arquivo »** [**Cadastros Incentivos Fiscais/Financeiros**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360052979134-Cadastro-Incentivos-Fiscais-Financeiros).
2.  Cadastre o incentivo fiscal e vincule-o à empresa responsável pela nota fiscal.

#### **Configuração de produtos**

1.  Acesse **Configurações » Cadastros »** [**Produtos**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos).
2.  Nos campos **"Cód. Apur. Inc. PRODEPE/FUNCRESCE"** e **"Indicador Esp. Inc. PRODEPE/FUNCRESCE"**, selecione **"Com Incentivos"**.

#### **Definição de CFOP**

1.  Acesse **Comercial » Arquivo » Cadastros »** [**CFOP**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044600714-CFOP).
2.  No CFOP utilizado no lançamento da nota, marque o campo **"Tipo de Operação PRODEPE"** como **"Operação Incentivada"**.

#### **Configuração de parceiros**

1.  Acesse **Configurações » Cadastros »** [**Parceiros**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros).
2.  Na aba [**Fiscal**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros#abafiscal), a opção **"Parceiro elegível à inaplicabilidade do PRODEPE?"** deve estar desmarcada, pois se habilitada as movimentações com o Parceiro não serão consideradas.  
     

#### **Validação da configuração**

Após concluir as configurações, siga os passos abaixo para validar se o sistema está gerando corretamente os registros fiscais:

#### **Lançamento da nota fiscal**

1.  Acesse **Comercial » Consulta »** [**Portal de Compras**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045111953-Portal-de-Compras).
2.  Lance uma **nota fiscal de compra** vinculada à empresa configurada anteriormente.

#### **Geração do livro fiscal**

1.  Acesse **Livros Fiscais » Arquivos »** [**Geração ICMS/IPI**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045115953-Gera%C3%A7%C3%A3o-ICMS-IPI).
2.  Gere a nota fiscal lançada anteriormente no **Livro Fiscal**.

#### **Processamento no EFD Fiscal ICMS/IPI**

1.  Acesse **Livros Fiscais » Conexão » EFD - Fiscal ICMS/IPI**.
2.  **Processe a referência da nota fiscal**.

#### **Verificação do resultado esperado**

*   O sistema deverá gerar o **Bloco C**, incluindo os registros de detalhamento do item.
*   O **Registro C177** deve ser gerado com o valor fixo **PE000100** no **campo 2**.
*   Ao exportar o arquivo texto, o sistema deverá conter a linha correspondente ao **Registro C177**, com a estrutura:

```auto
|C177|PE000100|
```

[\[voltar ao topo\]](#top)

#### **Registro C180**

Para gerar as informações do Número do Documento de Arrecadação e o Código do Modelo de Documento de Arrecadação, nos campos 10 - COD\_DA e 11 - NUM\_DA do registro C180 do Sped Fiscal, é necessário que você tenha notas de compras lançadas no [Portal de Compras](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603174-Portal-de-Compras-Atributos-da-Tela), com os campos **"Número do Documento de arrecadação"** e **"Cód. Mód. Documento de arrecadação"** do cabeçalho ou item da nota preenchidos:

![1.png](https://ajuda.sankhya.com.br/hc/article_attachments/7266738673303)

 **![informações adicionais FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16310089145751)****Informações adicionais:**

*   Se a opção **"GNRE"** do campo Cód. Mod. Documento de arrecadação esteja selecionada, será gerado valor 1 no campo 10 do registro C180; e, caso a opção **"Documento Estadual de Arrecadação"** esteja selecionada, será gerado valor 0 no campo 10.
*   Os referidos campos estão disponíveis no cabeçalho e item da nota, dessa forma, a regra a ser seguida é:

1.  Se forem preenchidos os campos do Item da nota, torna-se prioritária em relação ao cabeçalho.
2.  Se ambos estiverem vazios, será gerado **<Vazio>** nos campos 10 - COD\_DA e 11 - NUM\_DA do registro C180.

*   Para o campo 11 - NUM\_DA não é estabelecido quantidade de caracteres, sendo assim, será considerado o tamanho padrão do campo do cabeçalho.
*   Se um dos campos estiver preenchido, o outro também deverá estar.

Em casos de ressarcimento de ST, para que o sistema gere o registro H010 quando houver a geração do registro C180, deve-se efetuar as seguintes configurações:

1- No [Cadastro de Produto](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-), aba [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#abaimpostosinformaesporempresa) / [Informações por empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#abaimpostosinformaesporempresa), o campo **"Tipo de substituição"** não pode estar configurado com as opções **"Não tem"** ou **"Venda com Substituição Tributária (ST na Venda)"**.

2- É necessário que o item esteja incluído no inventário mesmo quando a quantidade dele for zero. Para que o sistema gere e considere a quantidade 0, o parâmetro **"Gerar H030 para estoque zerado? - GERH30EST0"** deve estar ligado.

3- Por fim, as marcações **"Ignorar filtro padrão"** e **"Recalcula Inventario"** localizadas na aba de [Configurações](https://ajuda.sankhya.com.br/hc/pt-br/articles/7267044122263#abaconfigura%C3%A7%C3%B5es), sub-aba [Restituição/Complementação de ST](https://ajuda.sankhya.com.br/hc/pt-br/articles/7267044122263#sub-abaRestitui%C3%A7%C3%A3o/Complementa%C3%A7%C3%A3odeST), poderão ser utilizadas conforme a necessidade.

[\[voltar ao topo\]](#top)

#### **Indicador de Frete no registro D100**

O sistema utiliza o tomador do serviço de frete e o valor do frete para preencher o campo **"Indicador do tipo do frete"** (17 - INS\_FRT) no registro D100 (aba **"D001"**), de acordo com as diretrizes do Manual do Layout 1.05 / Código 006 do Sped Fiscal para os modelos de CT-e 57 e 67, sendo eles:

<table style="border-collapse: collapse;"><tbody><tr style="height: 23px;"><td class="wysiwyg-text-align-justify" style="height: 23px; width: 100%;" colspan="2"><strong>&nbsp;Indicador do tipo do frete no layout 1.05/Código 006 do Sped Fiscal</strong></td></tr><tr style="height: 22px;"><td style="height: 22px; width: 8.42857%;">&nbsp;0</td><td style="height: 22px; width: 91.5714%;">&nbsp;Por conta do emitente</td></tr><tr style="height: 22px;"><td style="height: 22px; width: 8.42857%;">&nbsp;1</td><td style="height: 22px; width: 91.5714%;">&nbsp;Por conta do destinatário/remetente</td></tr><tr style="height: 22px;"><td style="height: 22px; width: 8.42857%;">&nbsp;2</td><td style="height: 22px; width: 91.5714%;">&nbsp;Por conta de terceiros</td></tr><tr style="height: 22px;"><td style="height: 22px; width: 8.42857%;">&nbsp;9</td><td style="height: 22px; width: 91.5714%;">&nbsp;Sem cobrança de frete</td></tr></tbody></table>

Para isso, haverá as seguintes validações:

 **![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28201800542999) Lançamento do CT-e (modelo 57 e 67) pela** [**Movimentação Financeira**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114753-Movimenta%C3%A7%C3%A3o-Financeira)**:**

*   Sempre que o frete for registrado pela Movimentação Financeira e o tomador do frete for a empresa, com valor superior a zero, o Indicador de Frete será automaticamente configurado como "**Por conta do destinatário/remetente"**.
    

 **![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28201800542999) Lançamento do CT-e (modelo 57 e 67) pelo** [**Portal de Compras**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045111953-Portal-de-Compras)**:**

*   No Portal de Compras, o comportamento é semelhante ao anterior, sendo que quando o tomador do frete for a empresa e o valor do frete for maior que zero, o sistema utilizará a opção Por conta do destinatário/remetente como Indicador de Frete.
    

 **![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28201800542999) Lançamento do CT-e (modelo 57 e 67) pelo** [**Portal de Vendas**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612654-Portal-de-Vendas)**:**

*   Se o valor do campo **"Vlr. Nota"** da [Central de Vendas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612414-Central-de-Vendas), for zero, o Indicador de Frete será preenchido com a opção **“Sem cobrança de frete”**, independente de quem seja o tomador;
    
*   No entanto, se o valor informado no campo Vlr. Nota for maior que zero e os campos **"Parceiro"** (tomador) e **"Parceiro Destinatário"** na grade [Cabeçalho](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612414-Central-de-Vendas#gradecabealho) na Central de Vendas, forem iguais, o Indicador de Frete será a opção Por conta do destinatário/remetente;
    
*   Ainda, se o valor informado no campo Vlr. Nota for maior que zero e os campos Parceiro (tomador) e **"Parceiro Remetente"** forem iguais, o Indicador de Frete também será Por conta do destinatário/remetente;
    
*   Caso o valor informado no campo Vlr. Nota for maior que zero e os dados (CNPJ e Inscrição Estadual) do parceiro informado no campo Parceiro (tomador) forem iguais aos dados preenchidos no campo **"Empresa"** (emitente) da Central de Vendas, o Indicador de Frete será **“Por conta do emitente”**.
    
*   Por fim, se o valor informado no campo Vlr. Nota for maior que zero e o campo Parceiro (tomador) for diferente dos campos Parceiro Destinatário, Parceiro Remetente e Empresa, o Indicador de Frete será **“Por conta de terceiros”**; 
    

**Importante:** para os casos descritos, não é necessário configurar manualmente o Indicador de Frete. Após realizar os lançamentos, basta gerar o Livro ICMS/IPI e a EFD - Fiscal ICMS/IPI.

[\[voltar ao topo\]](#top)

#### **Geração da Conta Contábil para o registro H010**

Observe abaixo, as configurações necessárias para geração da Conta Contábil para o registro do inventário H010:

1\. Primeiramente, temos três parâmetros que influenciam a geração do registro H010 do EFD, são eles:

*   Conta p/inventário (H010) do EFD (SPED FISCAL) - EFDH010;
    
*   Conta p/inventário Prop. c/ Terc (H010) do EFD - EFDH010\_PRTER;
    
*   Conta p/inventário Terceiro (H010) do EFD - EFDH010\_TER.
    

Nesses parâmetros, informe contas contábeis fixas para o inventário; sendo que, a informação incluída nos parâmetros será utilizada para geração do Campo 10 (Conta Contábil) do EFD Registro H010.

Caso uma conta contábil fixa não seja inserida, poderão ser informados valores especiais, de forma que o sistema irá localizar a Conta Contábil conforme as regras abaixo:

No [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Produtos-), aba [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#abaimpostos), há uma hierarquia de contas que o sistema irá buscar, sendo elas:

*   Conta Contábil 1 - O sistema busca a conta contábil 1;
    
*   Conta Contábil 2 - O sistema utiliza a conta contábil 2;
    
*   Conta Contábil 3 - O sistema emprega a conta contábil 3;
    
*   Conta Contábil 4 - O sistema procura a conta contábil 4.
    

Assim, o sistema utilizará uma dessas quatro contas contábeis informadas.

2. Logo abaixo, temos a configuração para informar a Conta Contábil que será gerada no H010 para empresas diferentes, sendo que, será aplicada às empresas que geram o registro H010 com Plano de Contas diferentes. Assim, temos os seguintes campos na tela Preferências da Empresa, aba EFD - Escrituração Fiscal Digital:

*   **Conta p/inventário (H010) do EFD (SPED FISCAL) -** Mesma funcionalidade do parâmetro Conta p/inventário (H010) do EFD (SPED FISCAL) - EFDH010;
    
*   **Conta p/inventário Prop. c/ Terc (H010) do EFD -** Mesma funcionalidade do parâmetro Conta p/inventário Terceiro (H010) do EFD - EFDH010\_TER;
    
*   **Conta p/inventário Terceiro (H010) do EFD -** Mesma funcionalidade do parâmetro Conta p/inventário Prop. c/ Terc (H010) do EFD - EFDH010\_PRTER.
    

3. Por último, ao realizar a geração do bloco H010, registro 010 (COD\_CTA), o sistema efetuará as seguintes verificações para preencher o campo do respectivo registro:

Primeiramente, será analisado nas Preferências da Empresa, [aba EFD - Escrituração Fiscal Digital](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaefdescrituraofiscaldigital), se aquele item para a empresa que está sendo gerada o SPED, há alguma configuração para os campos:

*   Conta p/inventário (H010) do EFD (SPED FISCAL);
    
*   Conta p/inventário Prop. c/ Terc (H010) do EFD;
    
*   Conta p/inventário Terceiro (H010) do EFD.
    

Se algum dos campos estiver definido, seu conteúdo será utilizado para alimentar a conta contábil. Caso não exista, serão utilizadas as configurações dos parâmetros Conta p/inventário (H010) do EFD (SPED FISCAL) - EFDH010, Conta p/inventário Prop. c/ Terc (H010) do EFD - EFDH010\_PRTER - EFDH010\_PRTER e Conta p/inventário Terceiro (H010) do EFD - EFDH010\_TER mencionados acima.

[\[voltar ao topo\]](#top)

#### **Registros 0300 e G125**

Quando a marcação **"Gerar CIAP de componentes para SPED"** nas [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa), aba [Bens](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#ababens) estiver realizada, o sistema irá gerar o Registro 0300 considerando o preenchimento do campo 05 (COD\_PRNC) e o vinculando a um bem principal, gerando assim, um Registro 0300 para o bem principal e, por fim, preenchendo o campo 03 (IDENT\_MERC) com a opção **"2 - componente"**.

**Observação:** para o Registro G125, o parâmetro **"Utiliza TIPOENTCIAP para geração do SPED - TIPOENTCIAPSPED"** já leva o EFD para todos os produtos, independentemente se são bens ou componentes, conforme a opção marcada no campo **"Tipo de Movimentação do Bem ou Componente"** da aba [Bens](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#ababens) do [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-).

Ao fazer o cadastro de um componente ou bem, marcando a opção **"IA-Imobilização em Andamento - Componente"**, o sistema levará esse código para o EFD. Assim, após processar o EFD na tela EFD - Fiscal ICMS/IPI, será possível validar que o campo 05 (COD\_PRNC) está vinculado a um bem principal e demonstrado nele, bem como verificar a marcação correta do campo 03 (IDENT\_MERC) sendo um componente, uma vez que está vinculado a um bem principal. 

Além disso, ao ativar o parâmetro **“UFs que consideram devoluções de venda no CIAP - UFCONSDEVCIAP”**, o sistema identifica automaticamente quais estados devem considerar as devoluções de venda no cálculo do índice de crédito de ICMS no CIAP.

#### **Configuração do Parâmetro**

*   Na tela [Preferências](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601834-Prefer%C3%AAncias).
*   No campo de valor, insira as **UFs separadas por vírgula** (exemplo: **RS, MG, RJ**).
*   Utilize as configurações disponíveis na [Melhores Práticas - Configuração e Cálculo do CIAP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044580254-Melhores-Pr%C3%A1ticas-Configura%C3%A7%C3%A3o-e-C%C3%A1lculo-do-CIAP).

#### **Regras de Aplicação**

*   Se a empresa estiver localizada em uma das UFs configuradas, **as devoluções de venda serão consideradas no cálculo do índice de crédito de ICMS**.
*   Os valores das devoluções serão automaticamente **subtraídos das colunas**:
    *   **Tributadas e Exportação**, quando aplicável.
    *   **Total de Saídas**, conforme as configurações do sistema.

#### **Impacto na Geração do Bloco G**

*   Os registros do **Bloco G do EFD ICMS/IPI** serão ajustados para refletir corretamente os totais de tributadas e exportação e totais de saída considerando as devoluções de venda, garantindo conformidade com as exigências fiscais.

#### **Composição da Receita Bruta para o Bloco G (CIAP)**

**O que faz:** Define quais valores de saída compõem o cálculo do índice de apropriação do ICMS no Bloco G. **Como funciona:** Para calcular o valor total das saídas e o índice de crédito, o sistema busca a configuração no [**Cadastro de CFOP**](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044600714-CFOP), seguindo esta hierarquia:

1.  **Receita Bruta p/ CIAP:** é o campo prioritário. Utilize-o para garantir que o valor componha o Bloco G sem afetar outras obrigações.
2.  **Receita Bruta p/ EFD Contribuições:** caso o campo anterior esteja vazio, o sistema utiliza este como _fallback_ (contingência).

> **Importante:**
> 
> **Independência Fiscal:** 
> 
> A configuração do campo **Receita Bruta p/ CIAP** não impacta o evento R-2060 da EFD-Reinf. Isso permite que você configure um CFOP para "Somar" no CIAP e "Não Afetar" na CPRB, eliminando conflitos de apuração.

[\[voltar ao topo\]](#top)

#### **Geração do registro 1400**

Na geração do Registro 1400 para o município do fator gerador, quando o documento utilizado para compor tal informação for um [CT-e](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044596834), o município a ser considerado será o de origem do CT-e. Considerando todas as situações de geração do município do registro 1400, este será gerado somente quando ele fizer parte do estado da empresa geradora do EFD, por exemplo, se uma empresa estabelecida no estado de Minas Gerais prestar serviço de transporte começando no próprio estado de Minas, este documento irá compor o registro 1400; porém, caso a mesma empresa inicie o serviço de transporte no estado de São Paulo, o documento não irá integrar o registro 1400.

#### Regras para a Geração do registro 1400:

*   A nota deverá ter sido inserida no Registro C100;
    
*   Os parâmetros **"CFOPs que geram Não Dedutíveis no registro 1400 - CFOPNAODED1400"**, **"UFs que geram Não Dedutíveis no registro 1400 - UFSNAODED1400"** e **"UFs que geram NF-e de Venda no registro 1400 - UFSVENREG1400"** deverão estar configurados com as devidas UFs e CFOPs;
    
*   A nota deverá possuir o **"Modelo de Documento"** igual a **"55-Nota Fiscal Eletrônica"** na tela [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP), aba [Livro Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abalivrofiscal);
    
*   A nota deve tratar-se de uma saída, possuir o **"Tipo de Movimento"** igual a **"P-Pedido de venda"** ou **"V-Venda"** e apresentar o valor de frete igual a zero;
    
*   Além disso, a nota deverá estar com o campo **"Indicador de Presença para NF-e/NFC-e"** (tela Tipos de Operação - TOP, aba NF-e/NFC-e) com uma das opções **"0-Não se aplica"**, **"1-Operação presencial"** ou **"5-Presencial, fora do estabelecimento"** selecionada;
    
*   Além disso, ainda na tela Tipos de Operação - Top, na aba Livro Fiscal, a marcação **"Gerar Registro 1400 no SPED Fiscal ?"** deverá estar acionada.
    

**Observação:** a tela [Códigos de itens (IPM) por UF no registro 1400](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116093-C%C3%B3digos-de-itens-IPM-por-UF-no-registro-1400) também deverá ter seu devido registro para que o correto funcionamento do registro ocorra. Sendo ainda que, para que seja impresso no registro 1400 o Código do Item, você também precisará efetuar os cadastros das abas [Grupo de Produto, Produto e Tipos de Operação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116093-C%C3%B3digos-de-itens-IPM-por-UF-no-registro-1400#abasgrupodeprodutoprodutoetiposdeoperao) da mesma tela.

**Observação:** insira no parâmetro **"UFs com cód.IBGE parceiro fornecedor p/ reg.1400 - IBGEPARC1400"** as UFs que serão utilizadas, para que, na geração do registro 1400, seja considerado o código do município do Parceiro. Sendo que, o parâmetro citado serve para amparar a regra DIPAM do estado de SP e/ou outras UFs, se necessário.

**Nota:** ao incluir o modelo 04 (NF Produtor Rural) na geração do Registro 1400, o município do Parceiro também será gerado, assim como nos modelos 01, 1A, 1B, 55 e 65. Dessa forma, este deve possuir as seguintes configurações:

*   Empresa do estado de SP;
    
*   Parceiro do estado de SP (não pode possuir inscrição estadual);
    
*   Nota de entrada nos modelos 01, 1A, 55 ou 65;
    
*   O Parceiro deve ser do mesmo estado da empresa e a UF deve ser preenchida no parâmetro.
    

[\[voltar ao topo\]](#top)

#### **Geração do registro 0205**

A geração do Registro 0205 deve ocorrer no mês em que a alteração da descrição do produto foi realizada, desde que haja movimentação do produto nesse período. Se não houver movimentação no mês da alteração, o Registro 0205 será gerado no primeiro período subsequente em que houver movimentação do produto.

[\[voltar ao topo\]](#top)

#### **Geração do registro 0221**

Observe abaixo as configurações necessárias para a geração do registro 0221 do SPED Fiscal para produtos classificados como mercadoria para revenda, sejam eles kits/cestas ou produtos comercializados individualmente:

*   Cadastre o registro 0221 nas [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa), aba [EFD - Escrituração Fiscal Digital](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaefdescrituraofiscaldigital), com o tipo de escrituração igual a EFD no bloco 0;
*   Verifique no [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos), aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos#abageral), se o produto está classificado como **"Mercadoria para Revenda"** no campo **"Tipo do Item/Sped"** ou como **"Revenda"** no campo **"Usado como"**;
*   Caso o produto seja relacionado a um kit ou cesta, é fundamental vincular seus componentes através da aba [Componentes](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos#abacomponentes), no Cadastro de Produtos, indicando a quantidade de cada componente;
*   Após a configuração será possível realizar a geração do registro 0221 do SPED Fiscal na tela EFD - Fiscal ICMS/IPI, acessando a aba 0001 e em seguida sub-aba 0200.

**Observação:** este registro não engloba produtos semelhantes com códigos de produto diferente, ou seja, caso exista dois produtos semelhantes com cadastros ou códigos de produtos diverso o sistema não realizará a geração do registro 0221 correlacionando esses dois produtos.

Se um produto for lançado em duas notas no mesmo mês, e cada nota possuir um preenchimento diferente no campo **"Cód. Produto p/ NF-e/NFC-e/CF-e"** da seção **"NF-E"**, na aba [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos#abaimpostos) do [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos) (uma como **"Código do Produto"** e a outra como **"Referência"**), ao processar o SPED Fiscal, serão gerados os registros 0200 e 0221 para esse produto.

Em um deles, o **"Cód. Item"** e o **"Código do Item Atômico"**, na tela do respectivo registro, serão preenchidos com o Código do Produto, e no outro, com o código da Referência.

**Observação:** caso o produto seja classificado como mercadoria para revenda, atráves da aba Geral ou da aba Impostos e o campo Cód. Produto p/ NF-e/NFC-e/CF-e seja configurado como Referência, mas o campo **“Referência”** da aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos#abageral) esteja sem preenchimento, a seguinte mensagem será exibida ao tentar gerar o SPED Fiscal:

_**"O produto XXX está com o campo "Referência" sem preenchimento."**_

Além disso, é possível configurar a geração do registro 0221 do SPED Fiscal para produtos com configuração por Empresa, utilizando somente a aba Impostos/Informações por empresa da tela Cadastro de Produtos, por meio de uma das seguintes opções:

*   Na referida aba, configure a empresa como **"Mercadoria para Revenda"** no campo Tipo do item p/ SPED da sub-aba Geral, ou;
*   Configure o campo Tipo do item p/ SPED como **"Utilizar do 'Uso do Produto'"** e, no campo **"Uso do Produto"**, defina como **"Revenda”**.

Utilizando uma das opções de configuração por Empresa mencionadas acima, ao gerar o arquivo, o sistema considerará as informações preenchidas nesta aba, desconsiderando o que estiver configurado na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos#abageral) nos campos Tipo do item p/ SPED e **"Usado como”**.

[\[voltar ao topo\]](#top)

#### **Registros do Bloco K**

O Bloco K é uma parte do SPED Fiscal que contém informações para controle da produção e dos estoques.

Assim, o Registro K280, refere-se à Correção de Apontamento do K200, de forma que, o mesmo ajustará o que foi enviado no Registro K200, ou seja, após o cliente entregar o registro K200, realizar a contagem do estoque e verificar a necessidade de corrigir o valor enviado neste registro, emitindo assim, uma Nota de Ajuste de Estoque com as configurações abaixo devidamente realizadas, para que o Registro K280 possa ser enviado. Pensando nisso, observe um exemplo:

Foi enviado o Registro K200 no mês de dezembro/2019, porém, em janeiro/2019 constatou-se a diferença no estoque. Assim, será preciso emitir a Nota de Ajuste de Estoque corrigindo essa diferença e quando for encaminhado o SPED em fevereiro/2019, será enviado o K280 com a quantidade ajustada assim como o K200, que será enviado normalmente com o valor do período.

**Observação:** quando a Nota de Ajuste for emitida, deve-se inserir a data de ajuste do estoque, ou seja, conforme o exemplo acima, a data de dezembro deverá ser informada para que o Registro K280 seja gerado.

Conforme a explicação acima, em relação ao Ajuste de Entrada = Ajuste Positivo de Estoque Próprio realize as seguintes configurações:

*   Na TOP **"Nota de Ajuste de Entrada de Estoque"**, tela Tipos de Operação - TOP, aba [Livro Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abalivrofiscal), a marcação **"Gerar Correção de Apontamento (K280)"** deve ser acionada;
*   Na aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abageral) da tela acima mencionada, o campo **"Atualização do Estoque"** deverá configurado com a opção **"Entrar"**;
*   Na aba [Estoque de Terceiros](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abaestoquedeterceiros) da mesma tela, o campo **"Estoque com/de Terceiros"** deve possuir a opção **"Não controla"** selecionada;
*   Após realizar os ajustes acima, a Nota com as devidas entradas de produtos será criada;
*   Em seguida, faça a geração do SPED Fiscal;
*   Assim, ao abrir o arquivo gerado, pode-se notar que o registro K280 foi gerado e validado no PVA sem erros e com a quantidade de produtos positiva.

Referente ao Ajuste de Saída = Ajuste Negativo de Estoque Próprio, os seguinte ajustes deverão ser realizados:

*   Selecione a TOP **"Nota de Ajuste de Saída de Estoque"** e realize a marcação Gerar Correção de Apontamento (K280) na aba Livro Fiscal;
    
*   Na aba Geral da tela Tipos de Operação - TOP, o campo Atualização do Estoque deverá estar com a opção **"Baixar"** selecionada;
    
*   O campo Estoque com/de Terceiros localizado na aba Estoque de Terceiros também deverá possuir a opção Não controla inserida;
    
*   Posteriormente, uma nota com a saída dos produtos será criada;
    
*   Após isso, o sistema realizará geração do SPED Fiscal e você poderá observar no arquivo, a geração de uma correção negativa dos produtos.
    

Referente ao Ajuste de Entrada (positivo) ou Saída (negativo) de Estoque de Terceiro, realize as configurações da seguinte forma:

*   Assim como nos ajustes acima, a marcação Gerar Correção de Apontamento (K280) deve ser efetuada, tanto para ajuste de entrada quanto para o de saída;
    
*   O campo Atualização do Estoque necessita estar com a opção **"Nenhuma"** selecionada;
    
*   Para o Ajuste de Entrada, o campo Estoque com/de Terceiros deve possuir a opção **"Somar ao estoque próprio em poder de terceiro"** inserida e, para o Ajuste de Saída, deverá ser selecionada a opção **"Subtrair ao estoque próprio em poder de terceiro"**;
    
*   Realizadas as configurações acima, deve-se criar as notas de entrada e saída de produtos;
    
*   Assim, observe no arquivo após gerar o SPED Fiscal, a geração positiva e negativa dos produtos.
    

No que se refere ao Ajuste de Entrada ou Saída em Propriedade de Terceiro realize os ajustes abaixo:

*   Selecione a marcação Gerar Correção de Apontamento (K280);
    
*   Insira a opção Nenhuma no campo Atualização do Estoque, para ajuste de Entrada quanto para Saída);
    
*   O campo Estoque com/de Terceiros deve possuir a opção **"Somar ao estoque de terceiros em poder da empresa"** para o Ajuste de Entrada e a opção **"Subtrair ao estoque de terceiros em poder da empresa"** para o Ajuste de Saída.
    

Após isso, realize os mesmos procedimentos dos ajustes anteriormente informados.

O Registro K210 (Desmontagem de mercadorias - Item de Origem) tem o objetivo de escriturar a desmontagem de mercadorias de tipos:

*   00 – Mercadoria para revenda;
    
*   01 – Matéria-Prima;
    
*   02 – Embalagem;
    
*   03 – Produtos em Processo;
    
*   04 – Produto Acabado;
    
*   05 – Subproduto;
    
*   10 – Outros Insumos.
    

Destaca-se ainda que, a quantidade deve ser expressa, obrigatoriamente, na unidade de medida de controle de estoque constante no campo 06 do registro 0200 - UNID\_INV.

**Observação:** quando houver identificação da ordem de serviço, a chave desse registro será os campos **"COD\_DOC\_OS"** e **"COD\_ITEM\_ORI"**. Nos casos em que a ordem de serviço não for identificada, o campo chave passa a ser **"COD\_ITEM\_ORI"**.

Em relação ao Registro K215 (Desmontagem de mercadorias - Item de Destino), ele tem a finalidade de escriturar a desmontagem (com ou sem ordem de serviço) de mercadorias de tipos:

*   00 – Mercadoria para revenda;
    
*   01 – Matéria-Prima;
    
*   02 – Embalagem;
    
*   03 – Produtos em Processo;
    
*   04 – Produto Acabado;
    
*   05 – Subproduto;
    
*   10 – Outros Insumos.
    

**Nota:** o Registro K215 é obrigatório caso exista o registro-pai K210 e o controle da desmontagem não seja por ordem de serviço (campos **"DT\_INI\_OS"**, **"DT\_FIN\_OS"** e **"COD\_DOC\_OS"** do Registro K210 em branco). Nesse caso, a saída do estoque do item de origem e a entrada em estoque do item de destino tem que ocorrer no período de apuração do Registro K100.  
Quando o controle da desmontagem for por ordem de serviço, deverá existir o Registro K215 até o encerramento da ordem de serviço, que poderá ocorrer em outro período de apuração.

**Observação:** a quantidade deve ser expressa, obrigatoriamente, na unidade de medida de controle de estoque constante no campo 06 do registro 0200 - UNID\_INV.

**Nota:** a chave do Registro K215 é o campo **"COD\_ITEM\_DES"**. 

O Registro K220 (Outras movimentações internas entre mercadorias) tem o objetivo de informar a movimentação interna entre mercadorias dos seguintes tipos (indicadas no campo TIPO\_ITEM do registro 0200 e que não se enquadrem nas movimentações internas já informadas nos demais tipos de registros): 

*   00 - Mercadorias para revenda;
*   01 - Matéria Prima;
*   02 - Embalagem;
*   03 - Produtos em processo;
*   04 - Produtos Acabados;
*   05 - Subprodutos;
*   10 - Outros insumos.

**Observação:** as informações pra geração do Registro K220 serão buscadas da tela [Reclassificação do Produto](https://ajuda.sankhya.com.br/hc/pt-br/articles/6024489775895-Reclassifica%C3%A7%C3%A3o-do-Produto-). 

Os Registros K260 e K265 têm o objetivo de informar o produto que será reprocessado ou que foi reprocessado e o insumo que será reparado ou que foi reparado no período de apuração do Registro K100.

O registro K260 é definido como **"Reprocessamento/reparo de produto/insumo**" e apresenta os produtos que saíram do estoque no período de apuração para serem reprocessados, incluindo a ordem de produção/serviço, o código do produto que foi reprocessado, a data de saída do estoque, a quantidade que saiu do estoque, a data de retorno ao estoque, e a quantidade que retornou ao estoque.

Já o registro K265 é o **"Reprocessamento/reparo - Mercadorias consumidas e(ou) retornadas"** e apresenta os produtos que foram consumidos no período de apuração no reprocessamento do produto informado no K260, incluindo o código do produto, a quantidade consumida e quantidade que retornou ao estoque. 

[\[voltar ao topo\]](#top)

### **Adequação do ERP ao SPED Fiscal (EFD-ICMS/IPI) 3.1.9 e 3.2.0**

A partir de **01/01/2026**, o ERP será atualizado para gerar o **SPED Fiscal (EFD-ICMS/IPI)** em conformidade com o novo leiaute (versão 3.1.9/3.2.0) e as orientações da **Reforma Tributária do Consumo**, incluindo os tributos **CBS**, **IBS** e **IS**.

Essa atualização foca em garantir a correta escrituração, especialmente em operações interestaduais com consumidor final não contribuinte, que exigem o **registro 0150 adicional** quando há divergência de UF.

#### **1\. Atualização e Vigência do Leiaute**

Para garantir a conformidade, a tabela de controle de versões do SPED Fiscal foi atualizada:

<table class="wysiwyg-table-resized"><colgroup><col style="width: 37%;"> <col style="width: 33%;"> <col style="width: 30%;"></colgroup><tbody><tr><td style="text-align: justify;"><span style="background-color: #ffffff; color: #4d4d4d;"><strong>Detalhe</strong></span></td><td style="text-align: justify;"><span style="background-color: #ffffff; color: #4d4d4d;"><strong>Valor</strong></span></td><td style="text-align: justify;"><span style="background-color: #ffffff; color: #4d4d4d;"><strong>Vigência</strong></span></td></tr><tr><td style="text-align: justify;"><span style="background-color: #ffffff; color: #4d4d4d;"><strong>Código do Leiaute</strong></span></td><td style="text-align: justify;"><span style="background-color: #ffffff; color: #188038;">020</span></td><td style="text-align: justify;"><span style="background-color: #ffffff; color: #4d4d4d;">A partir de <strong>01/01/2026</strong></span></td></tr><tr><td style="text-align: justify;"><span style="background-color: #ffffff; color: #4d4d4d;"><strong>Versão do Leiaute</strong></span></td><td style="text-align: justify;"><span style="background-color: #ffffff; color: #188038;">1.19</span></td><td style="text-align: justify;"><span style="background-color: #ffffff; color: #4d4d4d;">A partir de <strong>01/01/2026</strong></span></td></tr></tbody></table>

O sistema selecionará automaticamente a **Versão 1.19 (Código 020)** para qualquer escrituração com data-base igual ou posterior a **01/01/2026**.

#### **2\. Ajustes em Registros**

##### **2.1. Registro C120**

O **Registro C120** (localizado no caminho C001 > C100 > C120) sofreu uma atualização em seu campo de identificação.

*   **Campo Atualizado:** Campo 02
*   **Novo Valor Válido Adicionado:** **2**

O sistema foi devidamente ajustado para **permitir, validar e exportar** este novo valor no domínio do campo 02 do Registro C120.

##### **2.2. Considerações para a Escrituração de Novos Tributos (CBS, IBS e IS)**

A **EFD ICMS/IPI** **não** deve ser utilizada para a apuração dos novos tributos (CBS, IBS e IS - Contribuição sobre Bens e Serviços, Imposto sobre Bens e Serviços e Imposto Seletivo). No entanto, futuramente eles devem ser considerados no valor total dos documentos fiscais escriturados.

[\[voltar ao topo\]](#top)