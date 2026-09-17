# Editor de Mensagens

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360045106353-Editor-de-Mensagens](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045106353-Editor-de-Mensagens)

---

# Editor de Mensagens

 **![Módulo](https://ajuda.sankhya.com.br/hc/article_attachments/42310426284439) Módulo:** BI Móvel > Mensagens        

---

A **"Mensagem"** é como os valores das variáveis serão apresentados ao usuário. São compostas por texto e fórmulas que serão enviadas por E-mail ou Mensagens SMS no celular. Para a composição de uma mensagem, atente-se para as informações que serão descritas nos tópicos a seguir.

Inicialmente, tem-se o **"Código"** único da mensagem que é atribuído automaticamente pelo sistema.

A marcação **"Ativa"** é responsável por dizer se a mensagem está habilitada e poderá ser utilizada em outras telas do sistema.

<table style="border-collapse: collapse; width: 100%;" border="1"><tbody><tr><td style="width: 100%;"><h4 id="h_01HA54CBDFNXHWK2ERRSG6VPYB" class="wysiwyg-text-align-center"><span class="wysiwyg-color-black70"><strong>Funcionalidades da tela&nbsp;</strong></span></h4></td></tr><tr><td style="width: 100%;">&nbsp;<a class="topiclink" href="#abapropriedades">Aba Propriedades</a>&nbsp; &nbsp; &nbsp; &nbsp;</td></tr><tr><td style="width: 100%;">&nbsp;<a class="topiclink" href="#abamensagem">Aba Mensagem</a>&nbsp;</td></tr><tr><td style="width: 100%;">&nbsp;<a class="topiclink" href="#abacondio">Aba Condição</a></td></tr><tr><td style="width: 100%;">&nbsp;<a class="topiclink" href="#abaperfisdestinatrios">Aba Perfis Destinatários</a></td></tr></tbody></table>

![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/1500005449062)

### **Aba Propriedades**

![mceclip1.png](https://ajuda.sankhya.com.br/hc/article_attachments/1500005545761)

Os seguintes campos fazem parte da aba Propriedades:

O campo **"Autor"** é preenchido por quem escreveu a mensagem automaticamente.

A **"Indicação"** será o meio pelo qual a mensagem será enviada, que poderá ser:

*   E-mail/SMS;
*   Mensagem Instantânea;
*   Aplicativo Móvel;
*   E-mail;
*   SMS;
*   Notificação do Sistema.

Em **"Data de alteração"** insira a data da última modificação na mensagem.

No campo **"Tentativas"**, tem-se o número de tentativas de envio para a mensagem antes de ser considerada falha de envio.

O **"Período"** possui configuração semelhante do campo Período das variáveis, e indicará os horários em que a condição da mensagem será testada para o envio. Se a condição for atendida, a mensagem será inserida na fila de envio.

Ao preencher o **"Tipo de conteúdo"**, será informado ao sistema se o texto da mensagem deve ser tratado como HTML ou texto plano (indicado para mensagens SMS).

[\[voltar ao topo\]](#top)

### **Aba Condição**

Aqui é definida a condição que deve ser satisfeita para que uma mensagem seja enviada. Essa condição pode ser escrita tanto na linguagem de script própria do BI Móvel quanto na linguagem Java. Para mais detalhes sobre a construção da fórmula da condição, veja o tópico **"Condição de disparo das Mensagens"** dentro da aba [Mensagem](#abamensagem).

![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/1500005545981)

**Observação:** para que as mensagens sejam enviadas apenas uma vez por dia, deve-se ligar o parâmetro **"Forçar envio único de Mens. diária BI Móvel? - MSDFORCUNDIA"**, porém, a mensagem deve possuir apenas um agendamento diário. Desse modo, caso haja um envio programado para depois da hora do processamento atual, este não será enviado.

[\[voltar ao topo\]](#top)

### **Aba Mensagem**

Defina nessa aba o texto da mensagem. As regras para a formulação da mensagem serão discutidas no artigo [Linguagem de Script do BI MÓVEL](https://ajuda.sankhya.com.br/hc/pt-br/articles/360051941074-Linguagem-de-Script-do-BI-M%C3%93VEL).

![mceclip3.png](https://ajuda.sankhya.com.br/hc/article_attachments/1500005546101)

**Observação:** ligue o parâmetro **"Remove quebra de linha de mensagem BI Móvel?-RMVQUEBRALNMSG"** para que seja removido os caracteres de quebra de linha ("\\n") do corpo da mensagem cadastrada.

[\[voltar ao topo\]](#top)

### **Aba Perfis Destinatários**

Aqui serão exibidas a lista de perfis contendo os consumidores para os quais a mensagem será enviada. Os consumidores e os perfis de envio devem ser previamente cadastrados.

![mceclip4.png](https://ajuda.sankhya.com.br/hc/article_attachments/1500005449342)

![acesse também FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/20473619002135) Para verificar as especificidades do BI Móvel referente ao Editor de Mensagens, acesse a documentação [Linguagem de Script do BI Móvel](https://ajuda.sankhya.com.br/hc/pt-br/articles/360051941074-Linguagem-de-Script-do-BI-M%C3%93VEL).

[\[voltar ao topo\]](#top)