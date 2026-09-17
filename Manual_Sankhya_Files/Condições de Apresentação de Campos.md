# Condições de Apresentação de Campos

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/4404582004759-Condi%C3%A7%C3%B5es-de-Apresenta%C3%A7%C3%A3o-de-Campos](https://ajuda.sankhya.com.br/hc/pt-br/articles/4404582004759-Condi%C3%A7%C3%B5es-de-Apresenta%C3%A7%C3%A3o-de-Campos)

---

# Condições de Apresentação de Campos

![Versão - 32x32 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313285898775) **Versão:** a partir da 4.7

---

Esse é um recurso existente em configurações avançadas de campos, que permite ao modelador condicionar os campos que serão exibidos no formulário em virtude de um determinado dado preenchido em outro campo ou outra regra definida no script de condição de apresentação.

Sendo assim, esse recurso será utilizado quando houver a necessidade dos campos serem apresentados para preenchimento devido a um determinado dado preenchido anteriormente em outro campo do formulário e, dessa forma, o executor de tarefas terá uma melhor experiência de uso do sistema, pois irá visualizar apenas os campos que são realmente requeridos.

Nesse artigo, você terá acesso aos seguintes tópicos:

---

1.  [Caso de Uso](#casodeuso)                                                                       
2.  [Configurando a condição de apresentação de campos](#configurandoacondi%C3%A7%C3%A3odeapresenta%C3%A7%C3%A3odecampos)
3.  [Resultados](#resultados)

---

#### **Caso de Uso**

No processo de [Cadastro de Clientes](https://drive.google.com/file/d/1Niouu_at4ps-8Y-rAm3bXrov9tQqLIT_/view), na abertura do processo, o solicitante do cadastro deve preencher os dados gerais do cadastro do cliente. Utilizando o recurso de condição de apresentação de campos, iremos definir que, quando for informado o tipo de cliente, serão exibidos campos específicos para o tipo pessoa física ou tipo pessoa jurídica.

Com isso, iremos visualizar apenas os campos que realmente são de preenchimento necessário para um desses tipos, o que deixa os campos do formulário mais concisos e diminui a possiblidade de preenchimento desnecessário dos mesmos.

[\[voltar ao topo\]](#top)

#### **Configurando a condição de apresentação de campos**

Em nosso exemplo, iremos condicionar a apresentação dos campos **"Sexo"**, **"Razão social"**, **"Inscrição Estadual"** e **"Insc. Estadual na UF"** em função do dado preenchido no campo **"Tipo de pessoa"**.

Então, caso o campo Tipo de pessoa seja preenchido com a opção **"Pessoa física"**, o campo Sexo será apresentado para preenchimento e os demais campos serão ocultados do formulário.

De outra forma, sendo selecionada a opção **"Pessoa jurídica"** no campo Tipo de pessoa, ocorrerá o inverso, ou seja, o campo Sexo será ocultado do formulário e os demais serão exibidos para preenchimento.

Em nosso caso de uso, estamos utilizando o formulário do tipo nativo para configurar a condição de apresentação de um campo. Para isso, basta acessar as configurações do formulário através do botão ![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4404571204631):

![flow14.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4404627146775)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Representação do Processo</strong></span></p></td></tr></tbody></table>

Em seguida, devemos selecionar o campo que irá condicionar a apresentação e clicar no botão ![mceclip0.png](https://ajuda.sankhya.com.br/hc/article_attachments/4404627205015) **"Configurações avançadas de campo"**.

![flow15.gif](https://ajuda.sankhya.com.br/hc/article_attachments/4404619922455)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto; height: 22px;"><tbody><tr style="height: 22px;"><td style="width: 100%; height: 22px;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Configurações avançadas de campos</strong></span></p></td></tr></tbody></table>

Na sequência, acessamos a aba **"Condição de apresentação"** e definimos a condição de apresentação para o campo Sexo. Após isso, realizamos o mesmo procedimento para os demais campos que terão a apresentação condicionada:

![mceclip2.png](https://ajuda.sankhya.com.br/hc/article_attachments/4404627586839)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Script de condição de apresentação de campos</strong></span></p></td></tr></tbody></table>

**Script:**

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black50"><em>// Retorna campo 'Sexo' se campo 'Tipo de Pessoa' for igual a pessoa física (F)</em></span><span class="wysiwyg-color-black30"><br></span><span class="wysiwyg-color-yellow120">return</span><span class="wysiwyg-color-blue70"> getCampo</span><span class="wysiwyg-color-black">(</span><span class="wysiwyg-color-cyan110">"TIPPESSOA"</span><span class="wysiwyg-color-black">) </span><span class="wysiwyg-color-yellow120">== </span><span class="wysiwyg-color-cyan110">"F"</span><span class="wysiwyg-color-black">;</span></span></pre></td></tr></tbody></table>

**Outra forma de escrever o script seria:**

<table style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-black50"><em>// Retorna campo 'Sexo' se campo 'Tipo de Pessoa' for igual a pessoa física (F)</em></span><span class="wysiwyg-color-black30"><br></span></span><span class="wysiwyg-color-black"><span class="wysiwyg-font-size-medium"><strong>var </strong></span></span><span class="wysiwyg-font-size-medium wysiwyg-color-blue80">tipoPessoa</span><span class="wysiwyg-font-size-medium wysiwyg-color-yellow120"> = </span><span class="wysiwyg-color-blue80"><span class="wysiwyg-font-size-medium">getCampo</span></span><span class="wysiwyg-color-black"><span class="wysiwyg-font-size-medium">(<span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><span class="wysiwyg-color-cyan110">"TIPPESSOA"</span></span>);</span><span class="wysiwyg-font-size-medium"><br></span></span><span class="wysiwyg-color-yellow120"><span class="wysiwyg-font-size-medium">if</span></span><span class="wysiwyg-color-black"><span class="wysiwyg-font-size-medium"> (<span class="wysiwyg-font-size-medium wysiwyg-color-blue80">tipoPessoa</span> </span></span><span class="wysiwyg-color-yellow120"><span class="wysiwyg-font-size-medium">==</span></span><span class="wysiwyg-color-cyan110"><span class="wysiwyg-font-size-medium"> "F"</span></span><span class="wysiwyg-color-black"><span class="wysiwyg-font-size-medium">) {<br></span></span><span class="wysiwyg-color-yellow120"><span class="wysiwyg-font-size-medium">return true</span></span><span class="wysiwyg-color-black"><span class="wysiwyg-font-size-medium">;<br>} </span></span><span class="wysiwyg-color-yellow120"><span class="wysiwyg-font-size-medium">else</span></span><span class="wysiwyg-color-black"><span class="wysiwyg-font-size-medium"> {<br></span></span><span class="wysiwyg-color-yellow120"><span class="wysiwyg-font-size-medium">return false</span></span><span class="wysiwyg-color-black"><span class="wysiwyg-font-size-medium">;<br></span><span class="wysiwyg-font-size-medium">}</span></span><span class="wysiwyg-color-green120 wysiwyg-font-size-medium"><br></span></pre></td></tr></tbody></table>

**Observação:** outros métodos de consulta também podem ser utilizados em scripts para condicionar a apresentação de campos, conforme a imagem abaixo:

![flow16.png](https://ajuda.sankhya.com.br/hc/article_attachments/4404620290455)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Funções de Consultas para condicionar a apresentação de campos</strong></span></p></td></tr></tbody></table>

Na imagem abaixo, note que, ao configurar uma condição de apresentação na grade de campos, é apresentado o símbolo ![mceclip5.png](https://ajuda.sankhya.com.br/hc/article_attachments/4404620341143) que sinaliza essa configuração:

![mceclip3.png](https://ajuda.sankhya.com.br/hc/article_attachments/4404620320791)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Ícone que possui condição de apresentação&nbsp;</strong></span></p></td></tr></tbody></table>

[\[voltar ao topo\]](#top)

#### **Resultados**

Realizadas as configurações de condições de apresentações no ambiente de modelagem, agora podemos visualizar na [Lista de Tarefas](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044595434-Lista-de-Tarefas) o resultado dessas configurações.

Para isso, acesse o processo configurado e selecione no campo **"Tipo de pessoa"** uma das opções. Assim, é possível visualizar campos que são apresentados quando selecionamos o tipo Pessoa Física:

![mceclip6.png](https://ajuda.sankhya.com.br/hc/article_attachments/4404627767831)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Formulário na Lista de Tarefas - Pessoa Física</strong></span></p></td></tr></tbody></table>

E os campos exibidos quando selecionado o tipo Pessoa Jurídica:

![mceclip7.png](https://ajuda.sankhya.com.br/hc/article_attachments/4404627774999)

<table class=" wysiwyg-text-align-justify" style="border-collapse: collapse; width: 100%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><p class="wysiwyg-text-align-center"><span class="wysiwyg-font-size-small wysiwyg-color-black30"><strong>Formulário na Lista de Tarefas - Pessoa Jurídica</strong></span></p></td></tr></tbody></table>

Dessa forma, foram apresentados apenas os campos necessários para preenchimento para cada tipo, o que torna a visualização de campos do formulário mais enxuta e melhora a experiência para os executores de tarefas.

[\[voltar ao topo\]](#top)