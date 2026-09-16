# Geração da Conta Contábil para EFD ICMS/IPI

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/8811502871703-Gera%C3%A7%C3%A3o-da-Conta-Cont%C3%A1bil-para-EFD-ICMS-IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/8811502871703-Gera%C3%A7%C3%A3o-da-Conta-Cont%C3%A1bil-para-EFD-ICMS-IPI)

---

# Geração da Conta Contábil para EFD ICMS/IPI

Neste artigo iremos tratar das informações pertinentes para a geração da Conta Contábil para ICMS/IPI:

*   [Formas de Buscar a Conta Contábil](#FormasdeBuscaraContaCont%C3%A1bil)
*   [Geração do Registro 0300](#Gera%C3%A7%C3%A3odoRegistro0300)
*   [Geração do Registro 0500](#Gera%C3%A7%C3%A3odoRegistro0500)
*   [Registros gerados](#Registrosgerados)

---

### Formas de Buscar a Conta Contábil

Tem-se duas formas de realizar a pesquisa da Conta Contábil, sendo que uma empresa só poderá ter uma definição de busca configurada. Na rotina [Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa), o campo **"Tipo da Conta Contábil para EFD ICMS/IPI"** localizado na aba [EFD - Escrituração Fiscal Digital](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abaefdescrituraofiscaldigital), disponibiliza as opções que permitem realizar a referida seleção. São elas:

*   Cadastros;
*   Contabilização.

![Imagens\_ksnip\_192\_.png](https://ajuda.sankhya.com.br/hc/article_attachments/8809731301911)

Quando indicada a opção **"****Cadastros"**, teremos a seguinte hierarquia de busca da conta contábil:

 **![1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16427029350423)**Tela [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113), sendo que:

*   Se o registro se referir a Produtos, será verificada a aba [Impostos/Informações por empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113#abaimpostosinformaesporempresa), campo **"Contábil para EFD"**.
*   Caso o registro se refira a Serviço, será analisada a tela [Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Servi%C3%A7o#top), aba [Configurações por Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110553-Servi%C3%A7o#abaconfiguraesporempresa), campo **"Contábil para EFD"**.

 ![2 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16427029356823) Tela Cadastro de Produtos:

*   Para Produtos ou Serviços, será verificada a aba [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113#abaimpostos), campo **"Contábil para EFD"**.

 ![3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16427029362455) Tela [Grupos de Produtos/Serviços](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044598294):

*   Aba [Impostos por Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044598294#abaimpostosporempresa), campo **"Conta contábil para EFD"**.
*   Aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044598294#abageral), campo **"Conta contábil para EFD"**.

 ![4 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16427029366167) Tela [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114):

*   Aba [Livro Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114#abalivrofiscal), campo **"Conta contábil para EFD"**.

**Observação:** referente ao registro D100, quando a Conta Contábil da TOP estiver preenchida, o sistema irá considerá-la em primeiro nível da hierarquia ou quando este campo estiver vazio, o sistema seguirá com os níveis da hierarquia informada acima. 

Adotando a opção **"Contabilização"**, na geração do registro o sistema verificará na contabilização do documento em questão, ordenando primeiramente pelo lançamento na contabilidade de maior valor para a conta configurada no determinado grupo de **"Natureza para EFD"** definido. De forma que, o sistema localizará na contabilização as contas contábeis com as seguintes naturezas:

*   01- Receita de vendas; 
*   02- Receitas de vendas não tributadas; 
*   03- Receita de fretes, receita de transportes rodoviário de cargas;
*   04- Custos de produtos/serviços prestados por pessoa jurídica; 
*   05- Custos com transportes;
*   06- Despesas diversas; 
*   07- Despesas de fretes contratados e despesas de comercialização; 
*   08- Estoques, matéria-prima e material de embalagem; 
*   09- Aquisições de bens para revenda, aquisições de insumos para industrialização;
*   11- Máquinas e equipamentos do ativo imobilizado, ativo fixo, etc.

A determinação da conta a ser gerada no arquivo será conforme a movimentação do registro em foco. De forma que, o sistema localizará na contabilização dos determinados registros as contas contábeis configuradas com a natureza para EFD:

*   Para os registros referentes aos movimentos de Estoque que foram contabilizadas pela contabilização do Estoque ou do Livro (TCBINT.ORIGEM = 'E' ou ‘L’);
*   Para os registros referentes aos movimentos do Financeiro que foram contabilizadas pela contabilização do Financeiro, Baixa, Movimentação Bancária, Renegociação e Juros (TCBINT.ORIGEM = F', 'B', 'M', 'R', 'J’);
*   Para os registros referentes às movimentações do Imobilizado, a busca da conta será conforme a Contabilização que ocorreu no Produto ou no Bem em questão.

[\[voltar ao topo\]](#top)

### Geração do Registro 0300

Para o registro 0300 referente ao imobilizado, a hierarquia para a geração da conta contábil cadastrada no campo **"Conta Contábil para EFD"** seguirá a seguinte ordem: 

*   Tela [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113) > aba [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113#abaimpostos);
*   Tela [Tipos de Operação - TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114) > aba  [Livro Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114#abalivrofiscal).

No registro 0300 referente ao imobilizado a conta contábil pela Contabilização segue a mesma regra de quando utilizamos a opção Cadastro, uma vez que, não existe contabilização para estes movimentos.

Para que a informação do campo **"Conta Contábil para EFD"** do Cadastro de Produtos (aba Impostos, [Seção EFD Fiscal/Contribuições/Reinf/Sintegra](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos#Se%C3%A7%C3%A3oEFDFiscal/Contribui%C3%A7%C3%B5es/Reinf/Sintegra)), seja usada na geração do registro 0300 no [EFD Fiscal ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/7267044122263-EFD-Fiscal-ICMS-IPI), é preciso seguir as seguintes configurações:

1.  A conta contábil escolhida deve estar ligada à empresa no plano de contas. Esse plano é configurado nas [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa), na aba [Contabilidade](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abacontabilidade).
2.  Além disso, a conta contábil precisa ter o campo **"Natureza para EFD"**, da aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abageral), configurado com a opção **"11 - Máquinas e Equipamentos do Ativo Imobilizado, ativo fixo, etc."**

Se essas condições não forem cumpridas, o registro será preenchido com a conta contábil indicada no campo **"Conta Contábil 1"** do Cadastro de Produtos.

[\[voltar ao topo\]](#top)

### Geração do Registro 0500

O registro 0500 será gerado conforme a configuração do [Cadastro de Plano de Contas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116393-Plano-de-Contas) da Empresa que estiver gerando EFD Fiscal. Caso sejam gerados os registros das filiais no arquivo, também será gerado o plano de contas das filiais.

Só serão geradas as contas contábeis que foram geradas nos registros do arquivo.

[\[voltar ao topo\]](#top)

### Registros gerados 

**C170 no campo 37:**  Itens do documento (código 01, 1b, 04 e 55) registro filho do C100.

**C300 no campo 11:** Resumo diário das notas fiscais de venda a consumidor (código 02).

**C350 no campo 12:** Nota fiscal de venda a consumidor (código 02).

![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16427013330327)Lista de Naturezas utilizadas nos registros C170, C300 e C350: 

*   01- Receita de vendas;
*   02- Receitas de vendas não tributadas;
*   04- Custos de produtos/serviços prestados por pessoa jurídica;
*   06- Despesas diversas;
*   07-Despesas de fretes contratados e despesas de comercialização;
*   08- Estoques, matéria-prima e material de embalagem;
*   09-Aquisições de bens para revenda, aquisições de insumos para industrialização.

**C500 no campo 33:** Nota fiscal/conta de energia elétrica (código 06), nota fiscal de energia elétrica eletrônica – nf3e (código 66), nota fiscal/conta de fornecimento d'água canalizada (código 29) e nota fiscal consumo fornecimento de gás (código 28).

![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16427013330327)Lista de Naturezas:

*   01- Receita de vendas;
*   02- Receitas de vendas não tributadas;
*   03- Receita de fretes, receita de transportes rodoviário de cargas;
*   04- Custos de produtos/serviços prestados por pessoa jurídica;
*   06- Despesas diversas;
*   07-Despesas de fretes contratados e despesas de comercialização;
*   08- Estoques, matéria-prima e material de embalagem;
*   09-Aquisições de bens para revenda, aquisições de insumos para industrialização.

**D100 no campo 23:** Nota fiscal de serviço de transporte (código 07) e conhecimentos de transporte rodoviário de cargas (código 08), conhecimentos de transporte de cargas avulso (código 8b), aquaviário de cargas (código 09), aéreo (código 10), ferroviário de cargas (código 11), multimodal de cargas (código 26), nota fiscal de transporte ferroviário de carga (código 27), conhecimento de transporte eletrônico – ct-e (código 57), conhecimento de transporte eletrônico para outros serviços - ct-e os (código 67) e bilhete de passagem eletrônico – bp-e (código 63)

![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16427013330327)Lista de Naturezas:

*   03- Receita de fretes, receita de transportes rodoviários de cargas;
*   05- Custos com transportes;
*   06- Despesas diversas;
*   07- Despesas de fretes contratados e despesas de comercialização;
*   08- Estoques, matéria-prima e material de embalagem;
*   09-Aquisições de bens para revenda, aquisições de insumos para industrialização;
*   11- Máquinas e equipamentos do ativo imobilizado, ativo fixo, etc.

**D500 no campo 23:** Nota fiscal de serviço de comunicação (código 21) e nota fiscal de serviço de telecomunicação (código 22).

**D510 no campo 20:** Itens do documento – nota fiscal de serviço de comunicação (código 21) e serviço de telecomunicação (código 22). 

![Marcador 3 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16427013330327)Lista de Naturezas utilizadas nos registros D500 e D510:

*   06- Despesas diversas;
*   07- Despesas de fretes contratados e despesas de comercialização;

[\[voltar ao topo\]](#top)