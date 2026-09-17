# Processo Ativação do JasperViewer em Navegadores de Mercado

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/42697513128727-Processo-Ativa%C3%A7%C3%A3o-do-JasperViewer-em-Navegadores-de-Mercado](https://ajuda.sankhya.com.br/hc/pt-br/articles/42697513128727-Processo-Ativa%C3%A7%C3%A3o-do-JasperViewer-em-Navegadores-de-Mercado)

---

# Processo Ativação do JasperViewer em Navegadores de Mercado

**Módulo:** Configurações › Avançado

**Caminho de acesso:** Menu Principal › Configurações › Avançado › Preferências (Forma 1) ou Menu Principal › Configurações › Avançado › Relatórios Formatados / Modelos de Etiquetas (Forma 2)

---

**Neste artigo**

*   [O que é e para que serve](#oque)
*   [Antes de começar](#antes)
*   [Forma 1 — Ativar para todos os relatórios](#forma1)
*   [Forma 2 — Ativar por relatório específico](#forma2)
*   [Pontos de atenção](#pontos)

## O que é e para que serve

O **Processo Ativação do JasperViewer em Navegadores de Mercado** controla como o Sankhya Om exibe relatórios em PDF quando a impressão é feita pelo Chrome, Edge, Firefox ou outro navegador de mercado. Por padrão, o Sankhya Om abre o diálogo de impressão nativo do navegador, que pode descartar cores de fundo e imagens dependendo das opções escolhidas ali. Ao ativar o mecanismo, o Sankhya Om gera o relatório em formato `.jrprint` e abre o **WebConnection** para apresentá-lo diretamente no JasperViewer, preservando 100% da formatação original — cores, fontes e imagens — independentemente das configurações do navegador. Este processo **não** altera o conteúdo, os dados ou a geração do relatório: ele muda apenas a forma como o resultado é exibido a você, e vale para qualquer fluxo que utilize o serviço de visualização de relatórios do Sankhya Om. Esta funcionalidade depende de um aplicativo externo ao Sankhya Om — o **WebConnection** — e só está disponível para clientes que o têm instalado e devidamente configurado; sem ele, nenhuma das duas formas de ativação deste processo tem efeito.

---

## Antes de começar

Este processo depende de um aplicativo externo ao Sankhya Om, o **WebConnection**: sem ele instalado e configurado, nenhuma das duas formas de ativação a seguir funciona. Antes de ativar qualquer uma delas, garanta que:

*   O aplicativo **WebConnection** está instalado e em execução na máquina de onde você acessa o Sankhya Om
*   O parâmetro `global.porta.app.impressao` está configurado com a porta correta em **Configurações › Avançado › Preferências**

**⚠️ Atenção**

Sempre confirme que o WebConnection está ativo e funcionando antes de ativar o mecanismo e seguir com a impressão. Se o WebConnection não estiver instalado, configurado ou em execução no momento da impressão, você verá uma mensagem de erro e o relatório não abrirá no JasperViewer, independentemente da forma de ativação escolhida.

[↑ Voltar ao início](#sumario)

---

## Forma 1 — Ativar para todos os relatórios (Preferências do Sistema)

Esta forma ativa o mecanismo globalmente para **todos** os relatórios acessados por navegadores de mercado, em qualquer fluxo que utilize o serviço de visualização de relatórios do Sankhya Om.

1.  Acesse **Configurações › Avançado › Preferências**.
2.  Pesquise pela chave `MGEJASPERWEB`.
3.  Defina o valor como **Sim** para ativar o JasperViewer em todos os relatórios, ou mantenha **Não** para manter o diálogo de impressão nativo do navegador.

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Chave</strong></td><td style="border-color: #999; padding: 6px;"><code>MGEJASPERWEB</code></td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Nome</strong></td><td style="border-color: #999; padding: 6px;"><code>mge.report.utilizar.jasper.viewer.web</code></td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Tipo</strong></td><td style="border-color: #999; padding: 6px;">Lógico</td></tr><tr><td style="border-color: #999; padding: 6px;"><strong>Padrão</strong></td><td style="border-color: #999; padding: 6px;"><strong>Não</strong> (desativado)</td></tr></tbody></table>

**ℹ️ Nota**

O parâmetro equivalente para o Navegador Sankhya (Electron) é o `UTZJASPERWC`. Os dois parâmetros são independentes: ativar um não ativa o outro.

[↑ Voltar ao início](#sumario)

---

## Forma 2 — Ativar por relatório específico (property no JRXML)

Esta forma ativa o mecanismo apenas para um relatório específico, sem alterar o comportamento dos demais. Use quando somente determinados relatórios — como etiquetas — precisam de fidelidade total de impressão.

**⚠️ Atenção**

A property `useJasperViewerWeb` só tem efeito quando o parâmetro `MGEJASPERWEB` está desativado (**Não**). Com o parâmetro ativado, a configuração global prevalece sobre a property do relatório.

1.  Acesse a tela de manutenção do relatório: **Configurações › Avançado › Relatórios Formatados** ou **Modelos de Etiquetas**.
2.  Localize o registro pelo código. Se necessário, consulte a tabela `TSIRFE`.
3.  Baixe o arquivo `.jrxml` associado ao registro.
4.  Adicione a linha abaixo dentro do elemento `<jasperReport>`, junto às demais `<property>` existentes:
    
    ```xml
    <jasperReport ...>
        <property name="useJasperViewerWeb" value="true"/>
        <!-- demais properties e conteúdo do relatório -->
    ```
    
5.  Salve o arquivo e reenvie-o pelo mesmo campo na tela de manutenção.

Depois de reenviar o arquivo, a primeira impressão desse relatório pode ficar mais lenta enquanto o Sankhya Om recompila e armazena o relatório em cache — as impressões seguintes seguem no ritmo normal.

[↑ Voltar ao início](#sumario)

---

## Pontos de atenção

Quando as duas formas de ativação estão configuradas ao mesmo tempo, o parâmetro global prevalece sobre a property do relatório. Use a tabela abaixo para identificar qual configuração está ativa em cada cenário.

<table style="border-collapse: collapse;"><tbody><tr><td style="border-color: #999; padding: 6px;"><strong>Configuração</strong></td><td style="border-color: #999; padding: 6px;"><strong>Escopo</strong></td><td style="border-color: #999; padding: 6px;"><strong>Comportamento</strong></td></tr><tr><td style="border-color: #999; padding: 6px;"><code>MGEJASPERWEB</code> = <strong>Sim</strong></td><td style="border-color: #999; padding: 6px;">Todos os relatórios</td><td style="border-color: #999; padding: 6px;">JasperViewer ativo para qualquer relatório em PDF.</td></tr><tr><td style="border-color: #999; padding: 6px;"><code>useJasperViewerWeb = true</code> (JRXML)</td><td style="border-color: #999; padding: 6px;">Relatório específico</td><td style="border-color: #999; padding: 6px;">JasperViewer ativo apenas para esse relatório; só entra em vigor quando <code>MGEJASPERWEB</code> = <strong>Não</strong>.</td></tr><tr><td style="border-color: #999; padding: 6px;">Nenhuma das duas</td><td style="border-color: #999; padding: 6px;">—</td><td style="border-color: #999; padding: 6px;">Fluxo padrão do navegador (PDF nativo).</td></tr></tbody></table>

O mecanismo se aplica apenas a navegadores de mercado (Chrome, Edge, Firefox etc.). Para o Navegador Sankhya (Electron), a ativação equivalente é feita pelo parâmetro `UTZJASPERWC`, de forma independente das duas formas descritas neste artigo.