# Ajuste de Incidência de IRRF (CODINCIRRF)

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/37827360294295-Ajuste-de-Incid%C3%AAncia-de-IRRF-CODINCIRRF](https://ajuda.sankhya.com.br/hc/pt-br/articles/37827360294295-Ajuste-de-Incid%C3%AAncia-de-IRRF-CODINCIRRF)

---

# Ajuste de Incidência de IRRF (CODINCIRRF)

O **Código de Incidência do IRRF (CODINCIRRF)** de determinadas verbas da folha de pagamento **foi ajustado** para **corrigir o enquadramento tributário dessas rubricas**.

Os ajustes realizados foram:

*   a **maior parte das verbas** teve o CODINCIRRF alterado de **79 para 09**;
    
*   a rubrica **MULTA FGTS** teve o CODINCIRRF alterado de **74 para 09**.
    

A lista completa das rubricas ajustadas está disponível ao final deste artigo.

![Atenção FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/37827377069079)**Importante** 

*   A incidência anteriormente utilizada **não gerou impacto financeiro** nem para o colaborador, nem para o empregador.
*   Isso ocorreu porque as verbas estavam classificadas com **CODINCIRRF = 79 (Outras isenções)** e, por esse motivo, **não compunham a base de cálculo do IRRF**.

<table style="border-style: none;"><tbody><tr><td style="background-color: #66cc66; vertical-align: middle;"><strong>Por que esse ajuste foi necessário?</strong></td></tr></tbody></table>

O ajuste foi realizado porque algumas verbas estavam sendo tratadas como **rendimentos isentos de Imposto de Renda**, quando, na prática, são **verbas que apenas transitam pela folha**, sem natureza de rendimento.

Com a correção da classificação, garante-se que:

*   o **Imposto de Renda seja apurado corretamente**;
    
*   as informações enviadas ao **eSocial estejam corretas**;
    
*   a **DIRF 2026** (substituída pelo eSocial) seja gerada **sem inconsistências**;
    
*   o **Informe de Rendimentos do colaborador** apresente os valores de forma clara e correta.
    

<table style="border-style: none;"><tbody><tr><td style="background-color: #66cc66;"><strong>O que significa cada código de incidência?</strong></td></tr></tbody></table>

*   **CODINCIRRF = 79 — Outras isenções**
    
    Utilizado para **rendimentos isentos por lei** que não estão listados na **Tabela 21 do eSocial**, cuja natureza do pagamento deve ser explicitada no nome da rubrica.
    
    Essas informações:
    
    *   compõem os totalizadores do **evento S-5002**;
        
    *   são apresentadas no **Informe de Rendimentos**, com a descrição da rubrica que compôs as outras isenções.
        
*   **CODINCIRRF = 09 — Verba transitada pela folha de pagamento de natureza diversa de rendimento ou retenção/isenção/dedução de IR.**
    
    Utilizado para verbas que **transitam pela folha de pagamento**, mas que **não possuem natureza de rendimento, retenção, isenção ou dedução de IR**.
    
    **Por exemplo:** desconto de convênio farmácia, consignações, adiantamentos e outras verbas sem natureza tributável.
    
*   **CODINCIRRF = 74 — Indenização e rescisão de contrato, inclusive a título de PDV e acidentes de trabalho**
    
    Utilizado para identificar rubricas de **indenização e rescisão do contrato de trabalho**, incluindo:
    
    *   rescisões contratuais;
        
    *   PDV;
        
    *   indenizações por acidente de trabalho.
        

<table style="border-style: none;"><tbody><tr><td style="background-color: #66cc66;"><strong>O que muda na prática?</strong></td></tr></tbody></table>

Após o ajuste:

*   As verbas transitórias **não serão exibidas mais como rendimento isento** no Informe de Rendimentos.
    
*   Os valores enviados ao eSocial ficarão corretos nos eventos:
    
    *   **S-5002** (IRRF do trabalhador);
        
    *   **S-5012** (IRRF do empregador).
        
*   O **Demonstrativo do Informe de Rendimentos** ficará mais claro, diferenciando o que é:
    
    *   rendimentos tributáveis;
        
    *   rendimentos isentos;
        
    *   verbas sem natureza de rendimento.
        

<table style="border-style: none;"><tbody><tr><td style="background-color: #66cc66;"><strong>O que o cliente precisa fazer?</strong></td></tr></tbody></table>

Para que o ajuste reflita corretamente nos **relatórios fiscais, eSocial e Informe de Rendimentos**, é necessário executar os passos abaixo.

**1\. Atualizar as rubricas na tela Eventos** (Pessoal+ > Cadastros).

**2\. Enviar o evento S-1010 (Tabela de Rubricas) pela Central do eSocial**

*   Enviar o **S-1010 das rubricas listadas** neste artigo;
    
*   Utilizar **nova data de início de validade**, **no mínimo a partir de 01/2025, já com o código CODINCIRRF ajustado**;
    

![acesse também FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/37828469843095) Consulte a documentação: [**Como enviar o evento S-1010 (Tabela de Rubricas) com nova validade no eSocial**](https://ajuda.sankhya.com.br/hc/pt-br/articles/37825585095447).

**2\.** Reabrir, por meio do evento S-1298, todas as referências do ano de 2025 em que houve o envio de alguma das rubricas mencionadas ao eSocial.

**3\.** Em seguida, bloquear as folhas de pagamento dessas competências e gerar o evento S-1210 (Pagamentos) de exclusão, realizando o respectivo envio ao eSocial.

**4\.** Após a exclusão, liberar as folhas, gerar o evento S-1210 (Pagamentos) de inclusão e efetuar o envio.

**5\.** Concluído esse processo, realizar o fechamento das competências com o envio do evento S-1299 (Fechamento).

**6.** Após o processamento desses eventos, o eSocial passará a considerar a nova incidência das rubricas, refletindo corretamente nos retornos S-5002 e no consolidado S-5012.

**7.** Por fim, após o envio dos eventos S-1010, repetir os passos 2 a 5 para todas as competências de 2025 em que tenham sido enviadas rubricas com a incidência anterior.

Após esses envios, o eSocial passará a considerar a **nova incidência** nos retornos:

*   **S-5002** (IRRF do trabalhador);
    
*   **S-5012** (consolidado do empregador).
    

Com isso, já será possível emitir os [**Demonstrativos do Informe de Rendimentos**](https://ajuda.sankhya.com.br/hc/pt-br/articles/20941208310167).

![fluxo correção irrf.gif](https://ajuda.sankhya.com.br/hc/article_attachments/37835114254743)

### **Lista de rubricas ajustadas**

![Atenção FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/37827377069079) Faça a busca pela **descrição do evento ou pela característica**, pois o código pode ser diferente na sua base.

<table class="wysiwyg-table-resized"><colgroup><col style="width: 9%;"> <col style="width: 31%;"> <col style="width: 31%;"> <col style="width: 15%;"> <col style="width: 14%;"></colgroup><tbody><tr><td style="background-color: #66cc66; text-align: center;"><strong>Código</strong></td><td style="background-color: #66cc66; text-align: center;"><strong>Descrição do Evento</strong></td><td style="background-color: #66cc66; text-align: center;"><strong>Característica</strong></td><td style="background-color: #66CC66;"><strong>CODINCIRRF ANTIGO</strong></td><td style="background-color: #66CC66;"><strong>CODINCIRRF ATUAL</strong></td></tr><tr><td style="text-align: center;">5</td><td>HONORARIOS TRANSPORTE</td><td>HONORARIOSTRANSPORTE</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">16</td><td>DESC. EXCEDENTE ADTO 13º SAL.</td><td>DESCADTODECTERMAIOR</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">18</td><td>ANTEC 13ºFERIAS LIC MATERNIDADE COMPET</td><td>ANTECIP13FERIASLICGE</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">20</td><td>DESC ANTEC 13 FERIAS LICGE COMP</td><td>DESCANTEC13FERIASLICGE</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">301</td><td>1ª PARCELA DO 13° SALARIO</td><td>1PARCELADO13SALARIO</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">303</td><td>MEDIAS 1ª PARCELA 13° SALARIO</td><td>MEDIAS1PARCELADO13SALARIO</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">305</td><td>DESC 1ª PARCELA DO 13° SALARIO</td><td>DESCONTO1PARC13SAL</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">306</td><td>DESC ANTECIPACAO 13° SALARIO</td><td>DESCANTECIP13SALARIO</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">308</td><td>1ª PARC 13º LIC MATERNIDADE</td><td>1PARC13SALLICGEST</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">312</td><td>ANTECI 13ºSAL FER LIC MATERNIDADE</td><td>ADIANT13SALFERIASLICGE</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">313</td><td>MEDIA 1ª PARC 13º LIC MATERNIDADE</td><td>MEDIAS1PARC13SALLICG</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">315</td><td>DESCONTO 1ª PARC 13º RESCISAO</td><td>DESCONTO1PARC13SALRESCISA</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">316</td><td>DESC1ªPARC 13ºBASE FGTS MENSAL</td><td>DESC1PARC13BASEFGTSMENSAL</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">318</td><td>1ª PARC 13º ACID TRAB</td><td>1PARC13SACIDTRAB</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">319</td><td>2ª PARC 13° ACID TRAB</td><td>2PARC13SACIDTRAB</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">320</td><td>DESC 1ª PARC 13º ACID TRAB</td><td>DESC1PARC13SACIDTRAB</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">321</td><td>DESC 1ª PARC 13º LIC MATERNIDADE</td><td>DESC1PARC13SLICMATER</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">328</td><td>MEDIAS 1ª PARC 13º AC TRAB</td><td>MEDIAS1PARC13ACTRAB</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">329</td><td>MEDIAS 2ª PARC 13º AC TRAB</td><td>MEDIAS2PARC13ACTRAB</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">330</td><td>1ª PARC 13º LIC MATERNIDADE CIDADA</td><td>1PAR13SALLICGESTCIDADA</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">331</td><td>MEDIA 1ª PARC 13º LIC MATERNIDADE CIDADA</td><td>MEDIAS1PA13SGESTCIDADA</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">334</td><td>DESC 1ª PARC 13º LIC MATERNIDADE CIDADA</td><td>DESC1PAR13SAGESTCIDADA</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">542</td><td>ACIDENTE TRABALHO</td><td>ACIDENTETRABALHO</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">563</td><td>MEDIAS ACIDENTE TRABALHO</td><td>MEDIASACIDENTETRABALHO</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">990</td><td>MULTA FGTS</td><td>MULTAFGTS</td><td>74</td><td>9</td></tr><tr><td style="text-align: center;">996</td><td>FGTS 13º SALARIO</td><td>FGTS13SALARIO</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">997</td><td>FGTS INDENIZACOES</td><td>FGTSRESCISORIO</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">1851</td><td>BASE IRRF TRANSPORTE</td><td>BASEIRRFREDUZIDATRANSP</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">3000</td><td>ANTECIPACAO 13º SALARIO</td><td>ANTECIPACAO13SALARIO</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">4090</td><td>DESCONTO DE ABONO ADIANTADO</td><td>DESCONTODEABONOADIANTADO</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">4300</td><td>ANTECIPACAO 13° FERIAS</td><td>ANTECIPACAO13SALPGFERIAS</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">4301</td><td>DESC ANTECIPACAO 13° FERIAS</td><td>DESCANTEC13SALPGFERIAS</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">9210</td><td>FGTS INTERMITENTE</td><td>FGTSINTERMITENTE</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">9220</td><td>FGTS 13° INTERMITENTE</td><td>FGTS13INTERMITENTE</td><td>79</td><td>9</td></tr><tr><td style="text-align: center;">9367</td><td>DESC ANTEC 13SAL FER LIC MATERNIDADE</td><td>DESCANTEC13SALFERLIC</td><td>79</td><td>9</td></tr></tbody></table>