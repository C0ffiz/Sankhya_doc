# Manual de Implantação e Utilização de Álbum de Fotos

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360044602074-Manual-de-Implanta%C3%A7%C3%A3o-e-Utiliza%C3%A7%C3%A3o-de-%C3%81lbum-de-Fotos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044602074-Manual-de-Implanta%C3%A7%C3%A3o-e-Utiliza%C3%A7%C3%A3o-de-%C3%81lbum-de-Fotos)

---

# Manual de Implantação e Utilização de Álbum de Fotos

O álbum de fotos ou seleção de fotos é uma ferramenta criada integrada ao Sankhya Om. Com ela, as empresas do ramo de fotografias poderão agilizar e inovar no processo de escolha de fotos pelos seus clientes. De forma fácil e intuitiva, os clientes recebem acesso a um site de seleção de fotos e um site de votação, onde parentes e amigos poderão ajudar na escolha das fotos.

O processo consiste em lançar uma nota de venda para um determinado parceiro (cliente), e essa nota terá itens que serão os álbuns contratados pelo cliente. Com a nota lançada e confirmada, será possível entrar numa tela de autorização e envio das fotos para que o cliente receba em seu e-mail um link para que a seleção das fotos possa ser feita, e também receberá um link alternativo para enviar para familiares e amigos, esse link permitirá que as pessoas curtam as fotos que mais gostarem, facilitando assim a escolha das fotos pelo cliente. Assim teremos:

<table style="border-collapse: collapse; width: 100%; height: 110px;"><tbody><tr style="height: 22px;"><td style="width: 45.7618%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#configura%C3%A7%C3%B5es" target="_self" rel="undefined">Configurações</a></span></td><td style="width: 9.19039%; height: 22px;">&nbsp;</td><td style="width: 45.0476%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#execu%C3%A7%C3%A3odoprocesso">Execução do Processo</a></span></td></tr><tr style="height: 22px;"><td style="width: 45.7618%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#marcad'%C3%A1guaeredimensionamentodasfotos">Marca D'água e Redimensionamento...</a></span></td><td style="width: 9.19039%; height: 22px;">&nbsp;</td><td style="width: 45.0476%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#utilizandocsscomoutrosarquivos">Utilizando CSS com outros arquivos</a></span></td></tr><tr style="height: 22px;"><td style="width: 45.7618%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#sele%C3%A7%C3%A3odefotos">Seleção de Fotos</a></span></td><td style="width: 9.19039%; height: 22px;">&nbsp;</td><td style="width: 45.0476%; height: 22px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><a class="topiclink" href="#par%C3%A2metrosutilizadospelaferramenta">Parâmetros utilizados pela ferramenta</a></span></td></tr></tbody></table>

## Configurações 

Primeiramente, você deverá configurar o parâmetro **"Endereço para acesso externo ao WGE - ENDACESSEXTWGE"** com a URL externa ao Sankhya Om, onde a empresa terá acesso, assim essa URL deve ser informada no campo **"Texto"** do parâmetro, por exemplo, _http://fotos.sankhya.com.br/mge_.

![paramtero.png](https://ajuda.sankhya.com.br/hc/article_attachments/9855310615959)

Dessa forma, na tela [Configuração de Envio de Fotos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045111673-Configura%C3%A7%C3%A3o-do-Envio-das-Fotos), serão realizadas as configurações de FTP, selecione o grupo de produtos para álbuns, arquivos de customização do site de seleção de fotos, modelo de e-mail e se a empresa utilizará o questionário ou não.

![MEF01.png](https://ajuda.sankhya.com.br/hc/article_attachments/360087185973)

Na seção **"FTP das Fotos"** da tela, informe o **"Usuário"** do FTP e sua **"Senha"**, além do **"Endereço"**, sendo este, a porta do FTP que conterá as fotos dos clientes. É possível que as fotos fiquem em um FTP externo ou em um computador local que executa o Sankhya Om, uma vez que, para que permaneça no computador local é necessário instalar um servidor de FTP e criar uma pasta na sua máquina e para ser utilizada pelo FTP; então, após cadastrar as informações do FTP corretamente, clique no botão ![botão Testar-ftp.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16644696331799) **"Testar FTP"** para verificar a veracidade dos dados cadastrados.

Já na seção **"Aparência do site de fotos"**, você informará o endereço do repositório de arquivos para a **"Logo do Site"** e para a **"CSS externo do site"**, assim, deve ser realizado o upload dos arquivos na tela [Repositório de Arquivos](https://ajuda.sankhya.com.br/hc/pt-br/search?utf8=%E2%9C%93&query=Reposit%C3%B3rio+de+Arquivos) e informar nos referidos campos dessa seção apenas o caminho do arquivo no repositório. 

Além disso, lembre-se que, o arquivo de logomarca deve ser no formato **.png**, e o arquivo para CSS precisar possuir o formato **.css**, sendo assim, essa logo será apresentada no topo da tela de seleção de fotos.

No campo **"Arquivo modelo de e-mail p/ envio das fotos"**, insira um modelo de e-mail personalizado, que será enviado para o cliente. Existe um botão para download do modelo padrão, esse modelo nada mais é que um arquivo em linguagem HTML, ele possui algumas variáveis que poderão ser utilizadas para customização, como, por exemplo, abaixo você poderá conferir algumas variáveis que trará diferentes chamados. Observe:

<table style="border-collapse: collapse; width: 100%; height: 260px;"><tbody><tr style="height: 26px;"><td style="width: 6.47616%; height: 26px;">&nbsp;</td><td style="width: 5.33332%; height: 26px;">&nbsp;</td><td class="wysiwyg-text-align-justify" style="width: 88.1905%; height: 26px;"><strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;">&amp;codparc: </span></strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">código do parceiro que está enviando o e-mail.</span></span></td></tr><tr style="height: 26px;"><td style="width: 6.47616%; height: 26px;">&nbsp;</td><td style="width: 5.33332%; height: 26px;">&nbsp;</td><td class="wysiwyg-text-align-justify" style="width: 88.1905%; height: 26px;"><strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;">&amp;nomeparc<span style="font-family: Verdana,Geneva,Arial,sans-serif;">: </span></span></strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">nome do parceiro que está enviando o e-mail.</span></span></td></tr><tr style="height: 26px;"><td style="width: 6.47616%; height: 26px;">&nbsp;</td><td style="width: 5.33332%; height: 26px;">&nbsp;</td><td class="wysiwyg-text-align-justify" style="width: 88.1905%; height: 26px;"><strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;">&amp;codprojeto<span style="font-family: Verdana,Geneva,Arial,sans-serif;">: </span></span></strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">código do projeto (código do evento).</span></span></td></tr><tr style="height: 26px;"><td style="width: 6.47616%; height: 26px;">&nbsp;</td><td style="width: 5.33332%; height: 26px;">&nbsp;</td><td class="wysiwyg-text-align-justify" style="width: 88.1905%; height: 26px;"><strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;">&amp;nomeprojeto<span style="font-family: Verdana,Geneva,Arial,sans-serif;">: </span></span></strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">identificação do projeto (identificação do evento).</span></span></td></tr><tr style="height: 26px;"><td style="width: 6.47616%; height: 26px;">&nbsp;</td><td style="width: 5.33332%; height: 26px;">&nbsp;</td><td class="wysiwyg-text-align-justify" style="width: 88.1905%; height: 26px;"><strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;">&amp;razsoc<span style="font-family: Verdana,Geneva,Arial,sans-serif;">: </span></span></strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">razão social da empresa.</span></span></td></tr><tr style="height: 26px;"><td style="width: 6.47616%; height: 26px;">&nbsp;</td><td style="width: 5.33332%; height: 26px;">&nbsp;</td><td class="wysiwyg-text-align-justify" style="width: 88.1905%; height: 26px;"><strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;">&amp;datasis<span style="font-family: Verdana,Geneva,Arial,sans-serif;">: </span></span></strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">data do sistema (no momento do envio do e-mail).</span></span></td></tr><tr style="height: 26px;"><td style="width: 6.47616%; height: 26px;">&nbsp;</td><td style="width: 5.33332%; height: 26px;">&nbsp;</td><td class="wysiwyg-text-align-justify" style="width: 88.1905%; height: 26px;"><strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;">&amp;horasis<span style="font-family: Verdana,Geneva,Arial,sans-serif;">: </span></span></strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">hora do sistema (no momento do envio do e-mail).</span></span></td></tr><tr style="height: 26px;"><td style="width: 6.47616%; height: 26px;">&nbsp;</td><td style="width: 5.33332%; height: 26px;">&nbsp;</td><td class="wysiwyg-text-align-justify" style="width: 88.1905%; height: 26px;"><strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;">&amp;codacesso<span style="font-family: Verdana,Geneva,Arial,sans-serif;">: </span></span></strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">traz o código do acesso para o parceiro acessar o link de edição.</span></span></td></tr><tr style="height: 26px;"><td style="width: 6.47616%; height: 26px;">&nbsp;</td><td style="width: 5.33332%; height: 26px;">&nbsp;</td><td class="wysiwyg-text-align-justify" style="width: 88.1905%; height: 26px;"><strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;">&amp;link_edicao<span style="font-family: Verdana,Geneva,Arial,sans-serif;">: </span></span></strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">traz o link de edição das fotos.</span></span></td></tr><tr style="height: 26px;"><td style="width: 6.47616%; height: 26px;">&nbsp;</td><td style="width: 5.33332%; height: 26px;">&nbsp;</td><td class="wysiwyg-text-align-justify" style="width: 88.1905%; height: 26px;"><strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;">&amp;link_votacao<span style="font-family: Verdana,Geneva,Arial,sans-serif;">: </span></span></strong><span style="font-family: Verdana, Geneva, Arial, sans-serif;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">traz o link de votação das fotos.</span></span></td></tr></tbody></table>

![dica FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42310808291607) Recomendamos que você utilize o modelo padrão como base para sua personalização.

Após realizar a configuração do grupo de produtos dos álbuns, você deve configurar na TOP de venda que será utilizada nos eventos, habilite a marcação **"Integra Evento"** da aba [Geral](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abageral) para que, assim, o sistema estará apto para realizar o lançamento de notas de venda com álbuns de fotos.

Em seguida, você irá realizar o cadastro do questionário na tela [Questionário Pesquisa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044597514-Question%C3%A1rio-Pesquisa), onde esse questionário consiste na definição de um nome para o mesmo e cadastrar as perguntas, sendo que, para cada uma delas terá um campo **"Texto"** para escrever o texto da pergunta. Já no campo **"Tipo"**, será definido o tipo da resposta; além da marcação **"Pergunta Obrigatória"**, onde será configurado se a pergunta a ser realizada será obrigatório ou não.

Depois de criar o questionário, você poderá configurar o projeto, para isso, na tela [Projetos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045109073-Projetos), preencha os campos com as informações corretas. É importante que no campo **"Questionário"** dessa tela, seja informado o questionário criado anteriormente para que assim, o cliente possa responder às perguntas para cada álbum quando estes forem confirmados por meio do link da seleção de fotos.

**Nota:** o campo Questionário será exibido quando o parâmetro **"Permite cadastro de questionário** **no projeto - QUESTPROJETO"** for habilitado.

Para realizar o cadastro dos álbuns, deve-se primeiramente, cadastrar um produto para cada tipo de álbum no [Cadastro de Produtos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045112113-Cadastro-de-Produtos-), sendo que, a quantidade de fotos em cada álbum será escolhida no lançamento da nota. Deve-se ainda, configurar todos os produtos ábuns vinculados ao mesmo Grupo de Produto que representa os álbuns, grupo esse devidamente informado na tela [Configuração de Envio de Fotos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045111673-Configura%C3%A7%C3%A3o-do-Envio-das-Fotos).

[\[voltar ao topo\]](#top)

## Processo

Inicialmente, você deve realizar o lançamento a nota de venda utilizando a TOP criada anteriormente com a marcação Integra Evento habilitada, o Parceiro, e o Projeto correspondente ao Evento onde as fotografias foram feitas.  
Após o lançamento, insira os produtos na nota. Lembre-se ainda que, produtos que não são álbuns também poderão ser acrescidos junto à mesma nota, por exemplo, serviço de filmagens.

Para os produtos que são álbuns, é necessário que você informe o campo **"Qtd. Peças"**, sendo este, o responsável pela definição da quantidade de fotos que formarão o álbum referente ao item.

Cada produto álbum representa apenas 1 álbum, ou seja, caso o cliente deseje dois álbuns do mesmo tipo e mesma quantidade de fotos, não será permitido colocar o valor **"2"** no campo **"Quantidade"**, o correto seria inserir 2 produtos do mesmo código com o campo Quantidade igual a 1.

Depois, o fotográfo responsável deverá copiar as fotos do evento do Parceiro para uma pasta específica no FTP da empresa, por exemplo:

_/fotos/eventos/formaturas/69contabeis/jose\_da\_silva_

Após realizar a cópia das fotos, o caminho das fotos no FTP será utilizado na tela Autorização e Envio das Fotos.

![MEF02.png](https://ajuda.sankhya.com.br/hc/article_attachments/360085996934)

Dessa forma, na tela Autorização e Envio das Fotos, utilize os filtros rápidos e/ou personalizados para encontrar as notas dos parceiros para os quais os e-mails serão enviados.

Quando você der um duplo clique sobre um Parceiro na grade e clicar no botão ![botão Ver-pendências.FINALjpg.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16644863043479) **"Ver Pendências"**, o sistema abrirá a tela [Movimentação Financeira](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045114753-Movimenta%C3%A7%C3%A3o-Financeira) posicionada no título da pendência financeira do referido parceiro.

**Nota:** o sistema deixará vermelha a linha dos parceiros que possuírem pendências financeiras, porém, você poderá enviar o e-mail para esses parceiros normalmente.

Quando os parceiros para o qual você deseja enviar o e-mail forem filtrados, o caminho do FTP deve ser informado no campo **"Pasta no FTP"**.

![ksnip\_20221025-174525.png](https://ajuda.sankhya.com.br/hc/article_attachments/9857215239831)

Após salvar, clique no botão ![botão Gerar-thumbs.FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16644863047959) **"Gerar Thumbs"** para que o sistema verifique as fotos na pasta FTP e crie a pasta **"thumb"** no FTP para a geração de dos thumbnails, sendo estas, versões reduzidas das fotos usadas para agilizar e facilitar a escolha dos clientes no site.

Para gerar as thumbnails para múltiplos parceiros, você pode selecionar os parceiros e em seguida, clicar no botão **"Gerar Thumbnails"**.

Após a geração, você poderá realizar uma visualização prévia do álbum antes de enviar o e-mail para o parceiro por meio do botão ![botão Ver-álbum.FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16644893334551) **"Ver álbum"**.

Para efetivamente enviar o e-mail para os parceiros, selecione as linhas de sua preferência na grade acione o botão ![botão Enviar-email.FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16644893336983) **"Enviar Email"**, assim, o sistema irá realizar uma verificação para garantir que todos os thumbnails foram gerados e então, enviar os e-mails aos parceiros selecionados.

[\[voltar ao topo\]](#top)

## Marca D'água e Redimensionamento das fotos

A ferramenta permitirá que você insira a marca d'água automaticamente nas fotos, para isso, coloque o arquivo **"marcadagua.png"** no FTP. Sendo que, este pode ser colocado em qualquer pasta do FTP que esteja no caminho da pasta do parceiro. Observe o exemplo abaixo:

_/fotos/eventos/formaturas/69contabeis/jose\_da\_silva_

Bom base no exemplo acima, o arquivo poderá ser colocado na pasta **"Fotos"**, **"Eventos"**, **"Formaturas"**, **"69contabeis"** ou **"Jose da silva"**. Caso haja uma pasta diferente de **marcadagua.png**, o sistema dará prioridade ao arquivo mais a fundo no caminho, ou seja, uma marca d’água que esta na pasta **69contabeis**, tem prioridade sobre uma marca d’água colocada na pasta formaturas, e assim por diante.

![Atenção FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16644915125271) É importante que o arquivo da marca d’agua esteja nomeado marcadagua e tenha formato **.png**, ou seja, **"marcadagua.png"**. Qualquer outro tipo de nomenclatura ou formato não será reconhecido pelo sistema.

O sistema fará o redimensionamento das fotos, dessa forma, você não precisará diminuir a resolução das fotos antes de inseri-las no FTP, e ainda, a resolução sempre será reduzida no visualizador, de forma que, você não conseguirá salvar nenhuma foto em alta resolução ou sem a marca d'água.

[\[voltar ao topo\]](#top)

## Utilizando CSS com outros arquivos

Como foi exibido no tópico [Configurações](#configura%C3%A7%C3%B5es) desse artigo, você poderá vincular um arquivo **.css** para customização do site de seleção de fotos que será utilizado pelos clientes da empresa, porém, talvez você tenha que utilizar outras imagens além da logomarca para customizar o site. Assim, crie o arquivo **.css** utilizando como URL do caminho, apenas o nome do arquivo criado, depois, na tela Repositório de Arquivos, faça o upload desse arquivo para a mesma pasta onde está o arquivo **.css**. Dessa forma, considere o exemplo abaixo:

Para mudar o background de onde se encontra a logo do site, pode-se utilizar o .css com o seguinte conteúdo:

  **.topBar{**  
    **background-image: url('bgFotografando.png');**  
  
   **}**

Dessa forma, precisaríamos colocar os arquivos .css e .png na mesma pasta do Repositório, observe:

 _Repo://Fotografando/FotografandoTheme.css_ e _Repo://Fotografando/bgFotografando.png_

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td style="width: 6.57144%;">&nbsp;</td><td style="width: 93.4285%;"><span class="wysiwyg-color-pink120"><strong>Observações:</strong></span></td></tr></tbody></table>

*   Após gerar os thumbnails para uma determinada pasta, se alguma foto for removida da pasta das fotos em resolução normal, é necessário que se apague o thumbnail da foto manualmente também, ou apagar a pasta de thumbnails completamente e usar o sistema para gerar os thumbnails novamente.
*   Após o envio do e-mail para o parceiro, a pasta de fotos desse parceiro não poderá ser alterada, pois ele pode ter começado a selecionar as fotos para os álbuns, e se alguma foto que foi selecionada for removida ou renomeada, irá gerar inconsistência no banco de dados do sistema.

[\[voltar ao topo\]](#top)

## Seleção de fotos

Ao abrir o link de seleção de fotos enviado por email, o cliente visualizará uma tela onde terá o logotipo da empresa, em que, será o configurado na tela Configuração de Envio das Fotos. 

O Código de Acesso será enviado para o cliente junto ao link e após inserí-lo, clique em Entrar, o cliente terá uma tela com as fotografias que foram compartilhadas neste.

As fotos do evento sempre virão ordenadas pela ordem de quantidade de pessoas que curtiram aquela foto. A esquerda será possível ver todos os álbuns negociados pelo cliente na Nota de Venda.

Ao clicar em alguma foto, o sistema irá redimensionar a foto original para uma resolução menor, irá aplicar a marca d’água caso o arquivo **marcadagua.png** exista, e mostrará a foto ao usuário, que poderá navegar entre as fotos usando as setas do teclado ou clicando na seta de **"Anterior"** e **"Próximo"**.

Para fechar o visualizador poderá ser usado o **(X)** que fica no canto superior direito na imagem ou pressionando o botão **"ESC"**.

É mostrado o nome da imagem, caso o cliente queira fazer alguma observação (cortar, clarear, escurecer e etc) sobre alguma foto ao final da seleção.

Para colocar as fotos no álbum é necessário, clique sobre a foto e arraste ela até o álbum desejado.

Também é possível selecionar a foto clicando na seta ![AF03.png](https://ajuda.sankhya.com.br/hc/article_attachments/360088534073) presente no canto inferior direito na miniatura, essa seta aparece ao posicionar o mouse sobre a miniatura.

Note que ao posicionar o mouse sobre a imagem no canto inferior esquerdo é possível visualizar a quantidade de pessoas que curtiram aquela foto, pelo link que foi enviado no email.

Ao clicar em algum álbum específico, o sistema mostrará as fotos que já foram selecionadas para aquele álbum, permitindo utilizar a seta de opções novamente, desta vez para definir alguma foto como Capa ou Contra-Capa.

As fotos definidas como Capa e Contra-Capa não contam como quantidade de fotos do álbum, por esse motivo o sistema permite que sejam inseridas mais fotos do que o álbum suporta, para que depois sejam movidas algumas fotos para capa, ou mesmo para que o usuário insira várias fotos e depois vá filtrando a partir daquelas pré-selecionadas.

**Nota:** o sistema permite que a mesma foto escolhida na capa ou na contra-capa seja também escolhida no corpo do álbum ou em álbuns diferentes.

Os álbuns do tipo poster não terão capa e contra-capa. O  sistema fará a validação para garantir que o usuário não tenha esquecido de preencher completamente o corpo de algum álbum, ou esquecido de preencher a Capa ou Contra-capa, ou até mesmo ter escolhido mais fotos do que o álbum permite.

Na visualização do conteúdo dos álbuns, existem ainda as opções de cópia para outro lugar. Com isso, o cliente conseguirá selecionar uma mesma fotografia no corpo do álbum e na capa. A validação de não permitir fotos repetidas no corpo, capa e contra-capa, ou seja, você não conseguirá repetir uma mesma foto no corpo, na capa ou na contra-capa.

Após resolver as pendências e confirmar a seleção, caso a empresa tenha configurado um questionário, em seguida, ele aparecerá uma vez para cada álbum que o cliente negociou.Além diss, as perguntas marcadas como Obrigatórias ficam em negrito e  com um asterisco vermelho \* e após responder o questionário será apresentado um campo de texto para se digitar observações a serem feitas.

Após Finalizar o sistema mostrará uma mensagem que o deixa ciente da finalização da seleção e os álbuns não poderão mais ser modificados.

Quando houver a confirmação da seleção das fotos, todas as informações deverão ser extraídas da base através de componentes de BI e relatórios.

As Tabelas envolvidas são:

*   TGFPEV (Pedido por Evento)
*   TGFALB (Album)
*   TGFIAL (Item de Álbum)
*   TGFALV (Álbum Votação)
*   TGFQUE (Questionário)
*   TGFPQE (Perguntas do Questionário)
*   TGFRQE (Respostas de Questionário)
*   TGFQAL (Respostas por Álbum)

[\[voltar ao topo\]](#top)

## Parâmetros utilizados pela ferramenta

*   **CONFFTPALBUM** - Configuração de conexão com FTP das fotos.
*   **GRUPOALBUM** - Código do grupo de produto dos produtos álbuns.
*   **MODEMAILALBUM** - Arquivo modelo de e-mail para o envio do email com links.
*   **QUESTPROJETO** - Permite cadastro de questionário no projeto.
*   **FREPBASEFOLDER** - Diretório base para o repositório de arquivos.
*   **ENDACESSEXTWGE** - Endereço para acesso externo ao WGE.

[\[voltar ao topo\]](#top)