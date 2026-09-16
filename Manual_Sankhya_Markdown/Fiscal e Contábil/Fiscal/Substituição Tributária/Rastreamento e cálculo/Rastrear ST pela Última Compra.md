# Rastrear ST pela Última Compra

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594694-Rastrear-ST-pela-%C3%9Altima-Compra](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594694-Rastrear-ST-pela-%C3%9Altima-Compra)

---

# Rastrear ST pela Última Compra

<table style="border-collapse: collapse; width: 100%;" cellspacing="0,5"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><pre class="wysiwyg-text-align-justify"><span class="wysiwyg-font-size-small"><span class="wysiwyg-font-size-medium"><strong><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42312890504087" alt="Módulo 36x36 FINAL.png"> </strong></span></span><strong>Módulo: </strong>Livros Fiscais &gt; Avançado &gt; Rastreamento de Estoque/ST</pre></td></tr></tbody></table>

---

Esta tela apenas será exibida quando o parâmetro **"Rastreia ST pela última entrada - RASTSTULTENTRA"** encontrar-se habilitado, assim como a rotina [Entradas que Amparam ST](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594994).

![rastrear.png](https://ajuda.sankhya.com.br/hc/article_attachments/8769561618711)

**Importante:** esta tela é a responsável por implantar o processo de Rastreamento de ST pela Última Compra do produto; caso não tenha sido implantada em primeiro momento, as informações de ICMS ST não serão devidamente populadas ou utilizadas.

**Observação:** ao realizar o rastreamento por meio dessa tela, o sistema informará na tela [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113), aba [Rastreamento Por Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#abarastreamentoporempresa), o **"Tipo de Rastreamento"** com a opção **"Última Compra"**.

**Nota:** o saldo utilizado nesta rotina será informado na tela Entradas que Amparam ST, onde constam os valores unitários de ICMS ST capturados na Últ. Entrada.

<table style="border-collapse: collapse; width: 100%; height: 48px;"><tbody><tr style="height: 26px;"><td style="width: 33.3333%; height: 26px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#filtros">Filtros</a>&nbsp; &nbsp;</span></td><td style="width: 22.3333%; height: 26px;">&nbsp;</td><td style="width: 44.3333%; height: 26px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#gradeprodutos">Grade de Produtos</a></span></td></tr><tr style="height: 22px;"><td style="width: 33.3333%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#rastreamentodest">Rastreamento de ST</a></span></td><td style="width: 22.3333%; height: 22px;">&nbsp;</td><td style="width: 44.3333%; height: 22px;">&nbsp;</td></tr></tbody></table>

## Filtros

![ST1.png](https://ajuda.sankhya.com.br/hc/article_attachments/8769566212759)

No local em destaque, teremos o **"Filtro personalizado"** e os **"Filtros rápidos"**, sendo que, através de um Filtro personalizado será possível filtrar os produtos para o Rastreamento de ST de uma maneira dinâmica, em que você poderá utilizar variáveis ou querys; já em relação aos Filtros rápidos, estes estão divididos em **"Empresa"** (que se trata de um campo de preenchimento obrigatório), **"Produto"**, **"Grupo de Produto"** e **"Grupo de ICMS do Produto"**.

[\[voltar ao topo\]](#top)

## Grade Produtos

![ST2.png](https://ajuda.sankhya.com.br/hc/article_attachments/8769603035799)

Esta grade exibirá todos os produtos que foram filtrados através do Filtro personalizado ou dos Filtros rápidos e que poderão ser processados.

**Observação:** os produtos que não se enquadram nos filtros ou que já estão sendo rastreados não serão exibidos nesta grade.

[\[voltar ao topo\]](#top)

## Rastreamento de ST

Após filtrados os produtos, para processar o Rastreamento de ST pela Última Compra, acione o botão ![rastrear2.png](https://ajuda.sankhya.com.br/hc/article_attachments/8769621296407) **"Rastrear"**.

Assim, o sistema implantará o Rastreamento pela Última Compra para cada um dos produtos selecionados e, caso não ocorra nenhum erro, será exibida uma mensagem informando que o Rastreamento de ST pela Última Compra foi concluído com sucesso. Por outro lado, caso seja concluído o rastreamento mas ocorra erro em algum dos produtos apresentados na lista, será apresentada a seguinte mensagem:

_**"Erro ao tentar buscar o rastreamento:**_

_**\[Não foram encontrados valores de ICMS ST para rastreamento Código da Empresa: X Código do Produto: X Nota de Nro Único: X, Sequência: X\]."**_

Ainda neste sentido, caso o processamento do rastreamento tenha encontrado mais de um produto com erro, será exibida a mensagem a seguir:

_**"Erro ao tentar buscar o rastreamento para X produtos".**_

Após processado o rastreamento, o sistema incluirá e atualizará as informações do [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Produtos-), aba [Impostos / Informações por empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Produtos-#abaimpostosinformaesporempresa), marcando a opção **"Usa Rastro/ST pela Últ. Entrada"**.

**Nota:** caso já exista uma linha correspondente na aba acima mencionada, apenas será atualizado o campo; caso não exista, o sistema realizará a cópia dos dados do produto e irá inserir uma nova linha na aba Impostos / Informações por empresa, para que corresponda ao mesmo.

**Observação:** além de serem inseridos os dados na aba Impostos / Informações por empresa do Cadastro de Produtos, também serão inseridos na tela [Entradas que Amparam ST](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594994).

Desta forma, após obter-se os dados dos impostos unitários pela rotina de Entradas que Amparam ST e o produto encontrar-se marcado como Usa Rastro/ST pela Ult. Entrada, ao realizar a venda do mesmo, no momento da confirmação da NF de Venda, o sistema imputará os valores multiplicados pela quantidade negociada do mesmo.

[\[voltar ao topo\]](#top)