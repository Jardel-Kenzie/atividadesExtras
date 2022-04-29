### Class Lutador

Modele uma classe chamada **Lutador**, ela recebe como parâmetros do construtor, os seguintes elementos:

* nome - Tipo String
* category - Tipo String
* forca - Tipo Number
* defesa - Tipo Number

Além disso, ela também precisará ter a propriedade que terá um valor padrão.

* vitorias - Tipo Number - que começa com o valor 0.

### Class Arena

Modele uma classe chamada **Arena**, que tem uma propriedade estatica chamada **contadorDeBatalhas** e um método estático chamado **batalha**, que receberá por parâmetro:

* lutador1- Instância da classe Lutador tendo todos os os atributos dela.
* lutador2 - Instância da classe Lutador tendo todos os os atributos dela.

Esse método deverá validar se a força de um lutador é maior que a defesa do outro. Caso seja maior, acrescente uma vitória ao lutador vencedor e retorne uma mensagem, da seguinte forma:
```javaScript
{
	menssagem: LUTADOR venceu LUTADOR,
	vitoriasGanhador: NUMERO DE VITORIAS DE QUEM GANHOU,
	numeroDaBatalha: NUMERO QUE CONTA AS BATALHAS,
}
```