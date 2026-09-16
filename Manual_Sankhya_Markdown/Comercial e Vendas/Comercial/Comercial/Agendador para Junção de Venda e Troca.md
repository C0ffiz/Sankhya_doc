# Agendador para Junção de Venda e Troca

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360045119913-Agendador-para-Jun%C3%A7%C3%A3o-de-Venda-e-Troca](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045119913-Agendador-para-Jun%C3%A7%C3%A3o-de-Venda-e-Troca)

---

# Agendador para Junção de Venda e Troca

<table style="border-collapse: collapse; width: 100%; height: 29px;" cellspacing="0,5"><tbody><tr style="height: 58px;"><td class="wysiwyg-text-align-center" style="width: 100%; height: 29px;"><pre class="wysiwyg-text-align-justify"><span class="wysiwyg-font-size-medium"><strong><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42312131869591" alt="Módulo"> Módulo: </strong>Comercial &gt; Avançado &gt; Agendadores   </span></pre></td></tr></tbody></table>

---

 ![essencial](https://ajuda.sankhya.com.br/hc/article_attachments/16024064772119) Essa tela será habilitada somente se o parâmetro **"Junção de Pedidos de Venda e Troca - JUNVENDTROCA"** for ligado.

Esse agendador, normalmente é utilizado por empresas que trabalham com produtos perecíveis e que possuem compromisso de troca caso seus produtos pereçam no estoque de seus clientes.

Com base nisso, o sistema buscará os pedidos confirmados e pendentes com os [Tipos de Operação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP) configurados nesse agendador no período especificado; em seguida, irá inserir os itens do Pedido de Troca no Pedido de Venda correspondente, o que simplifica a quantidade de Pedidos a serem utilizados nesse processo.

Dessa forma, consulte os campos e funcionalidades disponíveis nessa tela nos links a seguir:

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td style="width: 35.9047%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#painelprincipal">Painel Principal</a></span></td><td style="width: 25.4762%;">&nbsp;</td><td style="width: 38.619%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#abahorrios">Aba Horários</a></span></td></tr><tr><td style="width: 35.9047%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#abafrenqunciaagendamento">Aba Frequência Agendamento</a></span></td><td style="width: 25.4762%;">&nbsp;</td><td style="width: 38.619%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#abaoutrasopes">Aba Outras Opções</a></span></td></tr><tr><td style="width: 35.9047%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#consideraesimportantes">Considerações importantes</a></span></td><td style="width: 25.4762%;">&nbsp;</td><td style="width: 38.619%;">&nbsp;</td></tr></tbody></table>

![agendador\_para\_j.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/1500006788282)

## Painel Principal

O campo **"Nro. agendamento"** corresponde à identificação do agendamento. Sendo que, ele pode ser gerado de forma automática ou manual.

Informe no campo **"Descrição agendamento"**, o nome da operação de agendamento a ser executada.

Defina a **"Empresa"** correspondente ao agendamento.

A marcação **"Ativo"**, determina se o agendamento está ativo ou não, ou seja, se pode ou não ser utilizado.

[\[voltar ao topo\]](#top)

## Aba Horários

No campo **"Próxima execução em"** dessa aba, você indicará a próxima data/hora em que a operação será executada.

Em **"Data Final de Execução"**, informe a data da operação.

![horarios\_agendador.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/1500006789302)

[\[voltar ao topo\]](#top)

## Aba Frequência Agendamento

Nessa aba, configure os Horários, dias, semanas ou meses de execução do agendador.

![frequencia\_agendamento\_3.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/1500006790142)

Na opção **"Horários"** são definidos em quais horários a tarefa será executada.

Temos também três opções de agendamento, sendo elas:

*   **Diário:** Ao selecionar essa opção, o sistema interpretará que a tarefa será executada todos os dias;
*   **Semanal:** Por meio dessa, será possível definir em quais dias da semana a tarefa será executada;
*   **Mensal:** Nessa opção, será definido em quais dias no mês a tarefa será executada.

[\[voltar ao topo\]](#top)

## Aba Outras Opções

![aba\_outras\_op\_\_es.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/1500006798642)

No campo **"TOP de Pedido de Venda"** dessa aba, você deve informar os Pedidos de Venda que possuem [Tipo de Operação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP) para que eles sejam processados com os Pedidos de Troca.

Informe no campo **"TOP de Pedido de Troca"** qual o Tipo de Operação a ser empregado para determinar que um Pedido corresponde a uma Troca.

Em **"Dias p/ buscar Pedidos"**, você definirá a quantidade de dias que o sistema fará a busca de todos os Pedidos entre a data atual, subtraída do número de dias informados nesse campo.

No campo **"% máximo de Troca"**, informe o percentual máximo do valor do pedido que poderá ser empregado na troca.

Caso haja algum erro durante a execução do Agendador e o campo **"E-mail p/informação de erros"** estiver preenchido, um e-mail a fim de comunicar o ocorrido será enviado para o endereço aqui informado.

**Nota:** Esse e-mail será enviado apenas quando acionado pelo recurso interno (job). Em execuções manuais, o mesmo não será enviado; assim, apenas ações programadas terão o comportamento de envio do e-mail.

O botão **"Executar agendador"** executa a junção de pedidos de venda e troca imediatamente, ignorando os cálculos de próxima execução do agendador. Esse botão utiliza os dados da tela no momento em que for pressionado.

Tanto pelo botão Executar agendador quanto pela execução normal do agendador no período determinado, o sistema buscará os pedidos confirmados e pendentes com as TOP's configuradas no agendador no período especificado e irá inserir os itens do Pedido de Troca no Pedido de Venda correspondente.

**Importante:** Para que sejam associados, a Empresa, o Parceiro e a Data de Negociação devem ser iguais no Pedido de Venda e no Pedido de Troca.

[\[voltar ao topo\]](#top)

## Considerações importantes

Destacamos ainda que, se houver mais de um Pedido de Troca, todos os itens dos Pedidos deverão ser inseridos no Pedido de Venda. Dessa forma, considere o exemplo a seguir:

Ao informar o % máximo de troca de 90%; considere três pedidos de troca, sendo que cada um deles possui valor total de R$ 30,00 totalizando R$ 90,00. Esses três pedidos foram relacionados a um pedido de R$ 200,00, pois a porcentagem máxima de troca foi respeitada.

Assim, temos o valor total dos Pedidos de Troca de R$ 90,00, dividido pelo valor total do Pedido de Venda de R$ 200,00, resultando em 0,45. Ou seja, 45% dos 90% permitido.

Os itens dos Pedidos de Troca serão inseridos no Pedido de Venda com **"Vlr. desconto"** igual ao valor total do item, e o campo Uso do Produto igual a Item de Troca.

Você pode observar esses itens na aba Troca, que corresponde à mesma aba Matéria-Prima ([Central de Vendas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612414)), mas com sua nomenclatura alterada pela ativação do parâmetro **"Calcular Desc. Indenização na hora do faturamento? - DESCINDENIZ"**, ou seja, o sistema não trabalhará com Matérias-Primas, mas sim com Trocas.

Se o valor do pedido de troca for superior ao percentual do campo **"% máximo de desconto de troca"** do pedido de venda, então a junção não será feita e um e-mail será enviado para o endereço inserido no campo **"E-mail p/informação de erros"** com data e hora da execução, assim como a mensagem a seguir:

_**"Pedido de troca \[NUNOTA do pedido de troca\] não foi descontado no pedido de venda porque o valor ultrapassou o % máximo de desconto de troca".**_

Ao faturar o Pedido de Venda, a Nota de Venda continuará com o Pedido de Troca (itens apresentados na aba Trocas), apesar dele não influenciar no valor total.

O valor total será o valor dos itens originais com o desconto proveniente dos itens de troca, que no caso do exemplo descrito acima, é R$200,00 (Valor total do pedido) – R$90,00 (Valor total dos pedidos de troca), que é igual a R$170,00.

O parâmetro DESCINDENIZ deve ser ligado para que o desconto dos itens de trocas sejam aplicados na Nota de Venda durante o faturamento.

**Observações complementares:**

*   Empresa, Parceiro e Data de Negociação devem ser iguais nos Pedidos de Venda e nos Pedidos de Troca, para que eles possam ser associados;
*   Se o sistema encontrar mais de um Pedido de Venda para um único Pedido de Troca, ele será **"ligado"** ao Pedido de Venda que possuir maior valor;
*   Se for encontrado mais de um Pedido de Troca, todos os itens de todos esses pedidos deverão ser inseridos no Pedido de Venda;
*   O sistema não possui uma regra para proibir a alteração nesses itens; esse comportamento deve ser controlado pela marcação **"Permite alteração após confirmar"** presente na [Aba Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abageral) do [Cadastro de Tipos de Operação](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP);
*   Depois da junção com o Pedido de Venda, o Pedido de Troca será marcado como não pendente;
*   Ao inserir o produto de troca no pedido comum, o Valor Unitário será o mesmo do Pedido de Troca.

[\[voltar ao topo\]](#top)