# Obtenção das credenciais do aplicativo Outlook para o protocolo OAuth

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/25744837815959-Obten%C3%A7%C3%A3o-das-credenciais-do-aplicativo-Outlook-para-o-protocolo-OAuth](https://ajuda.sankhya.com.br/hc/pt-br/articles/25744837815959-Obten%C3%A7%C3%A3o-das-credenciais-do-aplicativo-Outlook-para-o-protocolo-OAuth)

---

# Obtenção das credenciais do aplicativo Outlook para o protocolo OAuth

**Atenção: Este método de envio será descontinuado** A Microsoft deixará de oferecer suporte de segurança para o envio de e-mails via **SMTP (SMTP AUTH)** a partir de **01/03/2026**.

Para garantir que as suas comunicações e faturamentos não sejam interrompidos, recomendamos fortemente que utilize a nova integração via **Microsoft Graph API**. Ela é mais segura, moderna e o novo padrão recomendado pelo sistema.

[**Clique aqui para acessar o novo guia: Obtenção das credenciais do aplicativo Outlook para Graph API**](https://ajuda.sankhya.com.br/hc/pt-br/articles/40377307749399-Obten%C3%A7%C3%A3o-das-credenciais-do-aplicativo-Outlook-para-Graph-API)

### **Sobre este manual**

Este guia descreve o processo de obtenção de credenciais para o modelo de envio **SMTP via OAuth2 (Legado)**. Utilize estas instruções apenas se a sua operação ainda depender estritamente do protocolo SMTP e se estiver ciente do prazo de desativação mencionado acima.

Para criar o seu aplicativo no provedor da Microsoft, siga os passos abaixo:

### **Obtenção das credenciais do aplicativo Outlook**

Para criar um novo aplicativo utilizando o provedor da Microsoft, siga os passos abaixo:

Acesse o portal [Microsoft Entra](https://login.microsoftonline.com/organizations/oauth2/v2.0/authorize?redirect_uri=https%3A%2F%2Fentra.microsoft.com%2Fsignin%2Findex%2F&response_type=code%20id_token&scope=https%3A%2F%2Fmanagement.core.windows.net%2F%2Fuser_impersonation%20openid%20email%20profile&state=OpenIdConnect.AuthenticationProperties%3D81ZtVtoHs_guMhSBt0eUgF6X3cYbwzU6_epHgggbPw1hwpAqJv53FukYfjeeEeA9lTYMp22H7LDAALmvBft1rAHEFn2Q2bAGYt6JiElRfpl1Mi_Ykta8a_9Vy5X39mC4mpfw9BLLjt6to4Iyk8ZDKO0N1J95CPmM_j10_F2NGZp1TXD7mZAByo_D_YItEFFLNF12ISJN7fN5gUalZOfqut_RFLGCuAGO_Zbyde-XbOglAlxgNoQM4NWByEwusewrKy5wapPmOWxbDJLRMHdj2W5iZkh3VOPy00d2rjHZ7To0EMSgjXEIwka-Kbn84zK66pFIAfdMELrh83vOTN5Wn9d9IGjs6XzKG7GYAriSwPVayrcHYhw2KiMemJl3uEhGPH4PzNYZLKJ5hEUXuNuFChDV-ynKSX_UinzoWtpgQ7eVRkbfdenr9cYw4sF-Gppu&response_mode=form_post&nonce=638592325777495352.ZWQ3ODM5M2EtYzgyYy00NDcyLWI5NmUtOWJlNWNjMDJiMzc3MTQ3NzhlOTctMzQ3YS00OGU0LWI2NzAtNDFkZWFjMzdmNDNi&client_id=c44b4083-3bb0-49c1-b47d-974e53cbdf3c&site_id=501430&cobrandid=106b89c7-ab4e-4963-afb3-004cd2f15cac&client-request-id=ae9f5def-276f-4c7d-833d-012e1b92faaf&x-client-SKU=ID_NET472&x-client-ver=7.5.0.0&sso_reload=true). No menu lateral, clique em **"Aplicativos"** e em seguida selecione **"Registros de aplicativo"**. Clique na opção **"+Novo registro"**. Feito isso, preencha os detalhes do aplicativo:

*   **Nome:** defina o nome do aplicativo;
    
*   **Tipos de conta com suporte:** selecione um tipo de conta. Recomenda-se utilizar a opção **“Contas somente neste diretório organizacional (somente Diretório Padrão - único locatário)”**;
    
*   **URI de redirecionamento:** escolha a opção **"Web"** e, no campo ao lado, insira a URI de redirecionamento, que deve ser o endereço do servidor seguido de /mge/genericOauth.mge.
    

Após preencher os campos, clique em **"Registrar"**.

**Importante:** certifique-se de que a aplicação utiliza um certificado HTTPS válido.

![Registrar um aplicativo.gif](https://ajuda.sankhya.com.br/hc/article_attachments/25744979704343)

Na tela que será apresentada, clique no menu **"Visão geral"**. Copie os valores de **"ID do aplicativo (cliente)"** e **"ID do diretório (locatário)"**. Essas informações serão inseridas posteriormente no **Sankhya Om**, na tela [Configuração Oauth](https://ajuda.sankhya.com.br/hc/pt-br/articles/4410197622295-Configura%C3%A7%C3%B5es-OAuth).

![Visão Geral.png](https://ajuda.sankhya.com.br/hc/article_attachments/25745314637463)

Agora, acesse no menu **"Certificados e segredos"** a aba **"Segredos do cliente"** e clique em **"+Novo segredo do cliente"**. Defina uma descrição e selecione o prazo de validade para o segredo. Clique em **"Adicionar"**.

![Adicionar um segredo.png](https://ajuda.sankhya.com.br/hc/article_attachments/25745314641815)

Depois, no campo **"Valor"** copie a chave gerada (Secret ID). Essa informação também será utilizada na tela Configuração Oauth.

Acesse o menu **"Permissões de APIs"** e clique em **"Adicionar uma permissão"** e em **"Permissões delegadas"**. No campo **"Selecionar permissões"** busque as permissões necessárias. Sugestão de permissões:

*   email;
    
*   offline\_access;
    
*   openid;
    
*   profile;
    
*   Mail.Send;
    
*   SMTP.Send;
    
*   User.Read.
    

Clique em **"Adicionar permissões"** após selecionar as permissões desejadas.

![Permissões de APIs.png](https://ajuda.sankhya.com.br/hc/article_attachments/25745314645399)

Por fim, marque a opção **"Conceder consentimento do administrador para o Diretório padrão"**.

### **Configurações do protocolo OAuth no Sankhya Om**

Acesse agora a tela [Configurações OAuth](https://ajuda.sankhya.com.br/hc/pt-br/articles/4410197622295-Configura%C3%A7%C3%B5es-OAuth) para a utilização do protocolo OAuth no **Sankhya Om**.

![Outlook Oauth.png](https://ajuda.sankhya.com.br/hc/article_attachments/25747498870551)

Insira um nome para a configuração. Depois, em **"Provedor"** selecione **"Outlook"**.

Informe o **"Nome da API"** cadastrado no Microsoft. Em seguida, insira o **"Client ID"** e o **"Client Secret"** relacionado ao aplicativo criado.

Preencha os campos a seguir com as informações específicas para o Outlook:

**Redirect URI:** /mge/genericOAuth.mge

**Scopes:** offline\_access https://outlook.office.com/SMTP.Send

Com os campos preenchidos, clique em **"Salvar"**.

Após realizar a configuração OAuth, deve-se vincular as configurações do servidor SMTP. Para isso, na conta SMTP cadastrada na tela [Servidor SMTP](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044593494-Servidor-SMTP), acione a marcação **"Autenticar com OAuth"** e no campo **"Configurações OAuth"** busque o registro cadastrado na etapa anterior:

![Configura\_\_es\_no\_Sankhya\_\_1\_.gif](https://ajuda.sankhya.com.br/hc/article_attachments/25747184201239)

Após selecionar a configuração OAuth, realize a autenticação e confirme o processo. 

Pode-se certificar de que a configuração foi realizada com sucesso a partir do envio de um e-mail de teste.

[\[voltar ao topo\]](#top)