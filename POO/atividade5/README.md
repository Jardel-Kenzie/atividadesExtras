## POO

### Class Pessoa

Modele uma classe chamada **Pessoa** que precisa receber como parâmetros no construtor exatamente as seguintes propriedades:

- nome - Formato String
- sobrenome - Formato String
- idade - Formato Number

Além dessas propriedades, também receberá duas propriedades que não será passada como parâmetro no construtor, mas será definida como default na classe:

- saldo - Formato Number - Valor inicial: 0
- historico - Formato Array - Valor inicial: Um Array Vazio

Por fim, desenvolva um método chamado **mostrarNomeCompleto**, Esse método deve retorna o nome completo da pessoa, juntando o nome e sobrenome!

### Class Funcionario

Modele uma classe chamada **Funcionario** que será uma extensão de **Pessoa**, contendo essas informações extras:

- cargo - Formato String
- tipo - Formato String (sempre será clt ou pj)
- salario - Formato Number, resultado do método **relatarSalario**, que deverá acionar no constructor

Por fim, crie o método chamado **relatarSalario** que deverá pegar o array de objeto da classe **Empregos** (já predefinida no arquivo), selecionar desse array o valor do salario na qual se encaixa com o **cargo** e o **tipo** de salario do mesmo. E retornar esse valor!
