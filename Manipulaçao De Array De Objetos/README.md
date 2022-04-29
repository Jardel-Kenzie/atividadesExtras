## MultArray

Agora iremos trabalhar com um array bem dinâmico, lembrando que essa categoria de array, não cairá no Retake, ele é de uma complexidade bem maior

```javaScript
let objetoComplexo = [
    {nome: 'jardel', cursos:[ 
        {
            javaScirpt: [
                {usabilidade: "Lingugem atual"}, 
                {sobre: "rodar por um tempo"}
            ], 
            html: [ 
                {usabilidade: "Usamos tags no html"}, 
                {sobre: "da para colocar texto"}
            ] 
        }
        ] 
    },

    {nome: 'pedro', cursos:[ 
        {
            python: [
                {usabilidade: "find, desgin parterns"}, 
                {sobre: "acho bem legal :D "}
            ], 
            json: [ 
                {usabilidade: "armazenar valores"}, 
                {sobre: "usamos apenas na base"}
            ] 
        }
        ] 
    },

    {nome: 'maria ferrari', cursos:[ 
        {
            react: [
                {usabilidade: "organiza bem as pastas"}, 
                {sobre: "acho bem bonito"}
            ], 
            uxui: [ 
                {usabilidade: "deixar a página mais acessivel para o user"}, 
                {sobre: "complicadinho hahaha"}
            ] 
        }
        ] 
    }
]
```


### O que fazer agora?

* Tente fazer primeiramente na mão, acessar e verificar os **niveis** desse array, ou seja:
```javaScript
objetoComplexo[0].nome // retornaria para mim jardel
objetoComplexo[0].cursos // retornaria para mim, outro objeto contendo dois cursos(duas chaves), javaScript e HTML que são novamente arrays de objetos
```
agora tente pegar dois valores na mão para mim:

* sobre de uxui
* usabilidade do python
* sobre de javaScript

### Agora vamos tentar com loop?

* tente manipular esses elementos com loops, irei demostrar com for, mas pode usar métodos se quiser

```javaScript
const cursosJardel = ''

for(let index = 0; index < objetoComplexo.length; index++){
    let currentValue = objetoComplexo[index] // aqui ele vai pegar cada um dos usuarios e todos os seus atributos
    // iremos pegar com loop agora irei pegar todos os cursos de jardel
    if(currentValue.nome === "jardel"){ // verifico se pertence a jardel
        cursosJardel = currentValue.cursos
    }
}
```

agora tente você pegar esses valores:

* Cursos da maria
* verificar quem tem o curso chamado uxui e retornar o objeto completo 
* sobre de json


### Agora é com você

Fizemos alguns testes, agora é com você o item é bem grande, que tal brincar um pouco? O que tanto a tecnologia deixa você fazer? E até onde você é permitido ir? Quão dinâmico isso pode ficar? Ou quão na mão poderíamos fazer?
