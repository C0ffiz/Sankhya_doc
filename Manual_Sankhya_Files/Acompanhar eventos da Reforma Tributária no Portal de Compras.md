# Acompanhar eventos da Reforma Tributária no Portal de Compras

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/35812909713687-Acompanhar-eventos-da-Reforma-Tribut%C3%A1ria-no-Portal-de-Compras](https://ajuda.sankhya.com.br/hc/pt-br/articles/35812909713687-Acompanhar-eventos-da-Reforma-Tribut%C3%A1ria-no-Portal-de-Compras)

---

# Acompanhar eventos da Reforma Tributária no Portal de Compras

**Módulo:** Compras / Fiscal  
**Versão mínima:** 4.35 build 261 / 4.34 build 246 / 4.33 build 180 / mgeliv 5.17.9  
**Caminho de acesso:** **Portal de Compras › NF-e › Acompanhamento de Eventos Reforma Tributária**

**Você encontra neste artigo:**

<table class="wysiwyg-table-resized" style="border-collapse: collapse;"><colgroup><col style="width: 50%;"> <col style="width: 50%;"></colgroup><tbody><tr><td style="border-color: #999; padding: 8px; text-align: left; vertical-align: top;"><a href="#oque">O que é e para que serve</a><br><a href="#antes">Antes de começar</a><br><a href="#fluxo">Diagrama de fluxo</a><br><a href="#acessando">Acessando eventos</a><br><a href="#enviando">Enviando eventos</a><br>&nbsp;&nbsp;&nbsp;↳ <a href="#ev211110">Evento 211110: Solicitação de Apropriação de Crédito Presumido</a></td><td style="border-color: #999; padding: 8px; text-align: left; vertical-align: top;">&nbsp;&nbsp;&nbsp;↳ <a href="#ev211120">Evento 211120: Destinação para Consumo Pessoal</a><br>&nbsp;&nbsp;&nbsp;↳ <a href="#ev211124">Evento 211124: Perecimento, Perda, Roubo ou Furto</a><br>&nbsp;&nbsp;&nbsp;↳ <a href="#ev211128">Evento 211128: Aceite de Débito na Apuração</a><br>&nbsp;&nbsp;&nbsp;↳ <a href="#ev211130">Evento 211130: Imobilização de Item</a><br>&nbsp;&nbsp;&nbsp;↳ <a href="#ev211140">Evento 211140: Solicitação de Crédito de Combustível</a><br>&nbsp;&nbsp;&nbsp;↳ <a href="#ev211150">Evento 211150: Solicitação de Crédito para Bens e Serviços</a><br><a href="#cancelando">Cancelando eventos</a><br><a href="#pontos-atencao">Pontos de atenção</a><br><a href="#faq">Perguntas frequentes</a></td></tr></tbody></table>

---

## O que é e para que serve

O pop-up **Acompanhamento de Eventos Reforma Tributária** no [Portal de Compras](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045111953-Portal-de-Compras) permite que o destinatário da NF-e registre eventos fiscais diretamente à SEFAZ, como destinação para consumo pessoal, perecimento, aceite de débito, imobilização de itens e solicitação de crédito. O recurso garante conformidade com a legislação, facilita a gestão de ocorrências e permite o cancelamento individual de eventos. Apenas o destinatário da NF-e pode registrar eventos nesta tela.

---

## Antes de começar

*   Acesso ao [Portal de Compras](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045111953-Portal-de-Compras) com permissão para utilizar a funcionalidade **Acompanhamento de Eventos Reforma Tributária**.

## Diagrama de fluxo

O fluxo abaixo resume as etapas do processo de registro e cancelamento de eventos da Reforma Tributária no Portal de Compras:

![](https://ajuda.sankhya.com.br/hc/article_attachments/35812915725975)

_Etapas em verde representam ações do usuário. A etapa em vermelho (Cancelar evento) é condicional — ocorre apenas quando necessário._

---

## Acessando eventos

No [Portal de Compras](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045111953-Portal-de-Compras), selecione a nota para a qual deseja registrar um evento. Clique no botão **NF-e** e selecione **Acompanhamento de Eventos Reforma Tributária**.

![](https://ajuda.sankhya.com.br/hc/article_attachments/35812915728151)

O pop-up será aberto, onde você poderá enviar ou cancelar eventos de responsabilidade do destinatário.

---

## Enviando eventos

Selecione a aba **Envio**. No campo **Selecione o Evento**, escolha o evento desejado na lista de eventos disponíveis para o destinatário.

![](https://ajuda.sankhya.com.br/hc/article_attachments/35812915732631)

Na grade de itens da nota, selecione os itens que farão parte da transmissão. Para alguns eventos, você pode ajustar a **Quantidade do Evento** e a **Unidade** dos itens selecionados.

![](https://ajuda.sankhya.com.br/hc/article_attachments/35812915733143)

O sistema exibe informações detalhadas dos impostos para cada item: **Valor IBS**, **Valor CBS** e **Valor base Unitário**. Clique em **Enviar Evento** para finalizar.

### Evento 211110: Solicitação de Apropriação de Crédito Presumido

Permite ao destinatário enviar a solicitação de apropriação de crédito presumido sobre as notas fiscais de aquisição de terceiros, garantindo o direito ao crédito fiscal.

**⚠️ Atenção**

As alíquotas de IBS e CBS devem estar configuradas com o código de classificação e o percentual do crédito presumido corretos. O sistema valida se o CNPJ/CPF de quem envia é idêntico ao do destinatário da nota e se o item informado existe na NF-e original. Caso contrário, o sistema gera a Rejeição 575 (autor não é o destinatário) ou a Rejeição 1096 (item não existe no documento original).

Por determinação legal, este evento foi removido do Portal de Vendas e é de uso exclusivo no Portal de Compras. O sistema possui trava de segurança que impede o reenvio de eventos duplicados para uma mesma nota fiscal.

### Evento 211120: Destinação de Item para Consumo Pessoal

Informa ao governo que um item de uma compra foi destinado para consumo pessoal (pessoa física), o que anula o direito de apropriação do crédito fiscal.

**ℹ️ Nota**

Aplica-se à NF-e modelo 55. Permite o registro de múltiplos eventos para a mesma nota. Como o evento é por item, você pode editar a **Quantidade do Evento** e a **Unidade** para informar a quantidade exata destinada ao consumo.

### Evento 211124: Perecimento, Perda, Roubo ou Furto

Comunica a ocorrência de perecimento, perda, roubo ou furto de mercadorias durante o transporte. Aplica-se a casos em que o frete foi contratado pelo adquirente (modalidade FOB).

**ℹ️ Nota**

Aplica-se à NF-e modelo 55. Você pode editar a **Quantidade do Evento** e a **Unidade** para informar a quantidade exata de produtos afetados.

### Evento 211128: Aceite de Débito na Apuração

Permite que o destinatário aceite um débito na apuração de impostos gerado pela emissão de uma nota de crédito, ajustando corretamente o valor do débito fiscal.

**ℹ️ Nota**

Como este evento se refere à nota completa, os campos de quantidade e unidade não são editáveis.

### Evento 211130: Imobilização de Item

Informa ao Fisco que um item foi integrado ao ativo imobilizado, o que ajuda a controlar prazos para futuros pedidos de ressarcimento de crédito.

**ℹ️ Nota**

Você pode editar a **Quantidade do Evento** e a **Unidade** para informar a quantidade exata de produtos imobilizados.

### Evento 211140: Solicitação de Crédito de Combustível

Solicita a apropriação de um crédito fiscal relacionado à aquisição de combustível. O cancelamento deste evento segue o mesmo processo padrão descrito na seção [Cancelando eventos](#cancelando).

### Evento 211150: Solicitação de Crédito para Bens e Serviços

Solicita a apropriação de um crédito fiscal para bens e serviços cuja utilização depende da atividade econômica do destinatário. O cancelamento deste evento segue o mesmo processo padrão descrito na seção [Cancelando eventos](#cancelando).

---

## Cancelando eventos

É possível cancelar um evento já enviado — por exemplo, em caso de erro.

1.  No pop-up, localize e selecione o evento que deseja cancelar.
2.  Clique em **Cancelar Evento** para solicitar o cancelamento.

**ℹ️ Nota**

Uma mesma nota pode ter vários eventos, e cada um gera um protocolo único — você pode cancelá-los individualmente. Consulte o histórico de eventos na aba **Acompanhamento** para rastrear todas as comunicações realizadas.

---

## Pontos de atenção

*   Apenas o destinatário da NF-e pode registrar eventos nesta tela.
*   Eventos 211120, 211124 e 211130 permitem editar quantidade e unidade por item.
*   Eventos 211128, 211140 e 211150 não permitem edição de quantidade e unidade.
*   Para o Evento 211110, o sistema gera a Rejeição 575 se o autor não for o destinatário da nota, e a Rejeição 1096 se o item selecionado não existir no documento original.
*   Cada evento gera um protocolo único e pode ser cancelado individualmente.
*   Um mesmo item pode ter vários eventos registrados.

**💡 Dica**

Para mais informações, consulte também:

*   [Portal de Compras](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045111953-Portal-de-Compras)
*   [Guia da Reforma Tributária](https://ajuda.sankhya.com.br/hc/pt-br/categories/34702076010775-Reforma-tribut%C3%A1ria)

---

## Perguntas frequentes

### Quem pode registrar eventos fiscais no Portal de Compras?

Apenas o destinatário da NF-e.

### Posso editar a quantidade de itens em todos os eventos?

Não. A edição de quantidade e unidade está disponível apenas nos eventos 211120, 211124 e 211130.

### Como cancelar um evento já enviado?

Acesse a aba **Acompanhamento**, selecione o evento e clique em **Cancelar Evento**.

### Um mesmo item pode ter mais de um evento?

Sim. Cada evento gera um protocolo único e pode ser cancelado individualmente.

### Por que não encontro o Evento 211110 no Portal de Vendas?

Por determinação da Nota Técnica 2025.002, a solicitação de apropriação de crédito presumido é de uso exclusivo da empresa destinatária. A opção foi removida do Portal de Vendas e movida exclusivamente para o Portal de Compras.