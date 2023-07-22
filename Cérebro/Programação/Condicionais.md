
- **Definição**: Condicionais são estruturas de controle que permitem tomar decisões no código com base em condições.
- **Estrutura**: Usamos "if", "elif" (opcional) e "else" (opcional) para criar condicionais.
  <br>
	1. **if** = O "if" é a primeira estrutura a ser avaliada. Ele verifica se uma condição é verdadeira e executa o bloco de código associado somente se a condição for verdadeira.
	2. **elif** = O "elif" é uma abreviação de "else if" e é usado para testar condições adicionais, caso a condição do "if" não seja atendida. Podemos ter vários "elif" para verificar condições diferentes.
	3. **else** = O "else" é executado somente se nenhuma das condições do "if" e "elif" forem atendidas. É uma espécie de "caso contrário".
<br>

- **Importância**: Permitem executar diferentes ações com base em situações específicas.
- **Comparação**: Comparamos valores usando operadores como ">", "<", ">=", "<=", "==", "!=".
- **Indentação**: Blocos de código dentro de condicionais devem ser identados para indicar sua pertinência.
<br>
- **Exemplo**:

 idade = 18 
 if idade >= 18: 
	print("Você é maior de idade.") 
 else:  	
	 print("Você é menor de idade.")