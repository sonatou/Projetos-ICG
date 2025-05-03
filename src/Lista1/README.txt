Exercicios da lista 1 

	o exercício 7 ficou dividido em vários arquivos pois foi a maneira mais fácil q	achei de fazer
	o exercício 10 eu não fui capaz de completar. :(


Exercícios teóricos da lista 1

	1- O que é a GLSL? Quais os dois tipos de shaders são obrigatórios no pipeline programável da versão atual que trabalhamos em aula e o que eles processam? 

	GLSL é a linguagem de programação utilizada para escrever shaders na OpenGL, ela é baseada em C e permite programar a GPU diretamente, controlando como os vértices e fragmentos são processados.

na versão moderna da OpenGL vista em aula, os dois tipos de shaders obrigatórios são

vertex shader:
responsável por processar cada vértice individualmente, ele transforma as posições dos vértices e pode calcular outras informações como normais e coordenadas de textura.

fragment shader:
Responsável por processar cada fragmento, ele define a cor final de cada pixel, podendo aplicar efeitos de luz, texturas, transparência.


	2- O que são primitivas gráficas? Como armazenamos os vértices na OpenGL?
Primitivas gráficas são os elementos básicos usados para desenhar objetos na tela.

Pontos GL_POINTS

Linhas GL_LINES

Triângulos GL_TRIANGLES

Na OpenGL moderna, os vértices são armazenados em buffers na GPU usando:

VBO: armazena os dados dos vértices.

Esses dados são organizados e acessados com ajuda de um VAO.


	3- Explique o que é VBO e VAO, e como se relacionam (se achar mais fácil, pode fazer um gráfico
representando a relação entre eles).

VBO (Vertex Buffer Object):
Um buffer na GPU que contém os dados dos vértices armazena posições, cores, normais, coordenadas de textura.

VAO (Vertex Array Object):
Um objeto que organiza e guarda o estado das configurações dos VBOs define como os dados no VBO devem ser interpretados.


	4- Como são feitas as chamadas de desenho na OpenGL? Para que servem as primitivas de desenho?
São feitas com funções do tipo glDrawArrays(GL_TRIANGLES, 0, 3); e glDrawElements(GL_TRIANGLES, indexCount, GL_UNSIGNED_INT, 0);
As primitivas de desenho servem para indicar como a GPU deve interpretar os vértices.






