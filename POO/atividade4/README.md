## POO

### Class Carta

Modele uma classe chamada **Carta** que precisa receber como parâmetros no construtor exatamente as seguintes propriedades:

- remetente - Formato String
- destinatario - Formato String
- endereco - Formato String
- conteudo - Formato String

### Class Correio

Modele uma classe chamada **Correio** que será uma classe estatica, não tendo constructor, na qual terá essas variaveis predefinidas:

- historicoDeCartas - Formato Array - Inicialmente começa como um array vazio

Por fim, crie 2 Métodos para essa classe:

- Todos os métodos recebem uma parâmetro chamado **carta** na qual será um objeto instanciado da classe **Carta**

#### Método validaCarta

Tem como funcionalidade verificar se todas as propriedades (**remetente**, **destinatario**, **endereco**, **conteudo**) tem algum valor, ou seja, são diferentes de **undefined**, na qual retorna **true** se todas tiverem valor e **false** caso alguma propriedade não tenha valor.

#### Método enviarCarta

Tem como funcionalidade adicionar a carta na variavel **historicoDeCartas** caso ela seja uma carta valida. Caso seja possível enviar, adicione essa carta a variavel e retorne: "Carta Enviada com sucesso", caso contrario retornar: "Carta não enviada, possivelmente tem algum dado invalido/faltante"
