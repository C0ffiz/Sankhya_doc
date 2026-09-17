# Como alterar o nível de log do Sankhya Om

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/42562047860887-Como-alterar-o-n%C3%ADvel-de-log-do-Sankhya-Om](https://ajuda.sankhya.com.br/hc/pt-br/articles/42562047860887-Como-alterar-o-n%C3%ADvel-de-log-do-Sankhya-Om)

---

# Como alterar o nível de log do Sankhya Om

**Caminho de acesso:** Menu Principal › Configurações › Avançado › Preferências

**Você encontra neste artigo:**

<table style="border-collapse: collapse;" id="sumario"><tbody><tr><td style="border-color: #999; padding: 8px; vertical-align: top; width: 50%;"><a href="#oque">O que é e para que serve</a><br><a href="#versao-minima">Versão mínima necessária</a><br><a href="#niveis">Os níveis de detalhamento</a><br><a href="#como-alterar">Como alterar o parâmetro SANKHYALOGLEVEL</a></td><td style="border-color: #999; padding: 8px; vertical-align: top; width: 50%;"><a href="#roteiro">Roteiro recomendado de investigação</a><br><a href="#cuidados">Cuidados</a><br><a href="#sem-detalhes">Se o log continuou sem detalhes</a><br><a href="#faq">Perguntas frequentes</a></td></tr></tbody></table>

## O que é e para que serve

O parâmetro `SANKHYALOGLEVEL` controla o nível de detalhamento dos registros de log do Sankhya Om, permitindo aumentar temporariamente as informações registradas durante uma investigação e depois voltar ao comportamento padrão. Você altera o parâmetro com o Sankhya Om no ar, sem reinicializar nada e sem precisar de atualização de versão, desde que o ambiente já esteja no build mínimo exigido. Ele não altera nenhuma regra de negócio, cálculo, processo ou registro de auditoria do Sankhya Om — a mudança afeta apenas a quantidade de informação gravada no log do servidor.

## Versão mínima necessária

O parâmetro `SANKHYALOGLEVEL` está disponível a partir das versões abaixo. Localize a linha de versão do seu ambiente e confira o build:

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Linha de versão</strong></td><td style="border-color: #999; padding: 6px;"><strong>Build mínimo</strong></td></tr><tr><td style="border-color: #999; padding: 6px;">4.33</td><td style="border-color: #999; padding: 6px;">b254</td></tr><tr><td style="border-color: #999; padding: 6px;">4.34</td><td style="border-color: #999; padding: 6px;">b423</td></tr><tr><td style="border-color: #999; padding: 6px;">4.35</td><td style="border-color: #999; padding: 6px;">b766</td></tr><tr><td style="border-color: #999; padding: 6px;">4.36</td><td style="border-color: #999; padding: 6px;">b85</td></tr></tbody></table>

Ambientes em build anterior ao indicado para a sua linha não possuem o parâmetro — nesse caso é necessário atualizar o Sankhya Om antes de usar este recurso. Builds iguais ou superiores ao mínimo indicado para a linha também possuem o parâmetro disponível.

A versão e o build do ambiente aparecem no popup "Sobre a versão", aberto pelo link **Versão** (abaixo da foto do usuário, no menu do perfil), ou podem ser confirmados com o suporte.

![01-versao-minima-sobre-a-versao-A.png](https://ajuda.sankhya.com.br/hc/article_attachments/42562370907159)

[![02-versao-minima-sobre-a-versao-B.png](https://ajuda.sankhya.com.br/hc/article_attachments/42562399015959)↑ Voltar ao início](#sumario)

## Os níveis de detalhamento

Pense no nível como um piso: aparece tudo do nível escolhido para cima (mais grave), e desaparece tudo abaixo dele.

Do mais detalhado para o mais grave: **TRACE** → **DEBUG** → **INFO** → **WARN** → **ERROR** → **FATAL**.

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Nível</strong></td><td style="border-color: #999; padding: 6px;"><strong>O que significa</strong></td><td style="border-color: #999; padding: 6px;"><strong>Quando usar</strong></td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>TRACE</strong></td><td style="border-color: #999; padding: 6px;">Rastreamento minucioso, passo a passo</td><td style="border-color: #999; padding: 6px;">Só a pedido do suporte, por poucos minutos</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>DEBUG</strong></td><td style="border-color: #999; padding: 6px;">Detalhes de diagnóstico</td><td style="border-color: #999; padding: 6px;">Investigação de um problema específico</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>INFO</strong> (padrão)</td><td style="border-color: #999; padding: 6px;">Eventos importantes do funcionamento normal</td><td style="border-color: #999; padding: 6px;">Operação do dia a dia</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>WARN</strong></td><td style="border-color: #999; padding: 6px;">Situação inesperada, mas o sistema continua funcionando</td><td style="border-color: #999; padding: 6px;">Ambiente que quer log mais enxuto</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>ERROR</strong></td><td style="border-color: #999; padding: 6px;">Uma operação falhou</td><td style="border-color: #999; padding: 6px;">Raro — esconde avisos úteis</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>FATAL</strong></td><td style="border-color: #999; padding: 6px;">Erro crítico, com paralisação</td><td style="border-color: #999; padding: 6px;">Não recomendado</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>OFF</strong></td><td style="border-color: #999; padding: 6px;">Desliga o log</td><td style="border-color: #999; padding: 6px;">Não recomendado</td></tr></tbody></table>

### O que aparece em cada configuração

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Nível configurado</strong></td><td style="border-color: #999; padding: 6px;"><strong>Aparece no log</strong></td><td style="border-color: #999; padding: 6px;"><strong>Não aparece</strong></td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>TRACE</strong></td><td style="border-color: #999; padding: 6px;">tudo (TRACE, DEBUG, INFO, WARN, ERROR, FATAL)</td><td style="border-color: #999; padding: 6px;">—</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>DEBUG</strong></td><td style="border-color: #999; padding: 6px;">DEBUG, INFO, WARN, ERROR, FATAL</td><td style="border-color: #999; padding: 6px;">TRACE</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>INFO</strong> (padrão)</td><td style="border-color: #999; padding: 6px;">INFO, WARN, ERROR, FATAL</td><td style="border-color: #999; padding: 6px;">TRACE, DEBUG</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>WARN</strong></td><td style="border-color: #999; padding: 6px;">WARN, ERROR, FATAL</td><td style="border-color: #999; padding: 6px;">TRACE, DEBUG, INFO</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>ERROR</strong></td><td style="border-color: #999; padding: 6px;">ERROR, FATAL</td><td style="border-color: #999; padding: 6px;">TRACE, DEBUG, INFO, WARN</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>FATAL</strong></td><td style="border-color: #999; padding: 6px;">só FATAL</td><td style="border-color: #999; padding: 6px;">todo o resto</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>OFF</strong></td><td style="border-color: #999; padding: 6px;">nada</td><td style="border-color: #999; padding: 6px;">tudo</td></tr></tbody></table>

Sem nenhuma configuração, o Sankhya Om opera em **INFO**. Erros e avisos sempre são registrados nesse modo — ligar **DEBUG** não é necessário para que uma falha apareça no log, apenas para ver mais detalhes sobre como ela aconteceu.

[↑ Voltar ao início](#sumario)

## Como alterar o parâmetro SANKHYALOGLEVEL

O parâmetro fica no cadastro de parâmetros do Sankhya Om, junto com os demais parâmetros do sistema. Para conhecer a árvore de parâmetros completa e os recursos de pesquisa dessa tela, acesse a tela **Preferências**.

1.  Acesse a tela **Preferências** e abra a seção **Parâmetros do Sistema** (ela fica dentro dessa tela, não é uma tela separada).
2.  Localize o parâmetro `SANKHYALOGLEVEL`.
3.  Informe o nível desejado no valor do parâmetro — por exemplo, **DEBUG**.
4.  Salve.

Pronto. A alteração é aplicada na hora, em todas as instâncias do ambiente. Não é necessário reiniciar o servidor, encerrar sessões ou pedir que os usuários saiam do Sankhya Om.

![03-como-alterar-parametro-preferencias.png](https://ajuda.sankhya.com.br/hc/article_attachments/42562370907927)

### Modo global (recomendado)

Na maior parte dos casos, basta informar um único nível, que passa a valer para o Sankhya Om inteiro. Por exemplo: **DEBUG**.

Outros valores válidos no modo global:

*   **TRACE**
*   **DEBUG**
*   **INFO**
*   **WARN**
*   **ERROR**
*   **FATAL**
*   **OFF**

Para voltar ao comportamento padrão, informe **INFO** (ou limpe o valor do parâmetro).

**ℹ️ Nota**

O Sankhya Om também aceita os nomes antigos usados internamente (**FINE**, **WARNING**, **SEVERE**, **ALL**) e não diferencia maiúsculas de minúsculas. Se o valor informado for inválido, o parâmetro volta automaticamente para **INFO** e um aviso é registrado no log.

### Modo direcionado (quando o suporte pedir)

Em investigações mais delicadas — ambientes de grande volume, onde ligar **DEBUG** no modo global geraria log demais — o suporte pode fornecer um valor direcionado, que aumenta o detalhamento apenas de uma parte do Sankhya Om. Esse modo é mais avançado que o global: permite combinar várias configurações, com níveis e grupos (pacotes) diferentes ao mesmo tempo.

Nesse caso o valor tem outro formato, com entradas separadas por ponto e vírgula:

`INFO;com.sankhya.util=DEBUG`

Leitura desse exemplo: o Sankhya Om inteiro em **INFO**, exceto uma área específica, que fica em **DEBUG**.

**💡 Dica**

Não é necessário montar esse valor por conta própria. Quando o modo direcionado for adequado, o suporte envia o texto exato para colar no parâmetro. Basta copiar, salvar e, ao final da investigação, restaurar **INFO**.

[↑ Voltar ao início](#sumario)

## Roteiro recomendado de investigação

1.  Antes de mexer, anote o valor atual do parâmetro, para poder restaurá-lo.
2.  Altere `SANKHYALOGLEVEL` para o valor indicado pelo suporte, normalmente **DEBUG**.
3.  Reproduza o problema — repita a operação que apresenta a falha.
4.  Colete o arquivo de log do servidor referente a esse período e envie ao suporte.
5.  Volte o parâmetro para **INFO**. Este passo é importante.

O ciclo inteiro leva poucos minutos e não causa indisponibilidade.

[↑ Voltar ao início](#sumario)

## Cuidados

*   Não deixe **DEBUG** ou **TRACE** ligados permanentemente. O volume de log cresce muito, consome espaço em disco e pode afetar o desempenho do ambiente. Ligue durante a investigação e desligue em seguida.
*   **TRACE** é o nível mais agressivo. Use apenas por poucos minutos e somente quando o suporte solicitar explicitamente.
*   Evite **WARN**, **ERROR**, **FATAL** e **OFF** como configuração fixa. Eles escondem informações que ajudam o suporte a diagnosticar problemas futuros — inclusive avisos que antecedem falhas.
*   Log não é auditoria. O nível de log não altera nada nos registros de auditoria, histórico ou rastreabilidade de documentos do Sankhya Om.

[↑ Voltar ao início](#sumario)

## Se o log continuou sem detalhes

Alterou o parâmetro para **DEBUG** e nada mudou no arquivo de log? O nível de detalhamento tem dois controles independentes: o do Sankhya Om (este parâmetro) e o do servidor de aplicação, que grava o arquivo.

Se o servidor de aplicação estiver configurado para gravar somente mensagens de **INFO** para cima, as mensagens de **DEBUG** são descartadas na gravação — mesmo com o parâmetro corretamente ajustado.

Nesse caso, acione a equipe de infraestrutura ou o suporte Sankhya: o ajuste é na configuração de log do servidor de aplicação, feito uma única vez por ambiente.

[↑ Voltar ao início](#sumario)

## Perguntas frequentes

### Preciso reiniciar o Sankhya Om depois de alterar o parâmetro?

Não. A alteração é aplicada imediatamente e se propaga para todas as instâncias do ambiente automaticamente.

### Os usuários precisam sair do Sankhya Om?

Não. Não há impacto nas sessões em uso.

### Alterar o nível de log muda o comportamento do Sankhya Om?

Não. Muda apenas a quantidade de informação registrada no log. Nenhuma regra de negócio, cálculo ou processo é afetado.

### Ligar DEBUG deixa o Sankhya Om mais lento?

Em uso pontual, o impacto é pequeno. Mantido por longos períodos, o volume de log pode consumir disco e degradar o desempenho — por isso a recomendação de voltar para **INFO** após a coleta.

### Erros só aparecem no log se eu ligar DEBUG?

Não. Erros e avisos são registrados sempre, já no nível padrão **INFO**. O **DEBUG** adiciona detalhes sobre o caminho que levou ao erro.

### Onde encontro o arquivo de log?

Abra o menu do seu usuário (foto no canto superior direito) e clique em **Administração**. Na tela **Administração do Servidor**, use o botão **Download do Log**. Esse acesso é exclusivo de administradores — normalmente são eles quem também alteram o parâmetro de sistema. Se não tiver esse acesso, solicite ao suporte ou à equipe de infraestrutura responsável pelo seu servidor.

![04-faq-log-administracao-A.png](https://ajuda.sankhya.com.br/hc/article_attachments/42562399016471)

![05-faq-log-administracao-B.png](https://ajuda.sankhya.com.br/hc/article_attachments/42562399017111)