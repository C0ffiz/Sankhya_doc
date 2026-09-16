# Portabilidade Whintor

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/6516851968919-Portabilidade-Whintor](https://ajuda.sankhya.com.br/hc/pt-br/articles/6516851968919-Portabilidade-Whintor)

---

# Portabilidade Whintor

Através dessa ferramenta, você conseguirá exportar os dados de um legado Winthor, e realizar as transformações necessárias para convertê-los em um modelo Sankhya. Ao final do processo, essa ferramenta irá disponibilizar os dados convertidos em templates que sejam aceitos pelo [Importador de Dados](https://ajuda.sankhya.com.br/hc/pt-br/articles/5874837664023-Importador-de-Dados) e, dessa forma, o consultor conseguirá efetuar a carga dos dados em uma base Sankhya. 

**Essa documentação aborda os seguintes tópicos:**

<table class=" wysiwyg-text-align-center" style="border-collapse: collapse; width: 98.4286%; height: 112px;"><tbody><tr><td style="width: 26.7602%;"><a href="#instala%C3%A7%C3%A3odaportabilidadewhintor" target="_self"><img src="/hc/article_attachments/42311140074391" alt="inst.png" width="156" height="144"></a></td><td class="wysiwyg-text-align-center" style="width: 10.2082%;"><img src="/hc/article_attachments/42311140078871" alt="seta.png" width="77" height="23"></td><td class="wysiwyg-text-align-center" style="width: 26.8714%;"><a href="#conex%C3%A3ocomobancodedados" target="_self"><img src="/hc/article_attachments/42311152976919" alt="conex_o3.png" width="157" height="145"></a></td><td class="wysiwyg-text-align-center" style="width: 10.3116%;"><img src="/hc/article_attachments/42311140078871" alt="seta.png" width="77" height="23"></td><td class="wysiwyg-text-align-left" style="width: 35.097%;"><a href="#configura%C3%A7%C3%B5esgeraiseextra%C3%A7%C3%A3odosdados" target="_self"><img src="/hc/article_attachments/42311140081687" alt="configu.png" width="155" height="145"></a></td></tr></tbody></table>

###     ![clique.png](https://ajuda.sankhya.com.br/hc/article_attachments/42311152979479)

---

####  **I****nsta****lação da Portabilidade Whintor**

Para efetuar o download do Exportador de Dados, você primeiramente precisa estar logado na Central de Ajuda; após isso, acesse a categoria [Aceleradores de Implantação](https://ajuda.sankhya.com.br/hc/pt-br/categories/4414620572695-Aceleradores-de-Implanta%C3%A7%C3%A3o) e, em seguida, vá até a seção [Ferramentas](https://ajuda.sankhya.com.br/hc/pt-br/sections/7172302946327-Ferramentas-) e clique no artigo [Portabilidade Whintor](https://ajuda.sankhya.com.br/hc/pt-br/articles/7172352909975-Portabilidade-Whintor):

![whintor.gif](https://ajuda.sankhya.com.br/hc/article_attachments/7174289056151)

Feito isso, execute o arquivo em uma máquina que possua acesso ao banco de dados que terá seus dados extraídos. Dessa forma, o sistema irá verificar, caso haja conexão com a internet, se a versão executada é a mais recente.

<table style="border-collapse: collapse; width: 92.5692%; margin-right: auto; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre><strong><img src="/hc/article_attachments/42311152980503" alt="Atenção FINAL.png"> É muito importante que a extração seja realizada sempre com a última versão do <br>         sistema que está disponível.<br></strong></pre></td></tr></tbody></table>

Se a versão executada for a mais atual, o sistema será aberto conforme imagem a seguir:

![exportador.png](https://ajuda.sankhya.com.br/hc/article_attachments/7174336026391)

[\[voltar ao topo\]](#top)

---

####  **Conexão com o banco de dados**

Para realizar a conexão com o banco de dados, preencha os campos abaixo:

*   **Prospect / Cliente:** Informe nesse campo qual o nome do cliente.
*   **Sistema Legado:** Aqui é exibido o sistema legado que terá seus dados extraídos, no caso, o **"WINTHOR"**.
*   **Banco de Dados:** Indica o banco de dados que terá seus dados extraídos.
*   **Host / IP:** Informe o endereço de acesso ao servidor do banco de dados.
*   **SID / Instância:** Preencha aqui o nome ou instância do banco de dados.
*   **Porta:** Informe nesse campo qual a porta que será utilizada para a conexão com o banco de dados.
*   **Usuário:** Preencha esse campo com um usuário que tenha permissão de leitura no banco de dados.
*   **Senha:** Informe aqui a senha de acesso do usuário informado.

Feito isso, clique no botão **"Abrir Conexão"**. Assim, o sistema tentará conectar com o banco de dados. Caso ocorra alguma falha, será apresentada uma mensagem de erro e os dados de conexão deverão ser conferidos.

**Observação:** pode haver casos em que a conexão seja realizada com sucesso porém, o banco de dados não atenda aos requisitos necessários; desse modo, não será possível efetuar a extração dos dados por meio do Exportador de Dados e o sistema exibirá uma mensagem informando a situação.

Com a conexão estabelecida e validados os requisitos de banco, passaremos para a próxima etapa: [Configurações gerais e extração dos dados](#configura%C3%A7%C3%B5esgeraiseextra%C3%A7%C3%A3odosdados).

[\[voltar ao topo\]](#top)

---

####  **Configurações gerais e extração dos dados**

Após realizar a conexão com o banco de dados, a tela abaixo será apresentada:  
![exportador2.png](https://ajuda.sankhya.com.br/hc/article_attachments/7163701754903)

Nessa tela você deverá realizar as seguintes configurações:

*   **Período:** Escolha aqui o período inicial e final para a extração de dados.
*   **Número de Threads:** Esse campo trata da quantidade de extrações simultâneas de tabelas que serão realizadas. Por padrão, a ferramenta nos traz o valor **"4"**, podendo esse número ser alterado para qualquer valor entre **"1"** e **"8"**.
*   **Configurações TOP's:** Nessa seção você deve informar as TOP's que deseja utilizar. Assim, o exportador usará essas informações nas transformações das tabelas que necessitam desses dados (TGFCAB, TGFITE).

**Notas:**

*   Caso queira restaurar as TOP's, acione o botão ![botao-retornar-padrao.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/15642280232087). Assim, serão retornadas às configurações padrão.
*   Apenas as TOP's **"2000 - Pedido de Compra"**, **"3100 - Pedido de Venda"**, **"4101 - Despesas Diversas (avulsa)"** e **"Receitas Diversas (avulsa)"** estão disponíveis.

Após realizar as configurações acima, o próximo passo é selecionar a(s) tabela(s) que você deseja realizar a exportação:

![exportador5.png](https://ajuda.sankhya.com.br/hc/article_attachments/7174628850839)

Nessa listagem, todas as tabelas e colunas necessárias no processo são validadas, sendo que, se houver alguma que não esteja atendendo aos requisitos necessários, um pop-up será apresentado com a inconsistência encontrada e, consequentemente, o processo será abortado, impossibilitando a exportação.

Escolhendo as tabelas, basta clicar no botão **"Executar"**. Com o processo de exportação iniciado, você poderá acompanhar o andamento por meio da coluna "**Status"**, sendo que, as tabelas marcadas como **"PENDENTE"** ou **"FALHA"** ainda não foram extraídas, já as que tiveram a exportação finalizada, apresentarão a informação **"OK"**:

![exportador3.gif](https://ajuda.sankhya.com.br/hc/article_attachments/7163913909911)

Além da lista de tabelas, você pode acompanhar o progresso da exportação por meio da barra na parte inferior do sistema, que é carregada conforme o andamento, e do percentual de evolução.

---

*   Se houver a necessidade de parar o processo, clique no botão **"Cancelar"**, assim, o sistema exibirá a mensagem:

_**"Deseja encerrar a execução?**_

_**ATENÇÃO: Caso confirme a ação, os arquivos exportados, pela operação atual, serão deletados."**_

Clicando em **"OK"**, o processo será interrompido e os arquivos de exportação já gerados serão excluídos, sendo necessário realizar o processo de exportação desde o início. Optando por **"Cancelar"**, o processo continuará e o sistema prosseguirá na geração dos arquivos.

---

*   Caso você clique no botão **"Fechar"**, será exibida a seguinte mensagem, solicitando sua confirmação:

**_"Confirmação_**

**_Tem certeza que deseja sair do sistema?"_**

Clicando em **"Ok"** o sistema será encerrado, e caso haja alguma exportação em andamento, o processo será interrompido e os arquivos já gerados serão excluídos, necessitando uma nova exportação de todos os dados. Caso você decida **"Cancelar"**, o sistema continuará aberto e se houver alguma exportação em andamento o processo será retomado.

---

<table style="border-collapse: collapse; width: 92.5692%; margin-right: auto; margin-left: auto;"><tbody><tr><td class="wysiwyg-text-align-center" style="width: 100%;"><img src="/hc/article_attachments/42311140087063" alt="essencial FINAL (1).png"></td></tr><tr><td class="wysiwyg-text-align-justify" style="width: 100%;"><p>Se você selecionar para exportação uma tabela que possua dependências e tente executar, será apresentada a seguinte mensagem: <strong><em>"Deseja incluir na exportação as demais tabelas?"</em></strong>:</p><p><img src="/hc/article_attachments/42311140087703" alt="exportador4.gif"></p></td></tr></tbody></table>

---

Após a finalização da exportação, o Exportador de Dados exibirá a seguinte mensagem:

_**"Sucesso**_  
_**Extração concluída com sucesso. Os arquivos se encontram no diretório export da pasta do sistema."**_

Assim, acesse o diretório onde o sistema foi executado, nele você encontrará a pasta **"export"** que irá conter um arquivo "_zip"_ que reúne todos os arquivos que foram gerados e o log de execução do processo:

![export1.png](https://ajuda.sankhya.com.br/hc/article_attachments/6569861752343)

[\[Voltar ao topo\]](#top)

---

 **![acesse também FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16695791886999)**Acesse também:

[Acessos - Importador de Dados](https://ajuda.sankhya.com.br/hc/pt-br/articles/6327856217879-Acessos-Importador-de-Dados)

[Importador de Dados](https://ajuda.sankhya.com.br/hc/pt-br/articles/5874837664023-Importador-de-Dados)

[\[voltar ao topo\]](#top)