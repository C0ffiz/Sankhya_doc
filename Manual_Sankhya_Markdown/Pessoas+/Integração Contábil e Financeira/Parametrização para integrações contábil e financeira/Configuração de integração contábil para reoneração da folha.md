# Configuração de integração contábil para reoneração da folha

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/29805627986455-Configura%C3%A7%C3%A3o-de-integra%C3%A7%C3%A3o-cont%C3%A1bil-para-reonera%C3%A7%C3%A3o-da-folha](https://ajuda.sankhya.com.br/hc/pt-br/articles/29805627986455-Configura%C3%A7%C3%A3o-de-integra%C3%A7%C3%A3o-cont%C3%A1bil-para-reonera%C3%A7%C3%A3o-da-folha)

---

# Configuração de integração contábil para reoneração da folha

A reoneração da folha de pagamento mudou como algumas empresas calculam a contribuição ao INSS. Segundo a **Lei n.º 14.973/2024**, **empresas desoneradas não pagam a contribuição patronal sobre o 13º salário**, e a alíquota de 20% volta a ser aplicada gradualmente em municípios com baixo índice populacional.

Para garantir que o **Pessoal+** faça corretamente a integração contábil do **INSS parte empresa**, ao calcular o 13º salário (seja em rescisões ou na folha de pagamento), é **necessário** ajustar as [Fórmulas contábeis](https://ajuda.sankhya.com.br/hc/pt-br/articles/10086051863063) dos eventos usados nesse cálculo.

### **O que muda?**

A fórmula contábil não deve utilizar a variável "V\_perinss" (percentual INSS) para empresas desoneradas.

### **Como configurar?**

![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/29805961845655) **Fórmula para provisão do INSS 13º salário:**

*   antes;

**_(V\_totbas + V\_Incorpora)\* (V\_perinss + V\_pergrps + (V\_persegu \* V\_FAP) + V\_perRAT) / 100_  
**

![formula-utiliza-percentual-inss.png](https://ajuda.sankhya.com.br/hc/article_attachments/29806124932247)

*   agora.

**_(V\_totbas + V\_Incorpora)\* (V\_pergrps + (V\_persegu \* V\_FAP) + V\_perRAT) / 100_**

![nova-formula-perinss.png](https://ajuda.sankhya.com.br/hc/article_attachments/29806259852439)

---

 **![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/29805961845655) Fórmula para o INSS da folha normal do 13º salário:**

*   antes;

**_(V\_totbas )\* (V\_perinss + V\_pergrps + (V\_persegu \* V\_FAP) + V\_perRAT) / 100_**

![formula-perinss-folha-normal.png](https://ajuda.sankhya.com.br/hc/article_attachments/29806418211223)

*   agora.

**_(V\_totbas )\* (V\_pergrps + (V\_persegu \* V\_FAP) + V\_perRAT) / 100_**

![nova-formula-perinss-folha-normal.png](https://ajuda.sankhya.com.br/hc/article_attachments/29806518131479)

Essas fórmulas devem ser aplicadas **aos eventos de base de cálculo de 13º salário** utilizados na configuração contábil dos [Registros Fiscais](https://ajuda.sankhya.com.br/hc/pt-br/articles/360057060214) de empresas **optantes** pela desoneração da folha de pagamento.