# Como configurar eventos de horas extras para cálculo correto de médias em férias e 13° salário?

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/39387234449815-Como-configurar-eventos-de-horas-extras-para-c%C3%A1lculo-correto-de-m%C3%A9dias-em-f%C3%A9rias-e-13-sal%C3%A1rio](https://ajuda.sankhya.com.br/hc/pt-br/articles/39387234449815-Como-configurar-eventos-de-horas-extras-para-c%C3%A1lculo-correto-de-m%C3%A9dias-em-f%C3%A9rias-e-13-sal%C3%A1rio)

---

# Como configurar eventos de horas extras para cálculo correto de médias em férias e 13° salário?

Para que os eventos de “Horas Extras”, “Adicional Noturno”, “Horas Noturnas” ou quaisquer outros eventos que devam compor médias sejam calculados corretamente nas médias de férias e 13º salário, é fundamental validar a configuração desses eventos no sistema, principalmente o campo responsável por definir como eles incidem sobre as médias.

Caso o evento não esteja apresentando o comportamento esperado, é necessário verificar a configuração do campo **“Incide sobre Médias”**, pois essa parametrização impacta diretamente na forma como o evento será considerado nos cálculos.

### **Verificação da configuração dos eventos**

Acesse o cadastro de cada evento (Pessoal+ » Cadastros » Eventos) e verifique as seguintes configurações:

![1](https://ajuda.sankhya.com.br/hc/article_attachments/39387221483159)  Localize o evento desejado que está apresentando divergência no cálculo de médias.  
  
![2](https://ajuda.sankhya.com.br/hc/article_attachments/39387234411543)  Verifique, na aba **Avançado**, o campo **“Incide sobre Médias”** e valide como está configurado o evento em questão. Caso o objetivo seja que o evento componha a base de cálculo de outros eventos, a configuração deve ser ajustada para **“Incorpora ao Salário”**. Já nos cenários em que o evento deve compor as médias de cálculo do colaborador, é necessário configurá-lo para incidir como média, seja **por índice** ou **por valor**, conforme a necessidade do cálculo.  
 

![](https://ajuda.sankhya.com.br/hc/article_attachments/40751754062487)

![](https://ajuda.sankhya.com.br/hc/article_attachments/40755242677783)

  
![3](https://ajuda.sankhya.com.br/hc/article_attachments/39387221486103)  Após realizar a alteração, exclua o cálculo da folha já processada.  
  
![4](https://ajuda.sankhya.com.br/hc/article_attachments/39387221489431)  Calcule novamente a folha para que o sistema processe os eventos com a nova configuração.  
 

**Observação:** Quando o evento é configurado para incidir nas médias pelo valor, ele buscará exatamente o valor calculado na época, conforme exibido na tela de “Acumulados do Ano”, sem qualquer ajuste ou reajuste posterior.

Por outro lado, quando o evento está configurado para incidir nas médias pelo índice, esses valores serão ajustados caso o funcionário tenha recebido um reajuste salarial durante o período apurado.

### **Validação do cálculo**

Após realizar os ajustes, valide se os valores estão sendo processados corretamente:

![1](https://ajuda.sankhya.com.br/hc/article_attachments/39387221483159)  Consulte no calculo da folha do colaborador na aba de '**médias**'  para verificar se os eventos configurados estão sendo apresentados.  
  
![2](https://ajuda.sankhya.com.br/hc/article_attachments/39387234411543)  Consulte a regra de calculo (Pessoal+ » Cadastros » Regras de Cálculo) da empresa para verificar a forma de apuração de médias.

![](https://ajuda.sankhya.com.br/hc/article_attachments/40777800395159)

  
![3](https://ajuda.sankhya.com.br/hc/article_attachments/39387221486103)  Valide se o valor final da média de férias ou 13° salário está compatível com os valores dos eventos e os adicionais devidos.  
 

Seguindo essas orientações, os eventos de horas extras e adicionais noturnos passarão a compor corretamente as médias no cálculo, evitando divergências nos valores pagos aos colaboradores.