# Consultar a Média Diária dos Impostos ICMS/ST

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/7053152322839-Consultar-a-M%C3%A9dia-Di%C3%A1ria-dos-Impostos-ICMS-ST](https://ajuda.sankhya.com.br/hc/pt-br/articles/7053152322839-Consultar-a-M%C3%A9dia-Di%C3%A1ria-dos-Impostos-ICMS-ST)

---

# Consultar a Média Diária dos Impostos ICMS/ST

 **![Módulo 36x36 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313149805719) Módulo:** Livros Fiscais > Relatórios       ![Versão - 32x32 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313149806359) **Versão disponível:** a partir da 4.13 

---

Essa tela tem o objetivo de exibir o cálculo das médias diárias dos impostos ICMS, ST e FCP do ST para que sejam utilizados na geração do sped fiscal, compondo os valores dos registros C181, C185, C186, H010 e H030.

![consultar.png](https://ajuda.sankhya.com.br/hc/article_attachments/7053513189143)

Na lateral da tela, no painel de filtros, obrigatoriamente você deve informar a **"Empresa"** e a **"Referência"** que deseja consultar.

Informe também o **"Produto"** pois, se não for informado, será apresentada a mensagem abaixo:

**_"Não foi informado nenhum produto no filtro rápido ou personalizado. Favor informar um produto e realizar a consulta novamente"._**

**Observação:** se você configurar nos filtros personalizados a busca por mais de um produto, o sistema trará as informações desses produtos independente do que foi informado no campo Produto, ou seja, os filtros personalizados são soberanos aos filtros padrões da tela.

No campo **"Tipo Imposto"** você define quais impostos serão exibidos na consulta, sendo eles:

*   ICMS;
*   ST;
*   BASE ST;
*   FCP.

Por fim, selecione qual **"Tipo Média"** você quer consultar, se **"Diária"** ou **"Inventário"**.

Após aplicar os filtros, na grade central serão apresentados os resultados encontrados:

![consultar2.png](https://ajuda.sankhya.com.br/hc/article_attachments/7057705114519)

Na grade acima podemos destacar os seguintes campos:

**Qtd. Inicial do Estoque:** exibe o valor do estoque do dia anterior;

**Total das entradas:** soma de todas as entradas de estoque do produto no dia;

**Total das saídas:** soma de todas as saídas de estoque do produto no dia; 

**Vlr. Unit. do Item:** tem como finalidade apresentar o valor unitário do imposto. O valor exibido aqui seguirá a fórmula abaixo:

![Calculadora.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313126639127) _Vlr. Unit. do Item= Vlr. Total do Imposto / Qtd. Inicial do Estoque + Total_ _das entradas_

**Vlr. Total do Imposto:** corresponde a soma dos impostos da(s) nota(s) de entrada incluindo os impostos do dia anterior, isto é:

 **![Calculadora.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313126639127)**_Vlr. Total do Imposto= Vlr. Final do Imposto do dia anterior  + Vlr. total do Imposto  
     no dia_

**Qtd. Final do Estoque:** tem como finalidade trazer o saldo de estoque do final do dia:

 _![Calculadora.FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42313126639127) Qtd. Final do Estoque = Qtd. Inicial do Estoque + Total das Entradas - Saídas do dia_

**Vlr. Final do Imposto:** será calculado da seguinte maneira:

*   Caso a Qtd Final do Estoque seja igual ao campo Qtd. Inicial do Estoque mais o Total da entradas será utilizada a fórmula:

<table style="border-collapse: collapse; width: 96.0001%; margin-right: 0px; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42313126639127" alt="Calculadora.FINAL.png"> <em>Vlr. Final do Imposto = Vlr. Total do Imposto</em></pre></td></tr></tbody></table>

*   Se a Qtd Final do Estoque for diferente do valor Qtd. Inicial do Estoque mais o Total da entradas será utilizada a fórmula:

<table style="border-collapse: collapse; width: 95.7143%; margin-right: 0px; margin-left: auto;"><tbody><tr><td style="width: 100%;"><pre><img src="https://ajuda.sankhya.com.br/hc/article_attachments/42313126639127" alt="Calculadora.FINAL.png"> <em>Vlr. Final do Imposto = Qtd. Final do Estoque x Vlr. Unit. do Item&nbsp;</em></pre></td></tr></tbody></table>

---

![essencial FINAL (1).png](https://ajuda.sankhya.com.br/hc/article_attachments/16286750198423) Caso não seja localizado nenhum resultado, a mensagem abaixo é exibida:

_**"Não foi encontrada nenhuma média diária de Imposto para o Produto/Referência/Empresa informado.".**_

---

Através do botão ![botao-exportar-grade-para-pdf-FINAL.jpg](/guide-media/01H6743AM7C5181E5VX745E5ZA) **"Exportar grade para PDF"** você consegue **"Exportar para PDF"**, **"Exportar para planilha (xls)"**, **"Exportar para planilha (xlsx)"** e **"Exportar para cubo"** as informações.

Aqui você poderá também configurar a grade dos campos no botão ![Configurar FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16286798287511) **"Configurar grade"**.

[\[Voltar ao topo\]](#top)