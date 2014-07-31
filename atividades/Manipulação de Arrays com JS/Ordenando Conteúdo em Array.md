Ordernando Conteúdo
===================
Parágrafo
---------
```html
	<p class="names">Luke Yoda Skywalker Leia Chewbacca Padmé</p>
```

Código
------
- Seleciona o parágrafo via class
```js
	var names = document.querySelector('.names');
```
- Seleciona o conteúdo do parágrafo
```js
	var content = names.innerHTML;
```
- Corta o parágrafo transformando em array
```js
	content = content.split(" ");
```
- Coloca o array em ordem alfabática
```js
	content.sort();
```
- Zera o Parágrafo
```js
	names.innerHTML = "";
```
- Insere o conteúdo do array no parágrafo em ordem alfabética e por linha
```js
	for(var i = 0; i<content.length; i++){
    	names.innerHTML += content[i]+"<br />";
	}
```
- Resultado:
<a href="http://jsfiddle.net/taotiago/zyELz/">Resultado</a>
- Código Completo
```js
	var names = document.querySelector('.names');
	var content = names.innerHTML;
	content = content.split(" ");
	content.sort();
	names.innerHTML = "";
	for(var i = 0; i<content.length; i++){
	    names.innerHTML += content[i]+"<br />";
	}
```