# Envio da Folha de Pagamento para o eSocial

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/21012474338967-Envio-da-Folha-de-Pagamento-para-o-eSocial](https://ajuda.sankhya.com.br/hc/pt-br/articles/21012474338967-Envio-da-Folha-de-Pagamento-para-o-eSocial)

---

# Envio da Folha de Pagamento para o eSocial

**Módulo:** Pessoal+  
**Caminho de Acesso:** Pessoal+ > Rotinas Folha > Gerenciador de Folhas

                                      Pessoal+ > Rotinas Folha > Central do eSocial  
**ID da Tela:** br.com.sankhya.rh.GerenciadorFolha

                    br.com.sankhya.CentraleSocial

---

### **Descrição e Usabilidade**

Após realizar o cálculo e a conferência da folha de pagamento, é necessário efetuar a liberação das folhas para o eSocial e realizar a geração dos eventos na Central do eSocial.

Essa rotina é responsável por disponibilizar os dados das folhas para geração dos eventos periódicos do eSocial, como:

*   S-1200 – Remuneração do Trabalhador;
*   S-1210 – Pagamentos de Rendimentos do Trabalho;
*   S-2299 – Desligamento;
*   S-2399 – Trabalhador Sem Vínculo – Término.

A liberação é realizada por meio do botão **Liberação para eSocial**, disponível no **Gerenciador de Folhas**.

**⚠️** Após a liberação, ainda é necessário acessar a Central do eSocial para gerar e transmitir os eventos.

### **Pré-requisitos**

Antes de realizar o envio da folha para o eSocial, valide os seguintes pontos:

*   folha calculada e conferida;
*   eventos de rubricas enviados ao eSocial;
*   dados cadastrais da empresa atualizados;
*   folhas liberadas para envio;
*   usuário com acesso ao Gerenciador de Folhas e à Central do eSocial.

**⚠️** Qualquer alteração realizada após a liberação da folha exigirá nova liberação e nova geração dos eventos.

### **Jornada de Uso**

![liberarfolhapesocial.gif](https://ajuda.sankhya.com.br/hc/article_attachments/40495811672599)

1.  Acesse o Gerenciador de Folhas (Pessoal+ > Rotinas Folha);
    
2.  Localize a folha desejada utilizando o painel de filtros;
    
3.  Clique no botão **Liberação para eSocial**;
    
4.  No pop-up, selecione:
    
    *   **Tipo de Folha**;
        
    *   **Referência**;
        
    *   **Tipo de ação = Liberar Dados**. 
        
5.  Escolha a **Empresa** e os **Funcionários** clicando em seus respectivos cards ou marcando **Todos**;
    
6.  Clique em **Liberar Dados para eSocial** e confirme. 
    
    Ao confirmar a operação, o sistema exibirá um resumo da liberação realizada.
    

<table style="background-color: #fcfce9; border-style: none;"><tbody><tr><td style="background-color: #fcfce9; border-style: none;"><p><strong>⚠️</strong></p><p data-start="2357" data-end="2433">Sempre realize a liberação de todos os tipos de folhas da competência, como:</p><ul data-start="2435" data-end="2513"><li data-section-id="9b30o7" data-start="2435" data-end="2450" data-list-item-id="efa48eef896d7a2db93252550982c9492">folha mensal;</li><li data-section-id="1urjyrc" data-start="2451" data-end="2466" data-list-item-id="e4ec2532a27746c160fc534112ad7a20a">adiantamento;</li><li data-section-id="opwi9h" data-start="2467" data-end="2476" data-list-item-id="eba810d4c50e23b90dabcf031bb4cf3cb">férias;</li><li data-section-id="j6u8g2" data-start="2477" data-end="2488" data-list-item-id="e1841cd9228e4e850b03a08dd34da9a9c">rescisão;</li><li data-section-id="e6m1sm" data-start="2489" data-end="2513" data-list-item-id="ea628d50b3d925a655bcf883103559bcd">folhas complementares.</li></ul><p>Atente-se:</p><ul><li data-list-item-id="e18f01fa3fecf90348d333c6617b9e57d"><p data-start="2588" data-end="2614">O evento S-1200 considera todas as folhas da competência atual.</p></li></ul><p class="wysiwyg-indent4" data-start="2657" data-end="2665">Exemplo: competência da folha: <strong data-start="2689" data-end="2700">05/2026</strong></p><p class="wysiwyg-indent10" data-start="2702" data-end="2770">Todas as folhas da competência 05/2026 serão consideradas no S-1200.</p><ul><li data-list-item-id="ea33080370bc9a8d11e15f6f57aae0a30"><p data-start="2802" data-end="2828">O evento S-1210 considera as folhas cujo pagamento ocorreu na competência atual.</p></li></ul><p class="wysiwyg-indent4" data-start="2885" data-end="2893">Exemplo: uma folha da competência 04/2026 paga em 05/2026 será enviada no S-1210 da competência 05/2026.</p><p data-start="2992" data-end="3130">Por isso, é importante conferir se folhas de competências anteriores com pagamento na competência atual também foram liberadas para envio.</p></td></tr></tbody></table>

7.  Após essa liberação é necessário fazer a [Geração](https://ajuda.sankhya.com.br/hc/pt-br/articles/7064222145175-Central-do-eSocial#gera%C3%A7%C3%A3o) e [Envio](https://ajuda.sankhya.com.br/hc/pt-br/articles/7064222145175-Central-do-eSocial#eventospendentes) dos eventos na [Central do eSocial](https://ajuda.sankhya.com.br/hc/pt-br/articles/7064222145175). 
    
    ![geraenvia-eventosfechado.png](https://ajuda.sankhya.com.br/hc/article_attachments/40495936178199)
    

A liberação e o envio devem respeitar a hierarquia do eSocial.

A sequência recomendada é:

1.  Rubricas (S-1010);
    
2.  Rescisões (S-2299) da competência ainda não enviada;
    
3.  Alterações cadastrais (S-2205);
    
4.  Alterações contratuais (S-2206);
    
5.  Afastamentos temporários (S-2230);
    
6.  Remuneração (S-1200);
    
7.  Pagamentos (S-1210);
    
8.  Trabalhadores avulsos (S-1270);
    
9.  Informações complementares (S-1280).
    

![acesse também FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/21040156874135) Para saber mais sobre prazos e hierarquia de envio de cada evento, consulte o [Manual de Orientação do eSocial](https://www.gov.br/esocial/pt-br/documentacao-tecnica/manuais/mos-s-1-3-consolidada-ate-a-no-s-1-3-07-2026.pdf).

8.  Após o envio e retorno com sucesso dos eventos periódicos, finalizar a competência por meio do menu [**Finalização**](https://ajuda.sankhya.com.br/hc/pt-br/articles/7064222145175-Central-do-eSocial#finaliza%C3%A7%C3%A3o) na Central do eSocial; 
    
    ![finfechamentofolhaesocial.png](https://ajuda.sankhya.com.br/hc/article_attachments/40496021890839)
    
9.  Volte ao [Gerenciador de Folhas](https://ajuda.sankhya.com.br/hc/pt-br/articles/40106318532247-Gerenciador-de-Folhas#h_01KQN6106PKSHZXJST6M9STWH7) e realize o fechamento da competência.
    
    ![fechamentogerenciadordefolha.png](https://ajuda.sankhya.com.br/hc/article_attachments/40496011767319)
    

Caso existam diferenças entre os valores do Pessoal+ e os retornados pelo eSocial, utilize o relatório [Relatório S-5001 - Conferência de Contribuições sociais INSS/PIS](https://ajuda.sankhya.com.br/hc/pt-br/articles/36419467638551) para analisar as diferenças relacionadas a:

*   INSS;
*   FGTS;
*   IRRF.

Segue abaixo as principais causas de diferenças de IRRF, INSS e FGTS:

<table style="border-collapse: collapse;"><tbody><tr><td style="background-color: #66cc66; text-align: center; width: 50%;"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;"><strong>&nbsp; CAUSA</strong></span></td><td style="background-color: #66cc66; text-align: center; width: 50%;"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;"><strong>&nbsp; SOLUÇÃO</strong></span></td></tr><tr><td class="wysiwyg-indent1" style="text-align: left; vertical-align: top; width: 50%;"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Folha de pagamento sem liberação para envio ao eSocial.</span></td><td class="wysiwyg-indent1" style="text-align: left; width: 50%;"><ul><li data-list-item-id="efa199cc58ba11980e10ec6a18f9db72b">Fazer a <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/40106318532247-Gerenciador-de-Folhas#h_01KQN3XPDJ4KAYEW7VWMBHPXCZ" target="_blank" rel="noopener noreferrer">liberação para envio das folhas</a> no Gerenciador de Folhas;</li><li data-list-item-id="e4909bcffa9904cf905c575616e497af7">Realizar uma nova geração e envio na Central do eSocial.&nbsp;<br>&nbsp;</li></ul></td></tr><tr><td class="wysiwyg-indent1" style="vertical-align: top; width: 50%;"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Alterações no cálculo após o envio para o eSocial.</span></td><td class="wysiwyg-indent1" style="width: 50%;"><ul><li data-list-item-id="e7989600ceb0e140f6457ce3198650e27"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Bloquear a liberação das folhas no Gerenciador de Folhas;</span></li><li data-list-item-id="e11295ab6d6a5cfc4e1a53cdc9b13fb64"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Realizar uma nova geração e envio na Central do eSocial.&nbsp;</span></li></ul></td></tr><tr><td class="wysiwyg-indent1" style="width: 50%;"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Dados cadastrais da empresa divergentes (FAP, terceiros, INSS).</span></td><td class="wysiwyg-indent1" style="width: 50%;"><ul><li data-list-item-id="e28d61879dfecb5679f90c0f6158640a9"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Revisar os cadastros da empresa no sistema.</span><br>&nbsp;</li></ul></td></tr><tr><td class="wysiwyg-indent1" style="vertical-align: top; width: 50%;"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Cadastro de rubricas com incidências enviadas ao eSocial diferente das incidências do cálculo no Pessoal+.</span><br>&nbsp;</td><td class="wysiwyg-indent2" style="width: 50%;"><ul><li data-list-item-id="eacdf1c49b8a67f2fdee0706998b27f95"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Revisar o cadastro das incidências das rubricas e fazer um novo envio do S-1010 ajustando as incidências no portal.&nbsp;</span></li><li data-list-item-id="e32417755e86525b7867a5cf10e52bbe2"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Excluir a folha já enviada seguindo o processo abaixo:</span><ul><li data-list-item-id="ec47d461b37662ec1f0e695c3ce8fadc5"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Fazer a reabertura da competência na Central do eSocial;</span></li><li data-list-item-id="eae743b4977655a93af6b549cf4c8dbcb"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Bloquear o envio ao eSocial da folha que tem a rubrica incorreta no Gerenciador de Folhas;</span></li><li data-list-item-id="e61f5795d7784415ecc081554b886a344"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Com a folha bloqueada, realizar a Geração na Central do eSocial (será gerado uma exclusão da folha de pagamento);</span></li><li data-list-item-id="ef50d92b1f181dc6a2810501c7007f5e4"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Enviar o evento e aguardar o retorno;</span></li><li data-list-item-id="e84764fe5d2688bddc91dcd7903b594d5"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Liberar novamente a folha de pagamento no Gerenciador de Folhas;</span></li><li data-list-item-id="e1b3bc3f9dd310d14f0df15f680d02d7a"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Gerar os eventos na Central do eSocial;</span></li><li data-list-item-id="e4be0d089e2d4bf6773243331f2b8d793"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Enviar o evento e aguardar o retorno;</span></li><li data-list-item-id="eb9fbbe80d3b0033f9a512b34d101746f"><span style="font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif; font-size: 15px;">Enviar o fechamento da competência.</span></li></ul></li></ul></td></tr></tbody></table>

## **Pontos de Atenção**

*   Alterações na folha após envio exigem retificação;
*   Folhas não liberadas não serão consideradas nos eventos periódicos;
*   O S-1210 considera a data de pagamento e não a competência da folha;
*   O envio deve respeitar a hierarquia dos eventos do eSocial;
*   Rubricas com incidências incorretas podem gerar diferenças tributárias.

## **Dicas de Usabilidade**

*   Sempre confira todas as folhas antes da liberação;
*   Libere férias, rescisões e complementares junto da folha mensal;
*   Utilize a Conferência Analítica de Tributos após o envio;
*   Evite alterar cálculos após a geração dos eventos;
*   Revise incidências de rubricas periodicamente.

### **Artigos Relacionados**

*   [Gerenciador de Folhas](https://ajuda.sankhya.com.br/hc/pt-br/articles/40106318532247)
*   [Central do eSocial](https://ajuda.sankhya.com.br/hc/pt-br/articles/7064222145175)