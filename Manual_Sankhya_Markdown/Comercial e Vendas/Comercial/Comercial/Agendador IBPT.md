# Agendador IBPT

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/5692677947287-Agendador-IBPT](https://ajuda.sankhya.com.br/hc/pt-br/articles/5692677947287-Agendador-IBPT)

---

# Agendador IBPT

 **![Módulo](https://ajuda.sankhya.com.br/hc/article_attachments/42312226622487) Módulo:** Comercial > Avançado > Agendadores **![Versão](https://ajuda.sankhya.com.br/hc/article_attachments/42312210099223) Versão disponível:** A partir da 4.12

---

Por meio desta tela será possível agendar a atualização automática dos percentuais das cargas tributárias referentes a Lei da Transparência 12.741/2012. Estas informações serão obtidas por meio da integração do **Sankhya Om** com o site [API De Olho no Imposto](https://deolhonoimposto.ibpt.org.br/). 

![vantagens\_\_3\_.png](https://ajuda.sankhya.com.br/hc/article_attachments/5728110047255)

---

Para conhecer as funcionalidades dessa tela, clique nos links abaixo:

<table style="border-collapse: collapse; width: 100%; height: 90px;" border="1"><tbody><tr style="height: 24px;"><td style="width: 50%; height: 24px;" colspan="2"><h4 id="h_01HNJXJTYEJ6CP863C0X19MC59" class="wysiwyg-text-align-center"><strong>Funcionalidades da Tela</strong></h4></td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;<a class="topiclink" href="#configuracoesdarotina">Configurações da Rotina</a><br></span></td><td style="width: 50%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;<a class="topiclink" href="#abahorarios">Aba Horários</a></span></td></tr><tr style="height: 22px;"><td style="width: 50%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;<a class="topiclink" href="#abafrequenciaagendamento">Aba Frequência Agendamento</a>&nbsp;&nbsp;</span></td><td style="width: 50%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;<a class="topiclink" href="#abaconfiguracoes">Aba Configurações</a></span></td></tr><tr><td style="width: 50%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;<a class="topiclink" href="#abahistorico">Aba Histórico</a></span></td><td style="width: 50%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;</span></td></tr></tbody></table>

### **Configurações da rotina**

Primeiramente é necessário cadastrar o Token da empresa no campo **"Token IBPT"** localizado na tela [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893), aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893#abageral). Esta informação pode ser adquirida no site [https://deolhonoimposto.ibpt.org.br/](https://deolhonoimposto.ibpt.org.br/). 

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td style="width: 100%;"><pre><span class="wysiwyg-font-size-medium"><span style="font-weight: 400;"><span class="wysiwyg-color-black70"><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42312210099607" alt="Atenção"> O sistema não irá identificar se o Token pertence ao CNPJ da Empresa, e se o mesmo está </span><br><span class="wysiwyg-color-black70">válido ou expirado, portanto, deve-se verificar o status do Token no portal do IBPT.</span></span></span></pre></td></tr></tbody></table>

![aba-geral.png](https://ajuda.sankhya.com.br/hc/article_attachments/21046960017303)

Feito isso, acesse a tela Agendador IBPT para realizar as configurações do agendamento. Assim, para iniciar o cadastro acione o botão ![Botão](https://ajuda.sankhya.com.br/hc/article_attachments/15992628771351) **"Cadastrar Agendamento Tarefa"**, em seguida, no painel principal preencha o campo **"Descrição agendamento"** e acione a marcação **"Ativo"**. 

![Agend-ibpt-aba-horarios.png](https://ajuda.sankhya.com.br/hc/article_attachments/21047069371799)

**Nota:** poderá ser feito o acompanhamento do status da última execução do agendador através do campo **"Status Ú****ltima Execução"**.

---

Agora, configure as abas da tela, sendo elas:

### **A****ba Horários**

Nesta aba, preencha o campo **"Próxima execução em"** com a data e o horário da próxima execução. Informe também a **"Data Final de Execução"** e o horário final.

![aba-horarios.png.png](https://ajuda.sankhya.com.br/hc/article_attachments/21048239325207)

[\[voltar ao topo\]](#top)

### **A****ba Frequência Agendamento**

Configure nesta aba, a frequência de execução do agendador.

![aba-frequencia-agendamento.png](https://ajuda.sankhya.com.br/hc/article_attachments/21048271484439)

Assim, informe o horário da **"1° Execução"**, e caso seja necessário adicione mais execuções acionando o botão ![botão adicionar novo horário FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/21049093267095) **"Adicionar novo horário para execução"** ou remova todos os horários de execução por meio do botão ![botão remover todos os horários de execução FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/21049150106903) **"Remover todos os horários de execução"**.

Além do horário, poderá ser definido a frequência das execuções do agendador em:

*   **Diário:** clicando nesta opção, será efetuada diariamente;
*   **Semanal** e **Mensal:** selecionando uma destas opções, serão exibidas para marcação, os dias da semana e do mês, respectivamente. 

[\[voltar ao topo\]](#top)

### **A****ba Configurações**

Nesta aba, o campo **"Empresa"** deverá ser preenchido conforme as seguintes regras:

*   Informe neste campo a empresa que não utiliza a aba [Impostos/Informações por Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos#abaimpostosinformaesporempresa), da tela [Cadastros de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos#top) para definir os percentuais de carga tributária conforme a Lei da Transparência n° 12.741/2012.
*   Caso a empresa utilize essa aba, o preenchimento deste campo não será exigido. No entanto, será necessário informar ao menos uma empresa na sub-aba **"Empresas"** desta tela.

![aba-configuração.png](https://ajuda.sankhya.com.br/hc/article_attachments/21048271510295)

Nesta tela, ao habilitar a marcação **"Somar cargas trib. Estad. e Fed. no campo % Carga Média Trib. Nacional?"**, a seguinte mensagem de aviso surgirá:

**_"Os percentuais dos campos ‘% Carga Média Trib. Estadual:’ e ‘% Carga Média Trib. Federal:’ serão excluídos dos produtos de Origem 0, 4, 5, 6 ou 7 (Nacional) e, serão somados e informados no campo ‘% Carga Média Trib. Nacional:"_**

Isso significa que ao executar o Agendador com a marcação habilitada, serão excluídas todas as informações dos campos **"% Carga Média Trib. Estadual"** e **"% Carga Média Trib. Federal"** quando se tratar de produtos de origem 0, 4, 5, 6 ou 7 (nacional), preenchendo somente o campo **"% Carga Média Trib. Nacional"** com a soma dos percentuais definidos para a Carga Média Tributária Estadual e Federal.

Para produtos de origem 1, 2, 3 ou 8 (importado), o percentual do campo % Carga Média Trib. Estadual será excluído e substituído no campo % Carga Média Trib. Nacional. 

**Nota:** a funcionalidade da marcação não impacta o campo % Carga Média Trib. Importação, que será preenchido independente dela habilitada ou não.

Se a marcação estiver desligada, os campos % Carga Média Trib. Estadual e % Carga Média Trib. Federal de produtos de origem 0, 4, 5, 6 ou 7 (nacional), serão preenchidos com seus respectivos percentuais e o campo % Carga Média Trib. Nacional ficará vazio.

[\[voltar ao topo\]](#top)

### **A****ba Histórico**

Após a execução das atualizações, será apresentado nesta aba um registro com as seguintes informações básicas da execução: 

*   Nro. Agendamento;
*   Dh. Ini. Execução;
*   Dh. Fim Execução;
*   Tipo de Execução;
*   Mensagem.

![aba-historico.png](https://ajuda.sankhya.com.br/hc/article_attachments/21048271538455)

Após configurar o Agendador, para execução manual ou automática, ao realizar a execução, o sistema validará se o campo **"Token IBPT"** da aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abageral) da tela [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa) está preenchido para a(s) empresa(s) selecionada(s).

Na execução manual, se o sistema não encontrar informação no campo Token IBPT, irá impedir a execução e emitirá a mensagem de erro:

**_"Token não informado para a(s) empresa(s)_** **_(cód. Empresa)_****_. Não é possível realizar a execução."_**

Se o sistema não encontrar informação no campo Token IBPT, seja na execução manual ou automática, ele impedirá a execução e indicará no campo Mensagem desta aba, a seguinte informação:

**_"Token não informado para a(s) empresa(s)_** **_(cód. Empresa)"_**

Se a execução for realizada automaticamente ou pelo botão **"Executar Agora"**, e o sistema validar que o campo Token IBPT da aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa#abageral) da tela [Preferências da Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114893-Prefer%C3%AAncias-da-Empresa) está preenchido para a empresa selecionada, então a execução será permitida normalmente, e apresentará no campo Mensagem, desta aba, a seguinte informação:

**_"Execução concluída com sucesso!"_**

Com as configurações acima efetuadas, quando for executada a atualização automática, ou por meio do botão Executar Agora, o sistema irá atualizar os percentuais da carga tributária, da seguinte forma:

*   Quando for informada uma empresa no campo **"Empresa"** da aba **"Configurações"**, o sistema irá atualizar os percentuais de carga tributária da aba [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#abaimpostos), da tela [Cadastros de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-#top);
*   Quando for informado uma ou mais empresas na sub-aba **"Empresas"**, o sistema irá atualizar os percentuais de carga tributária da aba [Impostos / Informações por empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos#abaimpostosinformaesporempresa), da tela Cadastros de Produtos.

**Observação****:** se os campos **"NCM"**, aba Impostos e **"Cód. Exceção NCM"**, aba Geral ambos da tela Cadastro de Produtos forem preenchidos com informações inválidas ou inexistentes, a aplicação IBPT não retornará valores válidos, ou seja, a aplicação retornará com a informação _null_, permanecendo os valores já existentes nos campos.

[\[voltar ao topo\]](#top)