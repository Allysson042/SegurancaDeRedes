<img src = header2.JPG>


Nome Completo: Allysson Guimarães

Questões retiradas do livro-texto da disciplina. 

1\. Responda (de forma objetiva) as questões a seguir: 

(a) Quais são os elementos essenciais de uma cifra simétrica? 

**Chave e algoritmo de cifragem/decifragem.**

(b) Quais são as duas funções básicas usadas nos algoritmos de encriptação? 

` 		`**Cifragem e decifragem.**

(c) Qual é a diferença entre uma cifra de bloco e uma cifra de fluxo? 

**A forma como operam, cifras de bloco operam sobre blocos fixos de dados, geralmente de tamanho fixo, e cifra cada bloco separadamente. Como AES e DES.**

**Cifras de fluxo operam sobre os dados de forma contínua, normalmente um bit ou byte por vez, e gera um fluxo contínuo de dados cifrados. Como RC4 e  A5/1.**

(d) Quais são as duas técnicas gerais para atacar uma cifra? 

`		`**Força bruta e criptoanalíticos.**

(e) Quais são os dois problemas com o one-time pad? 

`		`**Necessidade de chaves longas e aleatórias, proibição da reutilização da chave.**

(f) O que é uma cifra de transposição? 

`		`**Reorganiza símbolos na mensagem sem substituí-los.**

(g) O que é esteganografia? 

`		`**Ocultar informações secretas dentro de outras informações para tornar a existência da mensagem secreta imperceptível.**


2\. Uma generalização da cifra de César, conhecida como cifra de César afim, tem a seguinte forma: a cada letra de texto claro *p*, substitua-a pela letra de texto cifrado *C* : 

*C* = *E*([*a, b*]*, p*) = (*ap* + *b*) mod 26 

um requisito básico de qualquer algoritmo de encriptação é que ele seja um para um. Ou seja, se *p ̸*= *q*, então *E*(*k, p*) *̸*= *E*(*k, q*). Caso contrário, a decriptação é impossível, pois mais de um caractere de texto claro é mapeado no mesmo caractere de texto cifrado. A cifra de César afim não é um-para-um para todos os valores de *a*. Por exemplo, para *a* = 2 e *b* = 3, então *E*([*a, b*]*,* 0) = *E*([*a, b*]*,* 13) = 3. 

(a) Existem limitações sobre o valor de b? explique por que sim ou por que não. 

(b) determine quais valores de a não são permitidos. 

(c) ofereça uma afirmação geral sobre quais valores de a são e não são permitidos. Justifique-a. 





3\. (a) Encripte a mensagem “meet me at the usual place at ten rather than eight oclock” usando 

a cifra de Hill com a chave 
</sup>
` `9 4

5 7



. Mostre seus cálculos e o resultado. 

(b) Mostre os cálculos para a decriptação correspondente do texto cifrado a fim de recuperar o texto claro original. 



4\. Elabore um programa que possa encriptar e decriptar usando a cifra de César geral, também conhecida como cifra aditiva. 

[**Código** ](https://colab.research.google.com/drive/1yP6295UdkPHSHm_QY5GbyVSSe7ox8KLj?usp=sharing)



5\. Elabore um programa que possa realizar um ataque de frequência de letra em uma cifra aditiva sem intervenção humana. Seu software deverá produzir textos claros possíveis em ordem aproximada de probabilidade. Seria bom se a sua interface com o usuário permitisse que ele especificasse “mostre os 10 textos claros mais prováveis”. 



6\. Crie um software que possa encriptar e decriptar usando uma cifra de Hill 2 *×* 2. 

