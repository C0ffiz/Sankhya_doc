# Contabilização de Financeiros com Ajuste ao Valor Presente

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360044598734-Contabiliza%C3%A7%C3%A3o-de-Financeiros-com-Ajuste-ao-Valor-Presente](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044598734-Contabiliza%C3%A7%C3%A3o-de-Financeiros-com-Ajuste-ao-Valor-Presente)

---

# Contabilização de Financeiros com Ajuste ao Valor Presente

O Conselho Federal de Contabilidade – CFC, através do Comitê de Pronunciamentos Contábeis - CPF tem o objetivo de adequar a nossa legislação às normas internacionais da contabilidade e determinou a adequação da contabilização de financeiros ajustada ao valor presente.

O Ajuste ao Valor Presente refere-se a todos aqueles elementos de longo prazo do ativo ou passivo ou de curto prazo, mas relevantes à entidade, que devem ser contabilizadas pelo seu valor presente, isso quer dizer que se retiram as parcelas dos juros do valor do financeiro conforme taxas de mercado.

Além da separação do valor principal dos juros na contabilização da receita/despesas/imobilizado, os valores constantes do realizável/exigível deverão inicialmente ser compostos apenas do valor principal (valor presente) e os juros em conta específica.  A contabilidade deverá ser capaz de periodicamente apropriar parcelas de juros ao realizável/exigível até que ao vencimento (ou antecipação) estes se igualem ao valor total da transação.

Essas questões influenciam diretamente na análise do balanço, principalmente ao analisarmos o **"Valor da Empresa"**, pois influenciam diretamente no ativo e passivo.

Para facilitar sua navegação nessa documentação, acesse os links abaixo:

[Configurações Necessárias](#configura%C3%A7%C3%B5esnecess%C3%A1rias)                                            [Cálculo do Valor Presente](#c%C3%A1lculodovalorpresente)

[Contabilização](#contabiliza%C3%A7%C3%A3o)                                                                   [Imobilizado](#imobilizado)

---

#### **Configurações Necessárias**

Na tela [Tipos de Título](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044606494-Tipos-de-T%C3%ADtulo), aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044606494-Tipos-de-T%C3%ADtulo#abageral) você deve efetuar a marcação **"Ajusta Valor Presente"**.

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4407180888983)

Informe o tipo de título valor presente ao [Tipo de Negociação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045109173-Tipos-de-Negocia%C3%A7%C3%A3o):

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4407194535447)

Após isso, na tela [Valores de Moedas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044604754-Valores-de-Moedas), cadastre uma moeda do tipo **"Índice"** e na aba **"Cotação de Moeda"** insira os índices da Data do Movimento com o último dia de cada mês.

Na [TOP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP), aba [Financeiro](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abafinanceiro), seção **"Ajuste Valor Presente"** é necessário inserir o **"****Cód. Moeda Ajusta Valor Presente"** cadastrado anteriormente e indicar uma das opões abaixo no campo **"****Ajusta Valor Presente"**:

*   **Mensal:** O sistema realiza o calculo mês a mês entre a data de negociação e a data de vencimento; o juro é calculado e inserido na tabela TGFAVP.
*   **Ajuste no Vencimento****:** Será gravada uma única linha com a data de referência da parcela de juros igual ao vencimento do título.
*   **Ajuste Anual****:** Partindo da data de negociação, serão calculados os juros para cada competência mensal da mesma forma que no ajuste mensal porém, acumula-se cada conjunto de 12 meses gerando registro na TGFAVP com a soma do valor dos juros gravando como referência a última data.
*   **Ajuste fim de exercício****:** O processo é mesmo do Ajuste anual porém, calcula-se primeiro até o final do exercício (Ano) e a partir daí a cada 12 meses.

![mceclip3.png](https://ajuda.sankhya.com.br/hc/article_attachments/4407180972311)

[\[voltar ao topo\]](#top)

#### **Cálculo do Valor Presente**

Após realizar as configurações acima, o sistema realiza o cálculo na inserção e/ou alteração do financeiro. Por exemplo:

Foram lançados os títulos;

<table style="border-collapse: collapse; width: 81.2746%; margin-right: auto; margin-left: auto;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><span class="wysiwyg-color-black60"><strong>Índices lançados ao final de cada mês:</strong> </span></pre></td></tr></tbody></table>

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto; height: 178px;"><tbody><tr style="height: 24px;"><td style="width: 50%; height: 24px;"><p><span class="wysiwyg-font-size-medium"><strong>Data do movimento</strong></span></p></td><td style="width: 50%; height: 24px;"><span class="wysiwyg-font-size-medium"><strong>Índice</strong></span></td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">31/12/2013</span></td><td style="width: 50%; height: 22px;">1,50</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">31/01/2014</span></td><td style="width: 50%; height: 22px;">2,00</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">28/02/2014</span></td><td style="width: 50%; height: 22px;">2,50</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">31/03/2014</span></td><td style="width: 50%; height: 22px;">3,00</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">30/04/2014</span></td><td style="width: 50%; height: 22px;">3,50</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">31/05/2014</span></td><td style="width: 50%; height: 22px;">4,00</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">30/06/2014</span></td><td style="width: 50%; height: 22px;">4,50</td></tr></tbody></table>

**Financeiro 1**

<table style="border-collapse: collapse; width: 81.2746%; margin-right: auto; margin-left: auto;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><span class="wysiwyg-color-black60"><strong><img src="/hc/article_attachments/42310682039191" alt="CF05.png" width="286" height="48"></strong></span></pre></td></tr></tbody></table>

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto; height: 178px;"><tbody><tr style="height: 24px;"><td style="width: 50%; height: 24px;"><p><span class="wysiwyg-font-size-medium"><strong>Data de Negociação</strong></span></p></td><td style="width: 50%; height: 24px;"><span class="wysiwyg-font-size-medium">10/03/2014</span></td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><strong><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Data de Vencimento</span></strong></td><td style="width: 50%; height: 22px;">09/04/2014</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><strong><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Valor de Desdobramento</span></strong></td><td style="width: 50%; height: 22px;">R$1.000,00</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><strong><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Valor Presente</span></strong></td><td style="width: 50%; height: 22px;">R$970,70</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><strong><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Juros Valor Presente</span></strong></td><td style="width: 50%; height: 22px;">R$29,30</td></tr></tbody></table>

<table style="border-collapse: collapse; width: 81.2746%; margin-right: auto; margin-left: auto;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><strong>Memória de cálculo – Tabela TGFAVP (Ajusta Valor Presente)</strong></pre></td></tr></tbody></table>

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto; height: 89px;"><tbody><tr style="height: 24px;"><td style="width: 41.5714%; height: 24px;"><p><span class="wysiwyg-font-size-medium"><strong>Data de Referência</strong></span></p></td><td style="width: 27.8571%; height: 24px;"><span class="wysiwyg-font-size-medium"><strong>Índice</strong></span></td><td style="width: 30.5715%; height: 24px;"><span class="wysiwyg-font-size-medium"><strong>Juros Valor Presente</strong></span></td></tr><tr style="height: 22px;"><td style="width: 41.5714%; height: 18px;"><p>31/03/2014</p></td><td style="width: 27.8571%; height: 18px;">2,1</td><td style="width: 30.5715%; height: 18px;">20,38</td></tr><tr style="height: 22px;"><td style="width: 41.5714%; height: 25px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">09/04/2014</span></td><td style="width: 27.8571%; height: 25px;">0,9</td><td style="width: 30.5715%; height: 25px;">8,92</td></tr><tr style="height: 22px;"><td style="width: 41.5714%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Juros Valor Presente</span></td><td style="width: 27.8571%; height: 22px;">&nbsp;13,17</td><td style="width: 30.5715%; height: 22px;">&nbsp;</td></tr></tbody></table>

**Financeiro 2**

<table style="border-collapse: collapse; width: 81.2746%; margin-right: auto; margin-left: auto;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><span class="wysiwyg-color-black60"><img src="/hc/article_attachments/42310682039703" alt="CF06.png"></span></pre></td></tr></tbody></table>

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto; height: 178px;"><tbody><tr style="height: 24px;"><td style="width: 50%; height: 24px;"><p><span class="wysiwyg-font-size-medium"><strong>Data de Negociação</strong></span></p></td><td style="width: 50%; height: 24px;"><span class="wysiwyg-font-size-medium">10/03/2014</span></td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><strong><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Data de Vencimento</span></strong></td><td style="width: 50%; height: 22px;">09/05/2014</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><strong><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Valor de Desdobramento</span></strong></td><td style="width: 50%; height: 22px;">R$1.000,00</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><strong><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Valor Presente</span></strong></td><td style="width: 50%; height: 22px;">R$936,47</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><strong><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Juros Valor Presente</span></strong></td><td style="width: 50%; height: 22px;">R$63,53</td></tr></tbody></table>

<table style="border-collapse: collapse; width: 81.2746%; margin-right: auto; margin-left: auto;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><strong>Memória de cálculo – Tabela TGFAVP (Ajusta Valor Presente)</strong></pre></td></tr></tbody></table>

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto; height: 111px;"><tbody><tr style="height: 24px;"><td style="width: 41.5714%; height: 24px;"><p><span class="wysiwyg-font-size-medium"><strong>Data de Referência</strong></span></p></td><td style="width: 27.8571%; height: 24px;"><span class="wysiwyg-font-size-medium"><strong>Índice</strong></span></td><td style="width: 30.5715%; height: 24px;"><span class="wysiwyg-font-size-medium"><strong>Juros Valor Presente</strong></span></td></tr><tr style="height: 22px;"><td style="width: 41.5714%; height: 18px;"><p>31/03/2014</p></td><td style="width: 27.8571%; height: 18px;">2,1</td><td style="width: 30.5715%; height: 18px;">19,67</td></tr><tr style="height: 22px;"><td style="width: 41.5714%; height: 25px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">30/04/2014</span></td><td style="width: 27.8571%; height: 25px;">3,5</td><td style="width: 30.5715%; height: 25px;">33,47</td></tr><tr style="height: 22px;"><td style="width: 41.5714%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">05/09/2014</span></td><td style="width: 27.8571%; height: 22px;">1,05</td><td style="width: 30.5715%; height: 22px;">10,39</td></tr><tr style="height: 22px;"><td style="width: 41.5714%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Juros Valor Presente</span></td><td style="width: 27.8571%; height: 22px;">38,17</td><td style="width: 30.5715%; height: 22px;">&nbsp;</td></tr></tbody></table>

**Financeiro 3**

<table style="border-collapse: collapse; width: 81.2746%; margin-right: auto; margin-left: auto;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><span class="wysiwyg-color-black60"><img src="/hc/article_attachments/42310682040087" alt="CF07.png"></span></pre></td></tr></tbody></table>

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto; height: 178px;"><tbody><tr style="height: 24px;"><td style="width: 50%; height: 24px;"><p><span class="wysiwyg-font-size-medium"><strong>Data de Negociação</strong></span></p></td><td style="width: 50%; height: 24px;"><span class="wysiwyg-font-size-medium">10/03/2014</span></td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><strong><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Data de Vencimento</span></strong></td><td style="width: 50%; height: 22px;">09/06/2014</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><strong><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Valor de Desdobramento</span></strong></td><td style="width: 50%; height: 22px;">R$1.000,00</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><strong><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Valor Presente</span></strong></td><td style="width: 50%; height: 22px;">R$899,12</td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><strong><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Juros Valor Presente</span></strong></td><td style="width: 50%; height: 22px;">R$100,88</td></tr></tbody></table>

<table style="border-collapse: collapse; width: 81.2746%; margin-right: auto; margin-left: auto;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre><strong>Memória de cálculo – Tabela TGFAVP (Ajusta Valor Presente)</strong></pre></td></tr></tbody></table>

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto; height: 111px;"><tbody><tr style="height: 24px;"><td style="width: 41.5714%; height: 24px;"><p><span class="wysiwyg-font-size-medium"><strong>Data de Referência</strong></span></p></td><td style="width: 27.8571%; height: 24px;"><span class="wysiwyg-font-size-medium"><strong>Índice</strong></span></td><td style="width: 30.5715%; height: 24px;"><span class="wysiwyg-font-size-medium"><strong>Juros Valor Presente</strong></span></td></tr><tr style="height: 22px;"><td style="width: 41.5714%; height: 18px;"><p>31/03/2014</p></td><td style="width: 27.8571%; height: 18px;">2,1</td><td style="width: 30.5715%; height: 18px;">18,88</td></tr><tr style="height: 22px;"><td style="width: 41.5714%; height: 25px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">30/04/2014</span></td><td style="width: 27.8571%; height: 25px;">3,5</td><td style="width: 30.5715%; height: 25px;">32,13</td></tr><tr style="height: 22px;"><td style="width: 41.5714%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">31/05/2014</span></td><td style="width: 27.8571%; height: 22px;">4,0</td><td style="width: 30.5715%; height: 22px;">38,01</td></tr><tr><td style="width: 41.5714%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">06/09/2014</span></td><td style="width: 27.8571%;">1,2</td><td style="width: 30.5715%;">11,86</td></tr><tr style="height: 22px;"><td style="width: 41.5714%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Juros Valor Presente</span></td><td style="width: 27.8571%; height: 22px;">100,88</td><td style="width: 30.5715%; height: 22px;">&nbsp;</td></tr></tbody></table>

Quando é realizado o estorno dos títulos, a TGFAVP retorna ao estado inicial.

**Nota:** da forma como foi apresentada a memória de cálculo da TGFAVP, o tipo de inserção do ajuste é **"Mensal"**, ou seja, mês a mês entre a data de negociação e a data de vencimento o juro é calculado e inserido na tabela TGFAVP; essa configuração é inserida da TOP, conforme citamos acima.

[\[voltar ao topo\]](#top)

#### **Contabilização**

Após calcular o financeiro com os valores presentes e as tabelas dos juros se apresentarem com valores presentes, é hora de realizar a contabilização.

Na tela [TOP de contabilização](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044608174-TOP-Contabiliza%C3%A7%C3%A3o), indique no campo **"Tipo de data"** a opção **"Ajusta Valor Presente"**:

![mceclip4.png](https://ajuda.sankhya.com.br/hc/article_attachments/4407194627351)

Para a contabilização da nota serão disponibilizadas as fórmulas:

*   **ValorPresente:** Somatória do campo TGFFIN.VALORPRESENTE dos títulos do financeiro da nota.
*   **TotalJurosValorPresente:** Somatória do campo TGFFIN.JUROSAVP dos títulos do financeiro da nota.

Para a contabilização do financeiro/baixa e renegociação serão disponibilizadas as fórmulas:

*   **ValorPresente (TGFFIN.VALORPRESENTE)**
*   **TotalJurosValorPresente (TGFFIN.JUROSAVP)**

Na tela de [Agendamento](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044608294-Agendamento), na aba **"Filtros"**, é possível agendar a contabilização filtrando por **"Juros AVP"**:

![mceclip5.png](https://ajuda.sankhya.com.br/hc/article_attachments/4407181075479)

[\[voltar ao topo\]](#top)

#### **Imobilizado**

Para que seja feita a aquisição de um imobilizado, a TOP de Compra deve estar configurada para atualizar o bem e as configurações do cálculo do valor presente (ajusta valor presente diferente de **'N'** e moeda maior que zero); o produto deve ser de imobilizado.

Ao gerar o financeiro da nota de compra do produto imobilizado, todos os financeiros terão o valor presente gerado e os juros gerados na tabela TGFAVP. Após gerar os financeiros, o valor presente e o valor de depreciação da tabela do imobilizado (TCIBEM) serão gerados.

Primeiro o índice:

_Índice = Soma(TGFFIN.VALORPRESENTE)/ SOMA(TGFFIN.VLRDESDOBR)_

_TCIBEM.VALORPRESENTE = TCIBEM.VLRAQUISICAO \* INDICE_

_TCIBEM.VLRDEP = TCIBEM.VLRDEPORIG \* INDICE_

**TCIBEM**

<table class="wysiwyg-text-align-center" style="border-collapse: collapse; width: 94.2842%;" border="1"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 21.0606%;"><strong>CODBEM</strong></td><td class="wysiwyg-text-align-center" style="width: 18.9394%;"><strong>NUNOTA</strong></td><td class="wysiwyg-text-align-center" style="width: 20%;"><strong>CODPROD</strong></td><td class="wysiwyg-text-align-center" style="width: 20%;"><strong>VALORPRESENTE</strong></td><td class="wysiwyg-text-align-center" style="width: 14.3956%;"><strong>VLRDEP</strong></td></tr><tr><td class="wysiwyg-text-align-center" style="width: 21.0606%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">00006621-008179-0001</span></td><td class="wysiwyg-text-align-center" style="width: 18.9394%;">6621</td><td class="wysiwyg-text-align-center" style="width: 20%;">8179</td><td class="wysiwyg-text-align-center" style="width: 20%;">144,32</td><td class="wysiwyg-text-align-center" style="width: 14.3956%;">144,32</td></tr></tbody></table>

O campo **"VLRDEPORIG"** serve para armazenar o valor de depreciação antes de aplicar o índice do valor presente. Portanto, deve-se preencher o campo **"VLRDEP"** via trigger ou qualquer outra maneira fora do Sankhya Om, sendo que o campo VLRDEPORIG deve ter o mesmo valor de VLRDEP quando inserir ou alterar o campo.

[\[voltar ao topo\]](#top)