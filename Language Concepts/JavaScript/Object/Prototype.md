# **O QUE É?**
Prototype (Protótipo) são o mecanismo pelo qual objetos JavaScript herdam recursos uns dos outros.
Em si, é parecido com a herança de outras linguagens

# **EXEMPLOS**
Por exemplo, se eu quero adicionar um novo método em um array que retorna o último elemento dele, usamos o prototype:

```js
Array.prototype.last = function() {
	return this[this.length - 1];
}

[1, 2, 3, 4, 5].last(); // retorna 5
```