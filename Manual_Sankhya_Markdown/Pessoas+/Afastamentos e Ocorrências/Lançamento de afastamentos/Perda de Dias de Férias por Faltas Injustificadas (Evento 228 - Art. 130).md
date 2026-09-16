# Perda de Dias de Férias por Faltas Injustificadas (Evento 228 - Art. 130)

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/42490629375511-Perda-de-Dias-de-F%C3%A9rias-por-Faltas-Injustificadas-Evento-228-Art-130](https://ajuda.sankhya.com.br/hc/pt-br/articles/42490629375511-Perda-de-Dias-de-F%C3%A9rias-por-Faltas-Injustificadas-Evento-228-Art-130)

---

# Perda de Dias de Férias por Faltas Injustificadas (Evento 228 - Art. 130)

**Módulo:** Pessoal+  
**Caminho de Acesso:** Pessoal+ > Rotinas Folha > Faltas  
**ID da Tela:** Não se aplica (conteúdo de referência)

---

## **Descrição e Usabilidade**

### **1\. Descrição da Funcionalidade**

Este artigo explica como o sistema aplica a regra prevista no **Art. 130 da CLT**, que determina a redução dos dias de férias do colaborador conforme a quantidade de faltas injustificadas registradas durante o período aquisitivo.

O cálculo é realizado automaticamente pelo sistema com base nas faltas lançadas na tela **Faltas** e utiliza o **Evento 228 – Art. 130** para aplicar o impacto correspondente nos cálculos de férias.

### **2\. Pré-requisitos**

*   Faltas injustificadas lançadas na tela **Faltas** **(****Pessoal+ > Rotinas Folha****)** dentro do período aquisitivo do colaborador.
*   Evento 228 – Art. 130 configurado no cadastro de **Eventos**.
*   Período aquisitivo de férias existente para o colaborador.

### **3\. Como funciona a perda de dias de férias**

De acordo com o **Art. 130 da CLT**, a quantidade de dias de férias a que o colaborador tem direito pode ser reduzida conforme o número de faltas injustificadas no período aquisitivo.

<table class="wysiwyg-table-resized"><colgroup><col style="width: 46%;"> <col style="width: 54%;"></colgroup><tbody><tr><td style="background-color: #bcedb8;"><strong>Qtde. de faltas injustificadas</strong></td><td style="background-color: #bcedb8;"><strong>Dias de direito a férias</strong></td></tr><tr><td>Até 5</td><td>30</td></tr><tr><td>6 a 14</td><td>24</td></tr><tr><td>15 a 23</td><td>18</td></tr><tr><td>24 a 32</td><td>12</td></tr><tr><td>Acima de 32</td><td>Perde o direito às férias do período aquisitivo</td></tr></tbody></table>

As faltas justificadas não são consideradas nesse cálculo.

### **4\. Como o sistema aplica o cálculo**

O sistema considera a quantidade de faltas injustificadas registradas no período aquisitivo e aplica a redução correspondente nos cálculos de férias.

O **Evento 228 – Art. 130** é utilizado para calcular o impacto financeiro quando houver valores proporcionais de férias envolvidos, como em cálculos de rescisão.

Para aplicar essa regra nos cálculos relacionados às férias proporcionais, o evento 228 utiliza a seguinte fórmula:

<table><tbody><tr><td><em>IF(&amp;FerPro &gt; 0, ((@E_FERIASPROPRESCISOES + @E_MEDIASFERIASPROPRESCISAO) * 1.33333) / &amp;FerPro * &amp;FALTASPRO, 0)</em></td></tr></tbody></table>

Interpretação da fórmula:

*   `IF(&FerPro > 0, ... , 0)`: executa o cálculo somente quando existem avos de férias proporcionais. 
*   `@E_FERIASPROPRESCISOES + @E_MEDIASFERIASPROPRESCISAO`: soma o valor das férias proporcionais e das médias de férias proporcionais. 
*   `* 1.33333`: aplica o adicional constitucional de 1/3 de férias. 
*   `/ &FerPro`: divide pelo número de avos de férias proporcionais. 
*   `* &FALTASPRO`: multiplica pela quantidade de faltas proporcionais consideradas no cálculo.

**Exemplo:** 

Considerando:

*   **Avos de férias proporcionais (&FerPro):** 8
*   **Férias proporcionais:** R$ 1.012,00
*   **Médias de férias proporcionais:** R$ 172,87
*   **Quantidade de faltas proporcionais:** 4,8

Cálculo:

*   Férias proporcionais + médias:  
    R$ 1.012,00 + R$ 172,87 = R$ 1.184,87
*   Aplicação do terço constitucional:  
    R$ 1.184,87 × 1,33333 = R$ 1.579,82
*   Valor por avo:  
    R$ 1.579,82 ÷ 8 = R$ 197,47
*   Resultado do evento:  
    R$ 197,47 × 4,8 = **R$ 947,89**

### **5\. Pontos de Atenção**

*   Somente faltas injustificadas são consideradas para aplicação da regra do Art. 130 da CLT.
*   Sem avos de férias proporcionais (`&FerPro = 0`), o resultado do cálculo do evento 228 será zero.
*   A quantidade de faltas considerada no cálculo corresponde às faltas injustificadas registradas durante o período aquisitivo.

### **6\. Dicas de Usabilidade**

*   Registre as faltas injustificadas assim que ocorrerem para garantir que os cálculos de férias e rescisão utilizem informações atualizadas.
*   Antes de validar um cálculo de férias ou rescisão, confira os lançamentos de faltas do colaborador.

## **Perguntas Frequentes (FAQ)**

**1\. Faltas justificadas reduzem os dias de férias?**

Não. Apenas as faltas injustificadas são consideradas para aplicação da regra prevista no Art. 130 da CLT.

**2\. O cálculo da perda de dias de férias é manual?**

Não. O sistema realiza o cálculo automaticamente conforme as faltas lançadas e a configuração do evento 228.

**3\. Onde devo lançar as faltas consideradas nesse cálculo?**

As faltas devem ser lançadas na tela **Faltas** (**Pessoal+ > Rotinas Folha**).

**4\. O evento 228 precisa ser lançado manualmente?**

Não. O evento é utilizado pelo sistema durante os cálculos em que essa regra deve ser aplicada.

## **Artigos Relacionados**

*   [Lançamento de Faltas na Folha de Pagamento](https://ajuda.sankhya.com.br/hc/pt-br/articles/42468035034647)
*   [Lançamento de Faltas com Suspensão Disciplinar na Folha de Pagamento](https://ajuda.sankhya.com.br/hc/pt-br/articles/42468830204567)
*   [Restituição de Faltas na Folha de Pagamento](https://ajuda.sankhya.com.br/hc/pt-br/articles/42487033706519)
*   [Cadastro de Eventos](https://ajuda.sankhya.com.br/hc/pt-br/articles/33041194565911)