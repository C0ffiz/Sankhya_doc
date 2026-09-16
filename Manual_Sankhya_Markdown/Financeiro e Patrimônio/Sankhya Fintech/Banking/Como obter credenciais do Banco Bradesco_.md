# Como obter credenciais do Banco Bradesco?

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/36551875605911-Como-obter-credenciais-do-Banco-Bradesco](https://ajuda.sankhya.com.br/hc/pt-br/articles/36551875605911-Como-obter-credenciais-do-Banco-Bradesco)

---

# Como obter credenciais do Banco Bradesco?

Para adquirir as credenciais do **Banco Bradesco** e ativar a funcionalidade de Boleto Simples, Híbrido ou PIX via API, siga as instruções abaixo:

 ![](https://ajuda.sankhya.com.br/hc/article_attachments/36551875593111) **Vincular  a SANKHYA como um PARCEIRO através da sua Conta Bradesco:**

1.1 Acesse o [Net Empresa](https://www.ne12.bradesconetempresa.b.br/ibpjlogin/login.jsf) do Bradesco e realize o login com seu usuário/senha

![](https://ajuda.sankhya.com.br/hc/article_attachments/36551875594135)

1.2 Acesse a aba **‘Serviços Operacionais’**

**![](https://ajuda.sankhya.com.br/hc/article_attachments/36551853648023)**

1.3 Clique em API :: **Integração com parceiros**

![](https://ajuda.sankhya.com.br/hc/article_attachments/36551853653015)

1.4 Preencha os dados

*   Produto = **API** 
*   Serviço = **Integração com Parceiro**
*   Tipo = **Contratação**

**![](https://ajuda.sankhya.com.br/hc/article_attachments/36551853653783)**

1.5 Preencha os dados solicitados no cadastro

**Importante:** Em ‘Parceiro Integrador’ selecione o parceiro = **SANKHYA**

**![](https://ajuda.sankhya.com.br/hc/article_attachments/36551875599895)**

1.8 Siga as etapas para que o usuário MASTER aprove  a solicitação

1.9 Certifique-se que a solicitação foi confirmada

![](https://ajuda.sankhya.com.br/hc/article_attachments/36551875602071)

Feito isso, inicie o processo de geração das credenciais:

 ![](https://ajuda.sankhya.com.br/hc/article_attachments/36551875603095) **Geração das Credenciais:**

**Importante:**

<table class="wysiwyg-table-resized"><colgroup><col style="width: NaN%;"></colgroup><tbody><tr><td><span style="background-color: #ffffff; color: #333333;">Para facilitar sua integração, reunimos aqui o passo a passo disponibilizado pelo Bradesco para criação das credenciais. Caso surjam dúvidas ou seja necessário suporte durante o processo, o <strong>contato deve ser feito diretamente com o Bradesco</strong>,&nbsp;</span></td></tr></tbody></table>

  
**2.1 Inscrição ao Portal Developers**

Acessar o [Portal Developers](https://developers.bradesco.com.br/#iss=https%3A%2F%2Flogin.axway.com%2Fauth%2Frealms%2FBroker) e seguir as etapas demonstradas abaixo, conforme instruções Bradesco :

**![](https://ajuda.sankhya.com.br/hc/article_attachments/36782473793431)**

**![](https://ajuda.sankhya.com.br/hc/article_attachments/36782473794327)**

  
![](https://ajuda.sankhya.com.br/hc/article_attachments/36782473795223)

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782435015447)

**2.2 Acesso ao Portal Developers**

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782473797015)

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782473798167)

**2.3 Inscrição para os produtos desejados**

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782473799191)

*   Para Boleto (Simples e Híbrido) : **Cobrança com QR Code**
*   Para PIX : **PIX - Geração de QR Code**

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782473804311)

Selecionado o produto, clique em ‘Inscrever-se’ para efetuar a assinatura no produto selecionado

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782473805591)

**Importante !**

No próximo passo, atente-se a seguinte informação : Para Integração aos serviços Fintech só serão aceitas Credenciais geradas em **PRODUÇÃO**.

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782435024791)

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782435025815)

**2.4 Registro da aplicação**

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782435027735)

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782473808791)

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782435029911)

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782473810455)

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782473811223)

Obs: Indicamos que todos os recursos ‘Produção’ sejam selecionados

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782435034391)

  
 

**2.5 Geração das Credenciais**

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782473812631)

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782435036823)

**Importante:**

<table class="wysiwyg-table-resized"><colgroup><col style="width: NaN%;"></colgroup><tbody><tr><td><p><span style="background-color: #ffffff; color: #333333;">Na etapa acima, no campo ‘<strong>Certificado Público no formato .pem .cer ou .crt’</strong>, deverá ser inserido o certificado baixado no SANKHYA.</span></p><p><span style="background-color: #ffffff; color: #333333;">Este certificado será encontrado em : Assistente de Melhores Práticas :: Configurações serviços Fintech :: Boleto Rápido :: Selecionar Conta Bradesco :: Etapa ‘Credenciais via API’ :: Campo <strong>‘Baixar Certificado’</strong></span></p><p><span style="background-color: #ffffff; color: #333333;"><strong><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42309696246807" width="587" height="229"></strong></span></p><p>&nbsp;</p></td></tr></tbody></table>

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782473815063)

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782435040279)

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782435041687)

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782473819287)

![](https://ajuda.sankhya.com.br/hc/article_attachments/36782435043607)