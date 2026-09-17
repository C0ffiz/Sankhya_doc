# Nota Técnica 2015.004 - CT-e - Fundo de Combate a Pobreza

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360045111493-Nota-T%C3%A9cnica-2015-004-CT-e-Fundo-de-Combate-a-Pobreza](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045111493-Nota-T%C3%A9cnica-2015-004-CT-e-Fundo-de-Combate-a-Pobreza)

---

# Nota Técnica 2015.004 - CT-e - Fundo de Combate a Pobreza

A Nota Técnica 2015.004 apresenta novas tratativas a serem consideradas para o CT-e. Dentre elas, há modificação no layout da NF-e para que este receba as informações da cobrança de ICMS nas operações interestaduais de vendas a consumidor final não contribuinte do imposto, de forma que, insira ainda novos campos para cálculo do Fundo de Combate à Pobreza UF Destino.  

Para se adequar às modificações, há no sistema novos campos que buscarão essas informações para enviá-las para as tag's do XML, pois são elas que serão validadas para que o CT-e seja aprovado.

Observe abaixo, os campos que receberão os valores do Fundo de Combate à Pobreza: 

<table style="border-collapse: collapse; width: 100%; height: 44px;"><tbody><tr style="height: 44px;"><td style="width: 4.00001%;">&nbsp;</td><td style="width: 6.14286%; height: 44px;"><img alt="Marcador 1 FINAL.png" src="/hc/article_attachments/28458109863063"></td><td class="wysiwyg-text-align-justify" style="width: 89.8571%; height: 44px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><strong>TGFICM.PERCICMSFCP:</strong> tela <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360044602934-Al%C3%ADquotas-de-ICMS" rel="noopener noreferrer" target="_blank">Alíquotas de ICMS</a>, aba <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360044602934-Al%C3%ADquotas-de-ICMS#abageral" rel="noopener noreferrer" target="_blank">Geral</a>, campo <strong>"Perc. ICMS Fundo Comb. Pobreza"</strong>;</span></td></tr></tbody></table>

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td style="width: 4.00001%;">&nbsp;</td><td style="width: 6%;"><img alt="Marcador 1 FINAL.png" src="/hc/article_attachments/28458109863063"></td><td class="wysiwyg-text-align-justify" style="width: 90%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><strong>TGFDIN.PERCFCP:</strong> tela <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612414-Central-de-Vendas" rel="noopener noreferrer" target="_blank">Central de Vendas</a>, botão <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360044612234" rel="noopener noreferrer" target="_blank">Outras Opções...</a>, opção <strong>"Perc. para Fundo Comb. Pobreza"</strong>;</span></td></tr></tbody></table>

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td style="width: 4.04759%;">&nbsp;</td><td style="width: 6.04757%;"><img alt="Marcador 1 FINAL.png" src="/hc/article_attachments/28458109863063"></td><td class="wysiwyg-text-align-justify" style="width: 89.9047%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">TGFDIN.VLRFCP: tela <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360045106793-Central-de-Compras" rel="noopener noreferrer" target="_blank">Central de Compras</a>, botão <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360044593994-Central-de-Compras-Bot%C3%A3o-Outras-Op%C3%A7%C3%B5es" rel="noopener noreferrer" target="_blank">Outras Opções...</a>, opção <strong>"Perc. para Fundo Comb. Pobreza"</strong>.</span></td></tr></tbody></table>

## Validações na confirmação do CT-e

<table style="border-collapse: collapse; width: 100%; height: 44px;"><tbody><tr style="height: 12px;"><td style="width: 3.28572%; height: 12px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;</span></td><td style="width: 5.71429%; height: 12px;"><img alt="Marcador 1 FINAL.png" src="/hc/article_attachments/28458109863063"></td><td rowspan="3" style="width: 90.9999%; height: 44px;"><p class="wysiwyg-text-align-justify"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Caso CT-e a ser confirmado possua documentos anteriores cadastrados (TGFDANT) e o campo <strong>"Tipo de Serviço CT-e"</strong> (aba <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abactemde" rel="noopener noreferrer" target="_blank">CT-e/MD-e</a>) seja definido com a opção <strong>"Normal"</strong> (TGFTOP.TIPSERVCTE = 0), a seguinte mensagem será exibida:</span></p><p class="wysiwyg-text-align-justify"><span style="font-family: Verdana,Geneva,Arial,sans-serif;"><em><strong>"Não devem ser informados documentos anteriores para CT-e com o tipo de serviço normal."</strong></em></span></p></td></tr><tr style="height: 10px;"><td style="width: 3.28572%; height: 10px;">&nbsp;</td><td style="width: 5.71429%; height: 10px;">&nbsp;</td></tr><tr style="height: 22px;"><td style="width: 3.28572%; height: 22px;">&nbsp;</td><td style="width: 5.71429%; height: 22px;">&nbsp;</td></tr></tbody></table>

<table style="border-collapse: collapse; width: 100%; height: 100px;"><tbody><tr style="height: 34px;"><td style="width: 3.3333%; height: 34px;">&nbsp;</td><td style="width: 5.61901%; height: 34px;"><img alt="Marcador 1 FINAL.png" src="/hc/article_attachments/28458109863063"></td><td rowspan="4" style="width: 91.0476%; height: 100px;"><p class="wysiwyg-text-align-justify"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">Se o CT-e a ser confirmado possuir dois serviços ou mais, e houver cálculo de DIFAL ou de Pobreza, os percentuais devem ser os mesmos (TGFDIN.ALIQINTDEST e TGFDIN.PERCFCP), caso contrário, a seguinte mensagem será exibida:</span></p><p class="wysiwyg-text-align-justify"><em><strong>"Verifique a tributação dos componentes do serviço (serviços) o CT-e! Para confirmação do CT-e é necessário que a tributação (CST), a alíquota de ICMS, percentual de redução de base, CFOP, alíquota interna de destino e fundo de combate à pobreza sejam os mesmos."</strong></em></p></td></tr><tr style="height: 22px;"><td style="width: 3.3333%; height: 22px;">&nbsp;</td><td style="width: 5.61901%; height: 22px;">&nbsp;</td></tr><tr style="height: 22px;"><td style="width: 3.3333%; height: 22px;">&nbsp;</td><td style="width: 5.61901%; height: 22px;">&nbsp;</td></tr><tr style="height: 22px;"><td style="width: 3.3333%; height: 22px;">&nbsp;</td><td style="width: 5.61901%; height: 22px;">&nbsp;</td></tr></tbody></table>

## Cálculo do ICMS para o Fundo de Combate à Pobreza

As regras para o cálculo do Fundo de Combate à Pobreza, seguem as mesmas condições para o cálculo do DIFAL. Observe:

<table style="border-collapse: collapse; width: 100%;"><tbody><tr><td style="width: 3.57143%;">&nbsp;</td><td style="width: 5.14289%;"><img alt="Marcador 1 FINAL.png" src="/hc/article_attachments/28458109863063"></td><td class="wysiwyg-text-align-justify" style="width: 91.2857%;">O <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP" rel="noopener noreferrer" target="_blank">Tipo de Operação - TOP</a> utilizado deve possuir o <strong>"Tipo de Movimento"</strong> como <strong>"V-Venda"</strong> ou <strong>"P-Pedido de venda"</strong>;</td></tr></tbody></table>

<table style="border-collapse: collapse; width: 100%; height: 44px;"><tbody><tr style="height: 44px;"><td style="width: 3.61901%; height: 44px;">&nbsp;</td><td style="width: 5.19046%; height: 44px;"><img alt="Marcador 1 FINAL.png" src="/hc/article_attachments/28458109863063"></td><td class="wysiwyg-text-align-justify" style="width: 91.1904%; height: 44px;">Na mesma tela, aba <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abaimpostos" rel="noopener noreferrer" target="_blank">Impostos</a>, a marcação <strong>"<span style="font-family: Verdana,Geneva,Arial,sans-serif;">Calcular DIFAL Partilhado</span>"</strong> (<span style="font-family: Verdana,Geneva,Arial,sans-serif;">TGFTOP.CALCDIFALPART</span>) deve ser habilitada;</td></tr></tbody></table>

<table style="border-collapse: collapse; width: 100%; height: 44px;"><tbody><tr style="height: 44px;"><td style="width: 3.47616%; height: 44px;">&nbsp;</td><td style="width: 5.47611%; height: 44px;"><img alt="Marcador 1 FINAL.png" src="/hc/article_attachments/28458109863063"></td><td class="wysiwyg-text-align-justify" style="width: 91.0476%; height: 44px;">Além disso, na aba <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abaimpresso" rel="noopener noreferrer" target="_blank">Impressão</a> o campo <strong>"Tipo de serviço CT-e"</strong> tem de ser definido com a opção <strong>"Normal"</strong>;</td></tr></tbody></table>

<table style="border-collapse: collapse; width: 100%; height: 34px;"><tbody><tr style="height: 34px;"><td style="width: 3.47616%; height: 34px;">&nbsp;</td><td style="width: 5.61897%; height: 34px;"><img alt="Marcador 1 FINAL.png" src="/hc/article_attachments/28458109863063"></td><td class="wysiwyg-text-align-justify" style="width: 90.9047%; height: 34px;">O parceiro destinatário, sendo este cadastrado na tela <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros" rel="noopener noreferrer" target="_blank">Parceiros</a>, precisar ser configurado com a opção <strong>"Consumidor Final"</strong> do campo <strong>"Classificação ICMS"</strong>, sendo este localizado na aba <a href="https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros#abafiscal" rel="noopener noreferrer" target="_blank">Fiscal</a>.</td></tr></tbody></table>

Dessa forma, o cálculo será realizado por item da seguinte forma:

        ![Calculadora.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42310973367319) **TGFDIN.VLRFCP = TGFDIN.BASE \* Perc. ICMS para Fundo Comb. Pobreza   
                                 (TGFICMS.PERCFCP)**

<table style="border-collapse: collapse; height: 55px; width: 100%;"><tbody><tr style="height: 11px;"><td rowspan="3" style="width: 4.42861%; height: 11px;"><img alt="roxo_2.png" height="110" src="/hc/article_attachments/42310952937111" width="15"></td><td class="wysiwyg-text-align-justify" rowspan="3" style="width: 93.7142%; height: 55px;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">No caso de a Alíquota de ICMS ser igual a Alíquota Interna de Destino, não haverá cálculo para o DIFAL, no entanto, caso seja informado o Perc. ICMS Fundo Comb. Pobreza, será calculado o valor do ICMS para o Fundo de Combate a Pobreza, e todas as tag's pertencentes ao Grupo das vendas interestaduais para Consumidor Final não contribuinte do ICMS, serão geradas.</span></td><td rowspan="3" style="width: 1.85712%;"><span style="font-family: Verdana,Geneva,Arial,sans-serif;">&nbsp;</span></td></tr></tbody></table>

No exemplo abaixo, você poderá observar alguns XML's de notas aprovadas:

 ![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28458109863063) Com DIFAL e com Fundo de Combate à Pobreza:

<imp>  
        <ICMS>  
                <ICMS00>  
                        <CST>**00**</CST>  
                        <vBC>**535.00**</vBC>  
                        <pICMS>**12.00**</pICMS>  
                        <vICMS>**64.20**</vICMS>  
                </ICMS00>  
        </ICMS>  
        <ICMSUFFim>  
                <vBCUFFim>**535.00**</vBCUFFim>  
                <pFCPUFFim>**2.00**</pFCPUFFim>  
                <pICMSUFFim>**23.00**</pICMSUFFim>  
                <pICMSInter>**12.00**</pICMSInter>  
                <pICMSInterPart>**40.00**</pICMSInterPart>  
                <vFCPUFFim>**10.70**</vFCPUFFim>  
                <vICMSUFFim>**23.54**</vICMSUFFim>  
                <vICMSUFIni>**35.31**</vICMSUFIni>  
        </imp>

 ![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28458109863063) Com DIFAL e sem Fundo de Combate à Pobreza:

<imp>  
        <ICMS>  
                <ICMS00>  
                        <CST>**00**</CST>  
                        <vBC>**521.81**</vBC>  
                        <pICMS>**12.00**</pICMS>  
                        <vICMS>**62.62**</vICMS>  
               </ICMS00>  
        </ICMS>  
        <ICMSUFFim>  
                <vBCUFFim>**521.81**</vBCUFFim>  
                <pFCPUFFim>**0.00**</pFCPUFFim>  
                <pICMSUFFim>**23.00**</pICMSUFFim>  
                <pICMSInter>**12.00**</pICMSInter>  
                <pICMSInterPart>**40.00**</pICMSInterPart>  
                <vFCPUFFim>**0.00**</vFCPUFFim>  
                <vICMSUFFim>**22.96**</vICMSUFFim>  
                <vICMSUFIni>**34.44**</vICMSUFIni>  
         </ICMSUFFim>  
  </imp>

 ![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28458109863063) Sem DIFAL e com Fundo de Combate à Pobreza:

<imp>  
        <ICMS>     
                  <ICMS00>  
                          <CST>**00**</CST>    
                          <vBC>**739.25**</vBC>  
                          <pICMS>**12.00**</pICMS>  
                          <vCIMS>**88.71**</vCIMS>  
                   </ICMS00>  
           </ICMS>  
           <ICMSUFFim>  
                   <vBCUFFim>**739.25**</vBCUFFim>  
                   <pFCPUFFim>**2.00**</pFCPUFFim>  
                   <pICMSUFFim>**0.00**</pICMSUFFim>  
                   <pICMSInter>**12.00**</pICMSInter>  
                   <pICMSInterPart>**40.00**</pICMSInterPart>  
                   <vFCPUFFim>**14.78**</vFCPUFFim>  
                   <vICMSUFFim>**0.00**</vICMSUFFim>  
                   <vICMSUFIni>**0.00**</vICMSUFIni>  
            </ICMSUFFim>  
</imp>

 ![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28458109863063) Sem DIFAL e sem Fundo de Combate à Pobreza:

      <imp>  
              <ICMS>  
                      <ICMS00>  
                              <CST>**00**</CST>  
                              <vBC>**416.32**</vBC>  
                              <pICMS>**12.00**</pICMS>  
                              <vICMS>**49.96**</ICMS>  
                       </ICMS00>  
               </ICMS>  
      </imp>

[\[Voltar ao topo\]](#top)