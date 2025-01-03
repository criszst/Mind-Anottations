A complexidade O(n²) é conhecida como **complexidade quadrática**. Esse tipo de complexidade aparece em algoritmos onde precisamos realizar operações para cada combinação de elementos em uma coleção, o que normalmente envolve **dois laços aninhados** que iteram sobre o mesmo conjunto de dados.


## **EXEMPLO O(n)**
Quando temos uma constante e queremos iterar sobre ela, fazemos um for. - o que caracteriza a complexidade de tempo como [O(n)](Programming%20Concepts/Big%20O%20Notation/Theory/O(n).md), ou seja, linear: 

```c sharp
// Complexidade O(n)
public static void OpLinear(int n) 
{
	for (int i = 0; i < n; i++) 
	{
		Console.WriteLine($"Complexidade Linear O(n): {i}");
	}
}
```


## **EXEMPLO QUADRÁTICO**
Caso precisamos iterar 2 vezes essa constante, o laço for se torna com uma complexidade quadrática - O(n ^2):

```c sharp
// Complexidade O(n^2)

public static void BigQuadratic(int n)
{
	for (int x = 0; x < n; x++)
	{
		for (int y = 0; y < n; i++)
		{
			Console.WriteLine($"Complexidade quadrática: {x} - {y}");
		}
	}
}
```

No exemplo da complexidade quadrática, temos dois laços `for` aninhados, ambos iterando `n` vezes. Assim, como cada laço interno executa `n` operações para cada iteração do laço externo, o total de operações é:
*n × n = n²*. 

Portanto, se o parâmetro `n` da função *BigQuadratic* fosse igual a 2, ela nos retornaria 4 mensagens no console, pois *2² = 4* :

![](../../../Images/Programming%20Concepts/Big%20O%20Notation/Pasted%20image%2020241113215338.png)



## **AUMENTANDO A COMPLEXIDADE**
Se quiséssemos - *por algum motivo desconhecido* - piorar a complexidade, bastávamos adicionar mais laços for e iterando cada vez mais. Por exemplo, para uma complexidade cúbica, teríamos que adicionar 3 for:

```c sharp
public static void BigCubic(int n) 
{
	for (int i = 0; i < n; i++)
	{
		for (int x = 0; x < n; x++)
		{
			for (int z = 0; z < n; z++)
			{
				Console.WriteLine($"Complexidade cubica: {i} - {x} - {z}");
			}
		}
	}
}
```

 Se o `n` fosse 2, então seria *n * n * n*, ou seja *n³* - o que nos retornaria *8* mensagens de console:
 
![](../../../Images/Programming%20Concepts/Big%20O%20Notation/Pasted%20image%2020241113221256.png)
