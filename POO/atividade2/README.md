### Classe Estoque

Modele uma classe chamada **Estoque** na qual será estática, ou seja, não possui constructor, apenas métodos ou propriedades estáticas. Dito isso crie a propriedade:

- controleEstoque = Tipo array - iniciado com esse array de objetos:

```javaScript
[
    {produto: "banana", precos: {promocao: 2.50,  normal: 3}, emPromocao: false},
    {produto: "arroz", preco: {promocao: 6.99,  normal: 8}, emPromocao: true},
]
```

Fique a vontade para aumentar esse array seguindo sempre esses pontos:

- produto - Tipo String - Referente ao nome do produto
- precos - Tipo Objeto - sempre terá as chaves promocao e normal:
- promocao - Tipo Number - Referente ao preço do produto em promoção
- normal - Tipo Number - Referente ao preço do produto quando não está em promoção
- emPromocao - Tipo Boleano - Referente a se o produto está ou não em promoção

### Método adicionarProduto

Crie um método chamado **adicionarProduto** na qual deve receber por parâmetros os mesmo parâmetros passados acima: **produto**, **precos**, **emPromocao**.
E tem como finalidade apenas adicionar esse novo produto ao **controleEstoque**.

Como Extra, que tal criar uma classe chamada **Produto** para fazer a modelagem desse produto? Fica a dica!

### Classe Cliente

Modele uma classe chamada **Cliente** na qual recebe a seguinte propriedades:

- nome - Tipo String
- saldo - Tipo Number

Além delas adicione essa propriedade predefinida:

- produtosComprados - Tipo Array - Iniciado como array vazio

### Método comprarProduto

Crie um método chamado **comprarProduto** na qual recebe por parâmetro o nome do produto no qual quer fazer a compra, dito isso esse método deve fazer o seguinte:

- Verificar se esse produto existe no **controleEstoque** da classe **Estoque**
- Caso exista deverá verificar se o produto está ou não em promoção
- Verificar se o cliente tem o valor suficiente para comprar o produto
- Caso tenha, adicionar o produto ao array **produtosComprados**
- Retirar so **saldo** o valor pago pelo produto
- Por fim, retorne um objeto da seguinte forma:

```javaScript
{
    nome: NOME DO PRODUTO,
    preco: PRECO DO PRODUTO
}
```
