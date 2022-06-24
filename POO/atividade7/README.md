## POO

### Class Livro

Modele uma classe chamada **Livro** que precisa receber exatamente as seguintes propriedades no construtor via parâmetro:

- titulo - Tipo **String**
- autor - Tipo **String**
- precoVenda - Tipo **Number**
- precoCompra - Tipo **Number**

### Class Livraria

Modele uma classe chamada **Livraria** que precisa receber exatamente a seguinte propriedade no construtor via parâmetro:

- nome - Tipo **String**

E além dessa, também existirá as seguintes propriedades predefinidas (default):

- estoque - Tipo **Array** - Predefinida como um objeto vazio
- caixa - Tipo **Number** - Predefinida com o número 100

Por fim, desenvolva os seguintes métodos para essa classe:

#### Method comprarLivros

Esse método receberá dois parâmetros:

- livro - Tipo **Objeto** instanciado através da classe Livro
- qtdLivros - Tipo **Number** | representa a quantidade de livros a ser comprada.

A finalidade desse método é adicionar o(s) livro(s) e sua(s) quantidade(s) ao estoque, isso caso a livraria tenha dinheiro suficiente para realizar a compra. Caso o dinheiro em caixa seja suficiente:

1. crie uma nova propriedade no objeto **livro** chamada **qtd** e atribua o valor de qtdLivros, que foi recebido por parâmetro, a ela.
2. adicione o livro ao array de estoque.
3. Retorne o objeto abaixo:

```javaScript
{
   mensagem: 'Compra realizada com sucesso!'
}
```

Caso a livraria não tenha dinheiro suficiente, o método deverá retornar a seguinte mensagem, também em forma de objeto:

```javaScript
{
   mensagem: 'Valor em caixa não é suficiente para essa compra!'
}
```

#### Method venderLivros

Esse método receberá dois parâmetros:

- livro - Tipo **Objeto** instanciado através da classe Livro
- qtdLivros - Tipo **Number** | representa a quantidade de livros a serem vendidos. Caso o usuário não passe esse parâmetro, ele terá o valor default igual a 1.

Esse método verifica se existem livros suficientes em estoque para realizar a venda. Caso existam livros suficientes, o método deverá:

1. Reduzir a quantidade de livros vendidos do estoque
2. Verificar qual o valor total da venda
3. Adicionar o valor total da venda ao caixa da livraria
4. Retornar o objeto abaixo com os valores especificados:

```javaScript
{
   mensagem: "(QUANTIDADE DE LIVROS) livros foram vendidos e foi faturado (VALOR TOTAL DA VENDA)"
}
```

Caso a quantidade de livros em estoque não seja suficiente para realizar a venda, o objeto abaixo deverá ser retornado:

```javaScript
{
   mensagem: "A quantidade de livros em estoque não é suficiente para essa venda!"
}
```
