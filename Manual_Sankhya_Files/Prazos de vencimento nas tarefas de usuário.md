# Prazos de vencimento nas tarefas de usuário

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/4408440807831-Prazos-de-vencimento-nas-tarefas-de-usu%C3%A1rio](https://ajuda.sankhya.com.br/hc/pt-br/articles/4408440807831-Prazos-de-vencimento-nas-tarefas-de-usu%C3%A1rio)

---

# Prazos de vencimento nas tarefas de usuário

![Versão - 32x32 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313355776279) **Versão disponível:** a partir da 4.9

---

Esse é um recurso que permite definir prazos de execução para as Tarefas de Usuário e geralmente é utilizando quando a empresa identifica a necessidade de estabelecer um prazo para as pessoas executarem uma determinada tarefa.

Em um processo de compras, por exemplo, podemos definir um prazo para os usuários que realizam a tarefa **"Realizar cotação"** (cotar preço/valor de algo) concluírem essa atividade.

Em nosso caso de uso, apresentaremos o processo de **"Adiantamento de viagens**":

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4408438283927)

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><span class="wysiwyg-color-black40 wysiwyg-font-size-small"><strong>Processo de Adiantamento de viagens</strong></span></td></tr></tbody></table>

Esse processo permite que qualquer colaborador solicite um adiantamento de viagem para seu líder imediato aprovar ou não essa solicitação. Essa análise tem o prazo de vencimento de 1 dia; conforme esse prazo for vencendo, o líder é alertado na tarefa e caso ele não analise dentro desse período, também será notificado sobre o status dessa tarefa via e-mail/sistema.

Aprovando a solicitação, ela é direcionada ao solicitante (colaborador), para que o mesmo detalhe todos os gastos ocasionados durante a viagem. Por fim, a solicitação é direcionada ao departamento financeiro realizar a análise das despesas e executar a compensação financeira.

Para que a tarefa **"Aprovar adiantamento de viagem"** tenha um prazo estabelecido, devemos habilitar a marcação **"Utilizar prazo?"**:

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4408438559639)

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><span class="wysiwyg-color-black40 wysiwyg-font-size-small"><strong>Utilizar prazo na tarefa</strong></span></td></tr></tbody></table>

Agora, o próximo passo é realizar as configurações necessárias para que o prazo de vencimento seja de 1 dia. Para isso, acessamos o botão **"Abrir configuração de Prazos de vencimento"** e na aba **"Prazo"** definimos o seguinte:

*   **Tipo de Prazo:** Fixo, pois sempre será o mesmo prazo.
*   **Prazo em:** Dia(s).
*   **Dias ou Horas:** 1

![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/4408438667287)

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><span class="wysiwyg-color-black40 wysiwyg-font-size-small"><strong>Configurando prazo na tarefa</strong></span></td></tr></tbody></table>

---

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 8.00004%;"><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42313295204631" alt="essencial FINAL (1).png"></td><td class="wysiwyg-text-align-justify" style="width: 92%;">Caso seja necessário definir um prazo dinâmico para uma mesma <span class="wysiwyg-underline">Tarefa de Usuário</span>, em função de um critério informado em um formulário, deve ser utilizado o <span class="wysiwyg-underline">Tipo de Prazo Variável</span>, para que seja possível escrever uma expressão em <span class="wysiwyg-underline">JavaScript</span> ou <span class="wysiwyg-underline">Groovy</span> e determinar a data de vencimento da tarefa. Nessa expressão poderão ser utilizadas todas as funções de consulta (disponível no help do script) para buscar os dados que foram preenchidos no processo.</td></tr></tbody></table>

---

Status é a situação de uma tarefa em relação ao seu prazo de vencimento. Por padrão, cada status (No prazo, A vencer, Vencido, Muito Vencido) tem um tempo decorrido já definido e, caso seja necessário, o modelador poderá alterá-lo. No status **"A vencer"**, por exemplo, o tempo decorrido padrão é de 70%, ou seja, quando atingir 70% do prazo estabelecido, a tarefa entrará no status A vencer.

**Observação:** na aba **"Status"**, o campo **"Contagem"** determina se o tempo decorrido será contado em **"Percentual"**, **"Dia(s)"** ou **"Hora(s)"**; por padrão ele já vem preenchido com a opção Percentual.

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4408525137303)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><span class="wysiwyg-color-black40 wysiwyg-font-size-small"><strong>Configurando status</strong></span></td></tr></tbody></table>

Para que o responsável pela tarefa Aprovar adiantamento de viagem visualize na Lista de Tarefas os status, conforme o prazo estabelecido for vencendo, manteremos ativo todos os status e para todos eles iremos configurar para que o dono/candidato da tarefa receba as notificações via e-mail e por sistema; para isso, selecionamos no **"Tipo"** a opção **"Ambas"** e informamos uma **"Conta SMTP"**. Também será possível inserir mais destinatários através de Scripts SQL porém não faremos nesse caso de uso.

Por fim, ao acessar a aba Prazo de vencimento, teremos o resumo de todas as configurações realizadas de prazo para essa tarefa:

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4408526237975)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><span class="wysiwyg-color-black40 wysiwyg-font-size-small"><strong>Resumo do prazo configurado</strong></span></td></tr></tbody></table>

Conforme as configurações realizadas, apresentaremos agora a visualização do prazo de vencimento e do status na tarefa (Lista de Tarefas).

Ao realizar a solicitação de um Adiantamento de viagem, a mesma foi direcionada para seu líder aprovar. Nesse exemplo, a solicitação foi feita no dia 21/09/2021 às 14:07:50 e, sendo assim, o prazo de vencimento é em 22/09/2021 às 14:07:50 e o status é **"No prazo"**, como apresentado no card e no cabeçalho da tarefa:

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409138814871)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><span class="wysiwyg-color-black40 wysiwyg-font-size-small"><strong>Prazo e status na tarefa</strong></span></td></tr></tbody></table>

Assim como configurado nos status, o dono/candidato da tarefa receberá uma notificação via sistema e e-mail o informando sobre o status do prazo de vencimento da tarefa:

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409134198679)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><strong><span class="wysiwyg-color-black40 wysiwyg-font-size-small">Notificação via sistema do status do prazo de vencimento da tarefa</span></strong></td></tr></tbody></table>

![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/4409134307479)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><span class="wysiwyg-color-black40 wysiwyg-font-size-small"><strong>Notificação via e-mail do status do prazo de vencimento da tarefa</strong></span></td></tr></tbody></table>

**Nota:** conforme for atingido o tempo decorrido que foi configurado em cada status, no card e no cabeçalho da tarefa o status será atualizado; por exemplo, ao atingir 70% do prazo decorrido de 1 dia, o status será atualizado para A vencer.

Outra funcionalidade com o prazo de vencimento no card da tarefa, é utilizar ele como critério na **"Ordenação das Tarefas"** de acordo com o seu vencimento, podendo ser **"Mais próximos primeiro"** ou **"Mais distantes primeiro"**:

![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/4408532928023)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><span class="wysiwyg-color-black40 wysiwyg-font-size-small"><strong>Ordenação das tarefas de acordo com o vencimento</strong></span></td></tr></tbody></table>

[\[Voltar ao topo\]](#top)