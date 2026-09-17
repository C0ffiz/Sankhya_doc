# Processo Geração da Conta Contábil para EFD - Contribuições

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360044599594-Processo-Gera%C3%A7%C3%A3o-da-Conta-Cont%C3%A1bil-para-EFD-Contribui%C3%A7%C3%B5es](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044599594-Processo-Gera%C3%A7%C3%A3o-da-Conta-Cont%C3%A1bil-para-EFD-Contribui%C3%A7%C3%B5es)

---

# Processo Geração da Conta Contábil para EFD - Contribuições

**Você encontra neste artigo:**

<table style="border-collapse: collapse;" id="sumario"><tbody><tr><td style="border-color: #999; padding: 8px; vertical-align: top; width: 50%;"><a href="#oque">O que é e para que serve</a><br><a href="#formas">Formas de Buscar a Conta Contábil</a><br>&nbsp;&nbsp;&nbsp;↳ <a href="#cadastros">Opção Cadastros</a><br>&nbsp;&nbsp;&nbsp;↳ <a href="#contabilizacao">Opção Contabilização</a><br><a href="#reg0500">Geração do Registro 0500</a></td><td style="border-color: #999; padding: 8px; vertical-align: top; width: 50%;"><a href="#reg0600">Geração do Registro 0600</a><br><a href="#obrigatorios">Registros Obrigatórios na Geração da Conta Contábil</a><br><a href="#observacoes">Observações Importantes</a></td></tr></tbody></table>

## O que é e para que serve

O **Processo Geração da Conta Contábil para EFD - Contribuições** gera a conta contábil utilizada nos registros da **Escrituração Fiscal Digital (EFD) - Contribuições**.

A conta contábil é buscada em outras telas do sistema — **Empresa**, **Cadastro de Produtos**, **Cadastro de Serviços**, **Tipo de Operação (TOP)** e **Plano de Contas** — e não na tela onde o arquivo é gerado. Ela é pré-requisito para a geração de determinados registros do arquivo (veja a lista completa em [Registros Obrigatórios na Geração da Conta Contábil](#obrigatorios)); esses registros são gerados na tela **EFD - Contribuições PIS/COFINS**.

## Formas de Buscar a Conta Contábil

Existem duas formas de pesquisar a conta contábil, e cada empresa só pode ter uma definição de busca configurada. Na rotina **Empresa**, aba **EFD - Escrituração Fiscal Digital**, o campo **Tipo da Conta Contábil para EFD** disponibiliza as opções:

*   **Cadastros**
*   **Contabilização**

### Opção Cadastros

Ao selecionar **Cadastros**, configure a **Conta Contábil para EFD**. Na geração do arquivo da EFD Contribuições, o sistema segue uma ordem de análise para buscar o código vinculado ao campo **Conta Contábil para EFD**.

Para produtos e serviços, a sequência de análise é:

1.  Produto › **Cadastro de Produtos**, aba **Impostos / Informações por empresa**; Serviço › **Cadastro de Serviços**, aba **Configurações por Empresa**
2.  Produto › **Cadastro de Produtos**, aba **Impostos**; Serviço › **Cadastro de Serviços**, aba **Impostos**
3.  **Cadastro de Grupos de Produtos/Serviços**, aba **Impostos por Empresa**
4.  **Cadastro de Grupos de Produtos/Serviços**, aba **Geral**
5.  **Tipo de Operação - TOP**, aba **Impostos**

Para os registros referentes aos financeiros — como F100, F500 e F525 — a hierarquia segue esta ordem:

1.  **Cadastro de Natureza de Receitas e Despesas**, aba **PIS/COFINS**
2.  **Tipo de Operação - TOP**, aba **Impostos**

Para os registros referentes ao imobilizado — como F120 e F130 — a ordem de hierarquia é:

1.  **Cadastro de Produtos**, aba **Impostos**
2.  **Tipo de Operação - TOP**, aba **Impostos**

### Opção Contabilização

Ao adotar **Contabilização**, na geração do registro o sistema verifica a contabilização do documento em questão, ordenando primeiro pelo lançamento na contabilidade de maior valor para a conta configurada no grupo de natureza para EFD definido.

A determinação da conta a ser gerada no arquivo segue a movimentação do registro em foco — o sistema localiza, na contabilização dos registros, as contas contábeis configuradas com a natureza para EFD:

*   Para os registros referentes aos movimentos de Estoque contabilizados pela contabilização do Estoque ou do Livro (`TCBINT.ORIGEM = 'E' ou 'L'`)
*   Para os registros referentes aos movimentos do Financeiro contabilizados pela contabilização do Financeiro, Baixa, Movimentação Bancária, Renegociação e Juros (`TCBINT.ORIGEM = 'F', 'B', 'M', 'R', 'J'`)
*   Para os registros referentes às movimentações do Imobilizado, a busca da conta segue a contabilização que ocorreu no Produto ou no Bem em questão

[↑ Voltar ao início](#sumario)

## Geração do Registro 0500

O registro 0500 é gerado conforme a configuração do **Cadastro de Plano de Contas** da empresa que estiver gerando a EFD - Contribuições. Caso sejam gerados os registros das filiais no arquivo, também é gerado o plano de contas das filiais. Só são geradas as contas contábeis que já foram geradas nos registros do arquivo.

A tabela a seguir detalha a composição de cada campo do registro 0500:

<table class="wysiwyg-table-resized" style="border-collapse: collapse;"><colgroup><col style="width: 11.76%;"> <col style="width: 29.68%;"> <col style="width: 11.45%;"> <col style="width: 47.11%;"></colgroup><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Campo</strong></td><td style="border-color: #999; padding: 6px;"><strong>Descrição</strong></td><td style="border-color: #999; padding: 6px;"><strong>Fixo</strong></td><td style="border-color: #999; padding: 6px;"><strong>Origem (TCBPLA)</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">1</td><td style="border-color: #999; padding: 6px;">Texto fixo contendo <code>0500</code>.</td><td style="border-color: #999; padding: 6px;"><code>0500</code></td><td style="border-color: #999; padding: 6px;"></td></tr><tr><td style="border-color: #999; padding: 6px;">2</td><td style="border-color: #999; padding: 6px;">Data da inclusão/alteração.</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">Conforme gravado no banco de dados, campo <strong>Referência de ativação</strong> (<code>DTINCLUSAO</code>).</td></tr><tr><td style="border-color: #999; padding: 6px;">3</td><td style="border-color: #999; padding: 6px;">Código da natureza da conta/grupo de contas:<br>01 - Contas de ativo;<br>02 - Contas de passivo;<br>03 - Patrimônio líquido;<br>04 - Contas de resultado;<br>05 - Contas de compensação;<br>09 - Outras.</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">Busca do campo <strong>Grupo de Conta</strong> conforme cadastro.</td></tr><tr><td style="border-color: #999; padding: 6px;">4</td><td style="border-color: #999; padding: 6px;">Indicador do tipo de conta:<br>S - Sintética (grupo de contas);<br>A - Analítica (conta).</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">Busca do campo <strong>Analítica</strong>.</td></tr><tr><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">S - Sintética (grupo de contas);</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;"></td></tr><tr><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">A - Analítica (conta).</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;"></td></tr><tr><td style="border-color: #999; padding: 6px;">5</td><td style="border-color: #999; padding: 6px;">Nível da conta analítica/grupo de contas.</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">Conforme o nível em que a conta contábil foi cadastrada.</td></tr><tr><td style="border-color: #999; padding: 6px;">6</td><td style="border-color: #999; padding: 6px;">Código da conta analítica/grupo de contas.</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">Busca do campo <strong>Conta contábil</strong>.</td></tr><tr><td style="border-color: #999; padding: 6px;">7</td><td style="border-color: #999; padding: 6px;">Nome da conta analítica/grupo de contas.</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">Busca do campo <strong>Descrição</strong>.</td></tr><tr><td style="border-color: #999; padding: 6px;">8</td><td style="border-color: #999; padding: 6px;">Código da conta correlacionada no Plano de Contas Referenciado, publicado pela Receita Federal do Brasil (RFB).</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">Busca do campo <strong>Cód. Conta Ref.</strong>.</td></tr><tr><td style="border-color: #999; padding: 6px;">9</td><td style="border-color: #999; padding: 6px;">CNPJ do estabelecimento, no caso de a conta informada no campo <code>COD_CTA</code> ser específica de um estabelecimento.</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">É gerado o código do CNPJ da empresa dona do plano de contas, somente nos casos em que o arquivo está sendo gerado para diversas filiais com planos de contas diferentes.</td></tr></tbody></table>

Exemplo do registro 0500 gerado no arquivo:

![1.png](https://ajuda.sankhya.com.br/hc/article_attachments/42432043355287)

[↑ Voltar ao início](#sumario)

## Geração do Registro 0600

O registro 0600 só é gerado para as empresas que buscam a conta contábil pela opção **Contabilização**, sendo que a contabilização dos movimentos deve ser por Centro de Resultado. Para as empresas que geram a conta contábil de forma fixa (opção **Cadastros**), este registro não é gerado.

Exemplo do registro 0600 gerado no arquivo:

![2.png](https://ajuda.sankhya.com.br/hc/article_attachments/42432056797847)

[↑ Voltar ao início](#sumario)

## Registros Obrigatórios na Geração da Conta Contábil

Abaixo estão os blocos e seus respectivos registros nos quais a geração da conta contábil é obrigatória. Cada registro utiliza uma listagem de naturezas das contas contábeis para buscar a conta contábil — essas naturezas são indicadas na rotina **Cadastro de Plano de Contas**, aba **Geral**, campo **Natureza para EFD**.

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Bloco A</strong></td><td style="border-color: #999; padding: 6px;"><strong>Bloco C</strong></td><td style="border-color: #999; padding: 6px;"><strong>Bloco C</strong></td><td style="border-color: #999; padding: 6px;"><strong>Bloco D</strong></td><td style="border-color: #999; padding: 6px;"><strong>Bloco F</strong></td><td style="border-color: #999; padding: 6px;"><strong>Bloco P</strong></td><td style="border-color: #999; padding: 6px;"><strong>Bloco 1</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">A170</td><td style="border-color: #999; padding: 6px;">C170</td><td style="border-color: #999; padding: 6px;">C481</td><td style="border-color: #999; padding: 6px;">D100</td><td style="border-color: #999; padding: 6px;">F100-Orig. Financ.</td><td style="border-color: #999; padding: 6px;">P100</td><td style="border-color: #999; padding: 6px;">1900</td></tr><tr><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">C175</td><td style="border-color: #999; padding: 6px;">C485</td><td style="border-color: #999; padding: 6px;">D101</td><td style="border-color: #999; padding: 6px;">F100-Orig.Jur./Mult.</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;"></td></tr><tr><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">C181</td><td style="border-color: #999; padding: 6px;">C491</td><td style="border-color: #999; padding: 6px;">D105</td><td style="border-color: #999; padding: 6px;">F120</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;"></td></tr><tr><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">C185</td><td style="border-color: #999; padding: 6px;">C495</td><td style="border-color: #999; padding: 6px;">D201</td><td style="border-color: #999; padding: 6px;">F130</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;"></td></tr><tr><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">C191</td><td style="border-color: #999; padding: 6px;">C501</td><td style="border-color: #999; padding: 6px;">D205</td><td style="border-color: #999; padding: 6px;">F500</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;"></td></tr><tr><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">C195</td><td style="border-color: #999; padding: 6px;">C505</td><td style="border-color: #999; padding: 6px;">D501</td><td style="border-color: #999; padding: 6px;">F525</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;"></td></tr><tr><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">C381</td><td style="border-color: #999; padding: 6px;">C810</td><td style="border-color: #999; padding: 6px;">D505</td><td style="border-color: #999; padding: 6px;">F550</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;"></td></tr><tr><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">C385</td><td style="border-color: #999; padding: 6px;">C870</td><td style="border-color: #999; padding: 6px;">D601</td><td style="border-color: #999; padding: 6px;">F650</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;"></td></tr><tr><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;">C396</td><td style="border-color: #999; padding: 6px;">C880</td><td style="border-color: #999; padding: 6px;">D605</td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;"></td><td style="border-color: #999; padding: 6px;"></td></tr></tbody></table>

**ℹ️ Nota**

As contas contábeis do Bloco M não são geradas, pois não há apuração do registro no sistema. Informe as contas diretamente no validador.

Cada lista de naturezas utilizada na busca da conta contábil é:

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Lista</strong></td><td style="border-color: #999; padding: 6px;"><strong>Naturezas</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">Lista 01</td><td style="border-color: #999; padding: 6px;">01 - Receita de Vendas, Receitas prestação serviços, Receitas financeiras, Receitas não operacionais<br>02 - Receitas de vendas não tributadas<br>04 - Custo de Produtos/Serviços prestados por pessoa jurídica<br>06 - Despesas Diversas<br>08 - Estoques, Matéria prima e material de embalagem<br>09 - Aquisições de bens para revenda, aquisições de insumos para industrialização</td></tr><tr><td style="border-color: #999; padding: 6px;">Lista 02</td><td style="border-color: #999; padding: 6px;">01 - Receita de Vendas, Receitas prestação serviços, Receitas financeiras, Receitas não operacionais<br>02 - Receitas de vendas não tributadas</td></tr><tr><td style="border-color: #999; padding: 6px;">Lista 03</td><td style="border-color: #999; padding: 6px;">03 - Receita de Fretes, Receita de transportes rodoviário de cargas<br>05 - Custos com transportes<br>06 - Despesas Diversas<br>07 - Despesas de fretes contratados e despesas de comercialização<br>08 - Estoques, Matéria prima e material de embalagem<br>09 - Aquisições de bens para revenda, aquisições de insumos para industrialização<br>11 - Máquinas e Equipamentos do Ativo Imobilizado, ativo fixo, etc.</td></tr><tr><td style="border-color: #999; padding: 6px;">Lista 04</td><td style="border-color: #999; padding: 6px;">03 - Receita de Fretes, Receita de transportes rodoviário de cargas</td></tr><tr><td style="border-color: #999; padding: 6px;">Lista 05</td><td style="border-color: #999; padding: 6px;">06 - Despesas Diversas<br>07 - Despesas de fretes contratados e despesas de comercialização</td></tr><tr><td style="border-color: #999; padding: 6px;">Lista 06</td><td style="border-color: #999; padding: 6px;">12 - Despesas de Aplicações Financeiras, Despesas Financeiras (juros/Multas)<br>13 - Receitas de Aplicações Financeiras, Receitas Financeiras (juros/Multas)</td></tr><tr><td style="border-color: #999; padding: 6px;">Lista 07</td><td style="border-color: #999; padding: 6px;">10 - Encargos de depreciação do período, encargos de amortização do período, etc.</td></tr><tr><td style="border-color: #999; padding: 6px;">Lista 08</td><td style="border-color: #999; padding: 6px;">11 - Máquinas e Equipamentos do Ativo Imobilizado, ativo fixo, etc.</td></tr><tr><td style="border-color: #999; padding: 6px;">Lista 09</td><td style="border-color: #999; padding: 6px;">01 - Receita de Vendas, Receitas prestação serviços, Receitas financeiras, Receitas não operacionais<br>02 - Receitas de vendas não tributadas<br>03 - Receita de Fretes e Receita de transportes rodoviários de cargas</td></tr><tr><td style="border-color: #999; padding: 6px;">Lista 10</td><td style="border-color: #999; padding: 6px;">Não é possível mapear este registro pela Contabilização. O sistema sempre busca a conta contábil configurada nas <strong>Preferências da Empresa</strong>, aba <strong>Reintegra Previdência</strong>, campo <strong>Código Conta Contábil</strong>.</td></tr></tbody></table>

Para a **Lista 08**, informe a conta contábil que será gerada no registro F130 no campo **Conta Contábil para EFD** (tela **Cadastro de Produtos**, aba **Impostos**).

[↑ Voltar ao início](#sumario)

## Observações Importantes

*   Os registros que apresentarem a conta contábil sem configuração são gravados no log de erro. O arquivo de log tem o mesmo nome do arquivo gerado, mas com a extensão `.erro` — por exemplo: _"REGISTRO: A170. NUNOTA: 475701. SEQUENCIA: 1. ORIGEM: E. Conta Contábil está vazia."_ Nesse caso, acesse o registro em questão, verifique a contabilização do documento de origem e analise as configurações definidas na busca da conta contábil.
*   Na geração da conta contábil nos registros EFD - Contribuições, informe o código da conta contábil credora ou devedora principal — a conta principal é aquela que recebeu o maior valor na contabilização da operação.
*   É enviado no arquivo EFD - Contribuições o plano de contas da empresa, somente das contas que obtiveram registros no arquivo. Empresas que também entregam a **Escrituração Contábil Digital (ECD)** devem informar as mesmas contas contábeis, de forma que seja enviado o mesmo plano de contas.
*   Na geração da EFD Contribuições, quando se trata de uma empresa com várias filiais, o sistema verifica se cada filial está configurada com o mesmo **Tipo de Conta Contábil para EFD** da matriz.

**⚠️ Atenção**

Caso as filiais não estejam configuradas com o mesmo **Tipo de Conta Contábil para EFD** da matriz, o sistema exibe a mensagem _"As empresas filiais da matriz X não possuem a mesma configuração para o campo Tipo da Conta Contábil para EFD e isso poderá impedir que o sistema busque corretamente as contas do arquivo. Deseja continuar?"_. Ao optar por **Sim**, a geração continua, mantendo o risco de busca incorreta das contas. Ao optar por **Não**, padronize o campo **Tipo de Conta Contábil para EFD** para todas as filiais nas **Preferências da Empresa**, aba **EFD - Escrituração Fiscal Digital**.

A relação entre o Plano de Contas e os registros EFD esperados pelo sistema para a geração das contas contábeis é:

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Registros</strong></td><td style="border-color: #999; padding: 6px;"><strong>Naturezas (lista)</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">A170, C170, C191, C195, C396, C481, C485, C501, C505, F100_NOTA, F100_FINANCEIRO</td><td style="border-color: #999; padding: 6px;">1, 2, 3, 4, 6, 7, 8, 9</td></tr><tr><td style="border-color: #999; padding: 6px;">C175, C181, C185, C381, C385, C491, C495, C810, C870</td><td style="border-color: #999; padding: 6px;">1, 2</td></tr><tr><td style="border-color: #999; padding: 6px;">D100, D101, D105</td><td style="border-color: #999; padding: 6px;">3, 5, 6, 7, 8, 9, 11</td></tr><tr><td style="border-color: #999; padding: 6px;">D201, D205, D601, D605</td><td style="border-color: #999; padding: 6px;">3</td></tr><tr><td style="border-color: #999; padding: 6px;">D501, D505</td><td style="border-color: #999; padding: 6px;">6, 7</td></tr><tr><td style="border-color: #999; padding: 6px;">F500, F510, F525, F550, F560, 1900</td><td style="border-color: #999; padding: 6px;">1, 2, 3</td></tr><tr><td style="border-color: #999; padding: 6px;">F100_MULTA, F100_JURO, F100_DESCONTO</td><td style="border-color: #999; padding: 6px;">1, 2, 6, 7, 12, 13</td></tr></tbody></table>