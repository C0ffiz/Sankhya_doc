# Geração de documentos extemporâneos no EFD - ICMS/IPI

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360052376694-Gera%C3%A7%C3%A3o-de-documentos-extempor%C3%A2neos-no-EFD-ICMS-IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360052376694-Gera%C3%A7%C3%A3o-de-documentos-extempor%C3%A2neos-no-EFD-ICMS-IPI)

---

# Geração de documentos extemporâneos no EFD - ICMS/IPI

#### **Geração de NF-e de Emissão Própria como extemporâneo**

Para que seja possível a geração de NF-e de emissão própria como extemporâneo, é necessário que você, primeiramente, habilite o parâmetro **"Permite informar data extemporâneos na CAF? - DOCEXTEMP"**; assim, será utilizada a data extemporânea do lançamento para definição, a data do movimento do livro fiscal e será gerada a informação do campo COD\_SIT do registro C100 igual a 01 (Escrituração extemporânea de documento regular).

**Observação:** quando o parâmetro acima estiver habilitado, você conseguirá alterar a NF-e de emissão própria que está com o status de aprovada.

---

**Geração de CT-e de terceiros como extemporâneo**

O parâmetro **"Permite informar data extemporânea no Financeiro - DOCMOVFINEXTEMP"** influenciará na geração do CT-e de terceiros como extemporâneo. Com ele ligado, será habilitado o campo de Data Extemporânea na [Movimentação Financeira](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044601874); assim, com o parâmetro habilitado e o campo Data Extemporânea preenchido, o lançamento será registrado no Livro para o período informado na Data Extemporânea, e o campo 06 (COD\_SIT) do registro D100 informando 01 (Escrituração extemporânea de documento regular) do EFD - ICMS/IPI.