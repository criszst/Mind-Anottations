Um objeto literal é uma estrutura de dados usado para armazenar coleções de dados. Em resumo, um objeto literal é uma forma de criar objetos de maneira direta e concisa.


Um objeto literal é representado por chaves `{}` e contém pares de chave valor, onde a chave é um identificador e o valor pode ser qualquer dado, como uma string, número, função ou outro objeto.

Em resumo, os objeto literais são fundamentais na manipulação de dados em JS, especialmente ao trabalhar com APIS ou gerenciar o estado de uma aplicação.

# Sintaxe
Em relação a sintaxe, é necessário colocar as propriedades e os métodos dentro de um par de chaves `{}`, separados por virgulas:

```javascript
const car = {
	name: 'Gol GTI',
	year: 2023,
	cv: 145,
}
```

Nesse exemplo, **car** é um objeto literal que contém 3 propriedades - nome, ano do modelo e cv (cavalos de potência), cada uma contendo o seu respectivo valor.

### Objeto literal com funções

Além disso, é possível criar objetos literais que contém funções:

```js
const Person = {
	name: 'Cristian',
	age: 16,
	hobby: 'Programming',
	greet: function() {
		console.log(`Hello World, meu nome é ${this.name}`)
	}
};

console.log(Person.greet())
// Hello World, meu nome é Cristian
```


### Estrutura mais complexa:

```js
const Person = {
	name: 'Cristian',
	age: 16,
	hobby: 'Programming',
	musicGenreFavs: {
		best: 'Rock',
	}
}

console.log(Person.musicGenreFavs.best)
// 'Rock'
```

