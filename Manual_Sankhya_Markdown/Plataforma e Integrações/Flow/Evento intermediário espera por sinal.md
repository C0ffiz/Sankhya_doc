# Evento intermediário espera por sinal

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/4405298024599-Evento-intermedi%C3%A1rio-espera-por-sinal](https://ajuda.sankhya.com.br/hc/pt-br/articles/4405298024599-Evento-intermedi%C3%A1rio-espera-por-sinal)

---

# Evento intermediário espera por sinal

![Versão - 32x32 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313306990359) **Versão:** a partir da 4.3

---

O Evento intermediário espera por sinal interrompe o fluxo do processo até a chegada de um sinal.

Ao integrar o processo com outras rotinas do ERP, como, por exemplo, em uma empresa de desenvolvimento de software existe um processo de correção de erros do sistema, em que, após a correção ser realizada, ela deverá ser oficializada em um pacote para ser disponibilizado ao cliente, que é realizada por um outro software. Nesse momento, o processo é interrompido até que a correção seja oficializada nesse pacote.

Assim, quando as tarefas são concluídas nessa segunda aplicação, um sinal é enviado ao SankhyaFlow para continuar o processo.

Outro exemplo são os processos que precisam aguardar a baixa de um título financeiro para dar continuidade na sua execução.

Para demonstrar essa funcionalidade, iremos utilizar como caso de uso o processo de [Adiantamento de viagens](https://drive.google.com/file/d/1RA3c5e-tg_rcHX3LhI_xnspczoYbiv2T/view):

![floww1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405303344663)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Processo de Adiantamento de viagens</strong></span></p></td></tr></tbody></table>

Esse processo permite que qualquer colaborador solicite um adiantamento de viagem para a empresa, que poderá ser aprovado ou reprovado pelo seu líder imediato.

Caso seja aprovado, dois títulos serão gerados automaticamente: receita e despesa. O título de despesa representa o desembolso financeiro que a empresa fará ao colaborador, através de uma transferência bancária, dinheiro, etc, e o título de receita será utilizado para basear a compensação financeira após o acerto de despesas.

Em seguida, o solicitante receberá um e-mail informando que sua solicitação foi aprovada e que em breve o dinheiro será disponibilizado. Nesse momento o processo é interrompido até que o financeiro faça a baixa do título de despesa. Quando for executada essa baixa, um sinal é enviado ao SankhyaFlow para continuar o processo.

---

No decorrer dessa documentação, demonstraremos como inserir o evento no processo e como personalizá-lo.

Para inserir o evento no processo, basta selecionar uma tarefa qualquer no diagrama do processo; assim, será apresentada uma caixa com várias opções, dentre elas, selecione **"Adicionar evento intermediário"** ou busque pelo elemento **"Criar evento intermediário"** dentro da paleta localizada no lado esquerdo:

![floww2.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4405298406551)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Inserção de Evento intermediário espera por sinal no processo</strong></span></p></td></tr></tbody></table>

Em seguida, com o evento selecionado, clique no ícone **"Alterar tipo" ![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405298409879)** e selecione o **"Evento intermediário espera por sinal"**:

![floww3.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4405298453527)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Inserção de Evento intermediário espera por sinal no processo</strong></span></p></td></tr></tbody></table>

Ao inserir esse evento no processo, você deve informar o **"Nome do Sinal"** pois o utilizaremos em sua personalização.

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/4405298467223)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Inserção Nome do Sinal</strong></span></p></td></tr></tbody></table>

**Observação:** o elemento sinal deve possuir um nome único, pertencente àquela abertura de processo em específico, para que possa enviar o sinal correto e dar continuidade ao fluxo certo.

A personalização do evento precisa implementar a chamada do método **sendSignal**, pertencente ao pacote **br.com.sankhya.workflow.api.SankhyaFlow**, que pode ser obtido a partir dessa [biblioteca](https://drive.google.com/file/d/1ZUS04jMHlmZ9gHRUkehgtUJiE2FAIP08/view?usp=sharing).

**Nota:** o Evento de sinal pode ser implementado através de uma personalização (Rotina Java) no Sankhya Om (evento programado, botão de ação, etc).

Abaixo, segue o exemplo de um evento programado para o nosso caso de uso, onde a baixa do título de despesa do adiantamento envia o sinal **"baixouTítulo"** ao processo:

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td class="wysiwyg-text-align-justify" style="width: 100%;"><pre><span class="wysiwyg-color-yellow120">import</span> br.com.sankhya.extensions.eventoprogramavel.EventoProgramavelJava;<br><span class="wysiwyg-color-yellow120">import</span> br.com.sankhya.jape.event.PersistenceEvent;<br><span class="wysiwyg-color-yellow120">import</span> br.com.sankhya.jape.event.TransactionContext;<br><span class="wysiwyg-color-yellow120">import</span> br.com.sankhya.jape.sql.NativeSql;<br><span class="wysiwyg-color-yellow120">import</span> br.com.sankhya.jape.vo.DynamicVO;<br><span class="wysiwyg-color-black50"><em>//Biblioteca de APIs do SankhyaFlow</em></span><br><span class="wysiwyg-color-yellow120">import</span> br.com.sankhya.workflow.api.SankhyaFlow;<br><span class="wysiwyg-color-yellow120">import</span> java.math.BigDecimal;<br><span class="wysiwyg-color-yellow120">import</span> java.sql.ResultSet;<br><span class="wysiwyg-color-yellow120">import</span> java.sql.Timestamp;<br><span class="wysiwyg-color-yellow120">import</span> java.util.ArrayList;<br><span class="wysiwyg-color-yellow120">import</span> java.util.List;<br>public class <span class="wysiwyg-color-blue80">SinalBaixarTitulo</span> implements <span class="wysiwyg-color-black30">EventoProgramavelJava {</span><br>public void <span class="wysiwyg-color-blue80">afterDelete</span>(PersistenceEvent <span class="wysiwyg-color-black30">arg0</span>) throws Exception <span class="wysiwyg-color-black30">{}</span><br>public void <span class="wysiwyg-color-blue80">afterInsert</span>(PersistenceEvent <span class="wysiwyg-color-black30">event</span>) throws Exception <span class="wysiwyg-color-black30">{}</span><br>public void <span class="wysiwyg-color-blue80">afterUpdate</span>(PersistenceEvent <span class="wysiwyg-color-black30">event</span>) throws Exception <span class="wysiwyg-color-black30">{</span><br>DynamicVO <span class="wysiwyg-color-blue80">financeiro</span> <span class="wysiwyg-color-yellow110">=</span> <span class="wysiwyg-color-black30">(DynamicVO)</span><span class="wysiwyg-color-blue80">event</span>.<span class="wysiwyg-color-blue80">getVo</span>();<br>BigDecimal <span class="wysiwyg-color-blue80">nufin</span> <span class="wysiwyg-color-yellow110">=</span> <span class="wysiwyg-color-blue80">financeiro</span>.<span class="wysiwyg-color-blue80">asBigDecimal</span>(<span class="wysiwyg-color-cyan110">"NUFIN"</span>);<br>Timestamp <span class="wysiwyg-color-blue80">dhbaixa</span> <span class="wysiwyg-color-yellow110">=</span> <span class="wysiwyg-color-blue80">financeiro</span>.<span class="wysiwyg-color-blue80">asTimestamp</span>(<span class="wysiwyg-color-cyan110">"DHBAIXA"</span>);<br><span class="wysiwyg-color-yellow120">if</span> (<span class="wysiwyg-color-black30">dhbaixa</span> <span class="wysiwyg-color-yellow110">!=</span> <span class="wysiwyg-color-yellow120">null</span>) {<br>List&lt;String&gt; <span class="wysiwyg-color-blue80">idIstPrn</span> <span class="wysiwyg-color-yellow110">=</span> <span class="wysiwyg-color-yellow120">new</span> ArrayList&lt;String&gt;();<br>NativeSql <span class="wysiwyg-color-blue80">query</span> <span class="wysiwyg-color-yellow110">=</span> <span class="wysiwyg-color-yellow120">null</span>;<br><span class="wysiwyg-color-yellow120">try</span> {<br><span class="wysiwyg-color-blue80">query</span> <span class="wysiwyg-color-yellow110">=</span> <span class="wysiwyg-color-yellow120">new</span> <span class="wysiwyg-color-blue80">NativeSql</span>(<span class="wysiwyg-color-blue80">event</span>.<span class="wysiwyg-color-blue80">getJdbcWrapper</span>());<br><span class="wysiwyg-color-blue80">query</span>.<span class="wysiwyg-color-blue80">appendSql</span>(<span class="wysiwyg-color-cyan110">"SELECT IDINSTPRN FROM AD_SOLICITACAOADIANTAMENTO WHERE<br>NUFIN_AD_D = :NUFIN"</span>);<br><span class="wysiwyg-color-blue80">query</span>.<span class="wysiwyg-color-blue80">setNamedParameter</span>(<span class="wysiwyg-color-cyan110">"NUFIN"</span>, <span class="wysiwyg-color-blue80">nufin</span>);<br>ResultSet <span class="wysiwyg-color-blue80">rs</span> <span class="wysiwyg-color-yellow110">=</span> <span class="wysiwyg-color-blue80">query</span>.<span class="wysiwyg-color-blue80">executeQuery</span>();<br><span class="wysiwyg-color-yellow120">while</span> (<span class="wysiwyg-color-blue80">rs</span>.<span class="wysiwyg-color-blue80">next</span>())<br><span class="wysiwyg-color-blue80">idIstPrn</span>.<span class="wysiwyg-color-blue80">add</span>(<span class="wysiwyg-color-blue80">rs</span>.<span class="wysiwyg-color-blue80">getBigDecimal</span>(<span class="wysiwyg-color-cyan110">"IDINSTPRN"</span>).<span class="wysiwyg-color-blue80">toString</span>()); <br>} <span class="wysiwyg-color-yellow120">finally</span> {<br><span class="wysiwyg-color-blue80">NativeSql</span>.<span class="wysiwyg-color-blue80">releaseResources</span>(<span class="wysiwyg-color-yellow120">query</span>);<br>} <br>String[] <span class="wysiwyg-color-blue80">instancias</span> <span class="wysiwyg-color-yellow110">=</span> idIstPrn.<span class="wysiwyg-color-black30">&lt;String&gt;</span><span class="wysiwyg-color-blue80">toArray</span>(<span class="wysiwyg-color-yellow120">new</span> String[<span class="wysiwyg-color-pink110">0</span>]);<br><span class="wysiwyg-color-black50"><em>//Método 'sendSignal' passando o nome do sinal e as instâncias de processo</em></span><br><span class="wysiwyg-color-blue80">SankhyaFlow</span>.<span class="wysiwyg-color-blue80">sendSignal</span>(<span class="wysiwyg-color-cyan110">"baixouTitulo"</span>, instancias);<br>} <br>}<br>public void <span class="wysiwyg-color-blue80">beforeCommit</span>(TransactionContext <span class="wysiwyg-color-black30">arg0</span>) throws Exception <span class="wysiwyg-color-black30">{}</span><br>public void <span class="wysiwyg-color-blue80">beforeDelete</span>(PersistenceEvent <span class="wysiwyg-color-black30">arg0</span>) throws Exception <span class="wysiwyg-color-black30">{}</span><br>public void <span class="wysiwyg-color-blue80">beforeInsert</span>(PersistenceEvent <span class="wysiwyg-color-black30">arg0</span>) throws Exception <span class="wysiwyg-color-black30">{}</span><br>public void <span class="wysiwyg-color-blue80">beforeUpdate</span>(PersistenceEvent <span class="wysiwyg-color-black30">arg0</span>) throws Exception <span class="wysiwyg-color-black30">{}</span><br>}</pre></td></tr></tbody></table>

Após a implementação da personalização, é gerado o módulo Java e então, ele é vinculado na aba Eventos da tabela TGFFIN.

 **![essencial FINAL (1).png](https://ajuda.sankhya.com.br/hc/article_attachments/16092588076183)**A(s) instância(s) do processo de Adiantamento de viagem será(ão) automaticamente interrompida(s) no momento que chegar no evento de sinal **"Aguardar baixa de título"** e somente será retomado quando o financeiro executar a baixa dos títulos de despesas.

[\[Voltar ao topo\]](#top)