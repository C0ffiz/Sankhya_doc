# Liberação de limite orçamentário do tipo Mensal

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360045226793-Libera%C3%A7%C3%A3o-de-limite-or%C3%A7ament%C3%A1rio-do-tipo-Mensal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045226793-Libera%C3%A7%C3%A3o-de-limite-or%C3%A7ament%C3%A1rio-do-tipo-Mensal)

---

# Liberação de limite orçamentário do tipo Mensal

Abaixo, tem-se um cenário de como funcionará a solicitação de liberação de limite orçamentário para o tipo Mensal:

**![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28454044600343)** **Orçamento previsto: 2.500,00**

<table border="1" style="border-collapse: collapse; width: 100%; height: 100px;"><tbody><tr style="height: 22px;"><td style="width: 25%; height: 22px;">&nbsp;</td><td class="wysiwyg-text-align-center" style="width: 25%; height: 22px;"><strong>Renato</strong></td><td class="wysiwyg-text-align-center" style="width: 25%; height: 22px;"><strong>Ricardo</strong></td><td class="wysiwyg-text-align-center" style="width: 25%; height: 22px;"><strong>Cristiano</strong></td></tr><tr style="height: 22px;"><td style="width: 25%; height: 22px;"><strong>&nbsp;Pode liberar até</strong></td><td style="width: 25%; height: 22px;">&nbsp;1.000,00</td><td style="width: 25%; height: 22px;">&nbsp;2.000,00</td><td style="width: 25%; height: 22px;">&nbsp;3.000,00</td></tr><tr style="height: 22px;"><td style="width: 25%; height: 22px;"><strong>&nbsp;Pode antecipar</strong></td><td style="width: 25%; height: 22px;">&nbsp;Sim</td><td style="width: 25%; height: 22px;">&nbsp;Sim</td><td style="width: 25%; height: 22px;">&nbsp;Sim</td></tr><tr style="height: 22px;"><td style="width: 25%; height: 22px;"><strong>&nbsp;Pode suplementar</strong></td><td style="width: 25%; height: 22px;">&nbsp;Não</td><td style="width: 25%; height: 22px;">&nbsp;Sim</td><td style="width: 25%; height: 22px;">&nbsp;Sim</td></tr><tr style="height: 22px;"><td style="width: 25%; height: 22px;"><strong>&nbsp;Pode transferir</strong></td><td style="width: 25%; height: 22px;">&nbsp;Não</td><td style="width: 25%; height: 22px;">&nbsp;Sim</td><td style="width: 25%; height: 22px;">&nbsp;Sim</td></tr></tbody></table>

---

No cenário acima descrito, o usuário Renato poderá apenas suplementar. No caso, ele poderá efetuar liberações mensais de até 1.000,00 de suplementação.

Já o usuário Ricardo pode antecipar, suplementar e transferir liberações mensais de até 2.000,00.

Por último, o usuário Cristiano também poderá antecipar, suplementar e transferir, porém, liberações mensais de até 3.000,00.

Desta forma, segue abaixo o caso de uso:

**![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28454044600343)** **Renato \- Suplementação:**

*   O vendedor lançou um documento no valor de R$1.500,00 e solicita sua confirmação;
*   O sistema processa o lançamento e não solicita liberação, visto que o orçamento previsto é de R$2.500,00;
*   O vendedor lança um segundo documento no valor de R$1.200,00 e solicita sua confirmação;
*   O sistema processa o lançamento e solicita uma liberação no valor de R$200,00 para o usuário Renato, visto que o mesmo possui alçada para liberação;
*   O usuário Ricardo verifica a liberação e efetua uma suplementação no valor solicitado;
*   O vendedor solicita a confirmação do documento;
*   O sistema processa o lançamento e confirma o documento, visto que houve a liberação (suplementado).

<table border="1" style="border-collapse: collapse; width: 100%;"><tbody><tr><td style="width: 25%;"><strong>&nbsp;Usuário</strong></td><td style="width: 25%;"><strong>&nbsp;Suplementação</strong></td><td style="width: 25%;"><strong>&nbsp;Antecipação</strong>&nbsp;</td><td style="width: 25%;"><strong>&nbsp;Transferência</strong></td></tr><tr><td style="width: 25%;">&nbsp;Renato</td><td style="width: 25%;">&nbsp;200,00&nbsp;</td><td style="width: 25%;">&nbsp;0,00&nbsp;</td><td style="width: 25%;">&nbsp;0,00&nbsp;</td></tr><tr><td style="width: 25%;">&nbsp;Ricardo</td><td style="width: 25%;">&nbsp;0,00</td><td style="width: 25%;">&nbsp;0,00</td><td style="width: 25%;">&nbsp;0,00</td></tr><tr><td style="width: 25%;">&nbsp;Cristiano</td><td style="width: 25%;">&nbsp;0,00</td><td style="width: 25%;">&nbsp;0,00</td><td style="width: 25%;">&nbsp;0,00</td></tr></tbody></table>

**![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28454044600343)** **Ricardo \- Suplementação****:**

*   O vendedor lança um documento no valor de R$1.000,00 e solicita sua confirmação;
*   O sistema processa o lançamento e solicita uma liberação no valor de R$1.000,00 para o usuário Ricardo, visto que Renato, o qual possui um limite de R$1.000,00 mensais não possui alçada (200 + 1.000 = 1.200);
*   Ricardo verifica a liberação e efetua a suplementação do valor solicitado;
*   O vendedor solicita a confirmação do documento;
*   O sistema processa o lançamento e confirma o documento, já que houve a liberação. 

<table border="1" style="border-collapse: collapse; width: 100%;"><tbody><tr><td style="width: 25%;"><strong>&nbsp;Usuário</strong></td><td style="width: 25%;"><strong>&nbsp;Suplementação</strong></td><td style="width: 25%;"><strong>&nbsp;Antecipação</strong>&nbsp;</td><td style="width: 25%;"><strong>&nbsp;Transferência</strong></td></tr><tr><td style="width: 25%;">&nbsp;Renato</td><td style="width: 25%;">&nbsp;200,00&nbsp;</td><td style="width: 25%;">&nbsp;0,00&nbsp;</td><td style="width: 25%;">&nbsp;0,00&nbsp;</td></tr><tr><td style="width: 25%;">&nbsp;Ricardo</td><td style="width: 25%;">&nbsp;1.000,00&nbsp;</td><td style="width: 25%;">&nbsp;0,00</td><td style="width: 25%;">&nbsp;0,00</td></tr><tr><td style="width: 25%;">&nbsp;Cristiano</td><td style="width: 25%;">&nbsp;0,00</td><td style="width: 25%;">&nbsp;0,00</td><td style="width: 25%;">&nbsp;0,00</td></tr></tbody></table>

**![Marcador 1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/28454044600343)** **Cristiano - Suplementação****:**

*   O vendedor lança um documento no valor de R$1.200,00 e solicita sua confirmação;
*   O sistema processa o lançamento e solicita uma liberação no valor de R$1.200,00 para Ricardo, visto que Renato ainda pode antecipar ou transferir;

Neste cenário podem existir duas situações:

![1 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16371136682391) Caso o vendedor escolha suplementar, o sistema reavaliará o lançamento e solicitará uma liberação ao Cristiano, visto que Ricardo não possui alçada para suplementar este valor (1.000,00 + 1.200,00 = 2.000,00).

![2 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16371128422935) Caso não se escolha o tipo de liberação, o sistema irá solicitar a liberação para Ricardo, o qual poderá apenas antecipar ou transferir.

Seguindo a primeira situação:

*   Cristiano verifica a liberação e efetua uma suplementação;
*   O vendedor solicita a confirmação do documento;
*   O sistema processa o lançamento e confirma o documento, já que houve a liberação.