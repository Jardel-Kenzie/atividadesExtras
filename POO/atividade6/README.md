## POO

### Class Email

Modele uma classe chamada **Email** que precisa receber exatamente as seguintes propriedades no construtor via parâmetro:

- email - Tipo **String**
- nome - Tipo **String**

E além dessas, também existirá a seguinte propriedade predefinida (default):

- conteudo - Tipo **Object** | Predefinida como um objeto vazio

Em seguida, desenvolva um método chamado **escreverEmail** que deverá receber os seguintes valores por parâmetro:

- assunto - Tipo **String**
- mensagem - Tipo **String**

Por fim, crie os atributos "assunto" e "mensagem" no objeto **conteudo** com seus respectivos valores recebidos por parâmetro e retorne o contexto.

### Class ServicoDeEmail

Modele uma classe chamada **ServicoDeEmail** que terá uma propriedade estática chamada **historico**, predefinida como um array vazio.

Após isso, desenvolva um método estático chamado **enviarEmail**, que receberá os seguintes valores por parâmetro:

- emailRemetente - Tipo **String**
- emailDestinatario - Tipo **String**

Esse método deverá verificar se o `emailRemetente` e `emailDestinatario` possuem valores, ou seja, são diferentes de **undefined**.

Caso sejam, os valores deverão ser considerados válidos, adicionando o seguinte objeto à propriedade **historico**:

```js
{
    emailRemetente: // EMAIL DE ORIGEM PASSADO POR PARÂMETRO,
    emailDestinatario: // EMAIL DE DESTINO PASSADO POR PARÂMETRO
}
```

Depois, retornar o objeto a seguir:

```js
{
    mensagem: "Email enviado com sucesso",
    status: "Enviado"
}
```

Caso os valores não sejam válidos, deverá ser retornado o seguinte objeto:

```js
{
    mensagem: "Email não enviado. Verifique se há dados inválidos e/ou faltantes",
    status: "Não enviado"
}
```
