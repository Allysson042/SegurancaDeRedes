Universidade Federal do ![](Aspose.Words.875a1119-1374-4a0a-bd71-a7167ed5eb5a.001.png)

Agreste de Pernambuco 

Av. Bom Pastor s/n - Boa Vista 

55292-270 Garanhuns/PE 

` `+55 (87) 3764-5500 

` `http://www.ufape.edu.br 

|<p>Bacharelado em Ciência da Computação </p><p>CCMP3079 Segurança de Redes de Computadores </p><p>Prof. Sérgio Mendonça </p><p>Atividade Cap. 09 </p><p>Para 18/12/2023</p>|
| :-: |


Nome Completo: Allysson Guimarães dos Santos Silva

Questões retiradas do livro-texto da disciplina. 

Conforme conversamos em sala de aula, as atividades devem ser realizadas para apresentação e discussão em sala, sempre nas aulas das quintas-feiras, atribuindo ao estudante uma nota de 0 ou 1 por cada atividade realizada e apresentada. 

**1. Quais são os principais elementos de um criptossistema de chave pública?** 

Texto claro: essa é a mensagem ou dados legíveis que são alimentados no algoritmo como entrada. 

Algoritmo de encriptação: realiza várias transformações no texto claro. 

Chaves pública e privada: esse é um par de chaves que foi selecionado de modo que, se uma for usada para encriptação, a outra é usada para decriptação. As transformações exatas realizadas pelo algoritmo dependem da chave pública ou privada que é fornecida como entrada. 

Texto cifrado: essa é a mensagem embaralhada produzida como saída. Ela depende do texto claro e da chave. Para determinada mensagem, duas chaves diferentes produzirão dois textos cifrados diferentes. 

Algoritmo de decriptação: aceita o texto cifrado e a chave correspondente e produz o texto claro original.

**2. Quais são os papéis da chave pública e da privada? Descreva-os com detalhes e com exemplos.** 

A chave pública é usada para criptografar dados. Quando alguém deseja enviar informações confidenciais para outra pessoa de forma segura, ele usa a chave pública do destinatário para criptografar os dados. A chave privada é usada para descriptografar os dados que foram criptografados com a chave pública correspondente. Somente o dono da chave privada deve ser capaz de realizar essa operação, garantindo a confidencialidade dos dados.

**3. Quais requisitos os criptossistemas de chave pública precisam cumprir para serem considerados como um algoritmo seguro?** 

É computacionalmente fácil para uma parte B gerar um par (chave pública PUb, chave privada PRb).

É computacionalmente fácil que um emissor A, conhecendo a chave pública e a mensagem a ser encriptada, M, gere o texto cifrado correspondente:

C = E(PUb, M)

É computacionalmente fácil que o receptor B decripte o texto cifrado resultante usando a chave privada para recuperar a mensagem original:

M = D(PRb, C) = D[PRb, E(PUb, M)]

É computacionalmente inviável que um invasor, conhecendo a chave pública, PUb, determine a chave privada, PRb. É computacionalmente inviável que um invasor, conhecendo a chave pública, PUb, e um texto cifrado, C, recupere a mensagem original, M.

**4. Descreva, em termos gerais, um procedimento eficiente para se escolher um número primo.** 

No momento, não existem técnicas úteis que geram números primos de qualquer tamanho, de modo que é preciso que haja algum outro meio de resolver o problema. O procedimento geralmente usado é escolher um número ímpar aleatório da ordem de grandeza desejada e testar se ele é primo. Se não, é escolhido números aleatórios sucessivos até que seja encontrado um primo. Porém, existem algoritmos que podem auxiliar na predição de números primos. Um dos algoritmos mais eficientes e populares, o Miller-Rabin segue os seguintes passos:

Escolha um inteiro ímpar n aleatoriamente (por exemplo, usando um gerador de número pseudoaleatório). Escolha um inteiro a < n aleatoriamente. Realize o teste probabilístico de números primos, como Miller-Rabin, usando a como parâmetro. Se n falhar no teste, rejeite o valor dele e vá para a etapa 1. Se n tiver passado por um número de testes suficiente, aceite-o; caso contrário, vá para a etapa 2.

<b>5. Antes da descoberta de quaisquer esquemas de chave pública específicas, como RSA, uma prova de existência foi desenvolvida, cuja finalidade era demonstrar que a encriptação de chave pública é possível em teoria. Considere as funções <i>f</i><sub>1</sub>(<i>x</i><sub>1</sub>) = <i>z</i><sub>1</sub>; <i>f</i><sub>2</sub>(<i>x</i><sub>2</sub><i>, y</i><sub>2</sub>) = <i>z</i><sub>2</sub>; <i>f</i><sub>3</sub>(<i>x</i><sub>3</sub><i>, y</i><sub>3</sub>) = <i>z</i><sub>3</sub>, onde todos os valores são inteiros com 1 <i>≤ x<sub>i</sub>, y<sub>i</sub>, z<sub>i</sub> ≤ N</i>. A função <i>f</i><sub>1</sub>, pode ser representada por um vetor M1 de tamanho <i>N</i>, em que a <i>k</i>-ésima entrada é o valor de <i>f</i><sub>1</sub>(<i>k</i>). De modo semelhante, <i>f</i><sub>2</sub> e <i>f</i><sub>3</sub> podem ser representados pelas matrizes M2 e M3 de tamanho <i>N × N</i>. A intenção é indicar o processo de encriptação/decriptação por pesquisas de tabela para aquelas com valores muito grandes de <i>N</i>. Essas tabelas seriam impraticavelmente grandes, mas, a princípio, poderiam ser construídas. O esquema funciona da seguinte forma: construa M1 com uma permutação aleatória de todos os inteiros entre 1 e <i>N</i>; ou seja, cada inteiro aparece exatamente uma vez em M1. Construa M2, de modo que cada linha contenha uma permutação aleatória dos primeiros <i>N</i> inteiros. Finalmente, preencha M3 para satisfazer a seguinte condição:</b> 

<b><i>f</i><sub>3</sub>(<i>f</i><sub>2</sub>(<i>f</i><sub>1</sub>(<i>k</i>)<i>, p</i>)<i>, k</i>) = <i>p</i> para todo <i>k, p</i> com 1 <i>≤ k, p ≤ N</i></b> 

**Resumindo,** 

**1. M1 toma uma entrada *k* e produz uma saída *x*.** 

**2. M2 toma as entradas *x* e *p*, dando a saída *z*.** 

**3. M3 toma as entradas *z* e *k* e produz *p*.** 

**As três tabelas, uma vez construídas, se tornam públicas.** 

**a) Deverá ficar claro que é possível construir M3 para satisfazer a condição anterior. Como um exemplo, preencha M3 para o caso simples a seguir:** 

**M1 =** 

<b> <sup></sup></b> 

**5 4 3 2 1** 

**** 

<b><sup></sup><sub></sub>M2 =</b> 

<b> <sup></sup></b> 

**5 2 3 4 1 4 2 5 1 3 1 3 2 4 5 3 1 4 2 5 2 5 3 4 1** 

**** 

<b><sup></sup><sub></sub>M3 =</b> 

**** 

<b><i>a</i><sub>1</sub> <i>a</i><sub>2</sub> <i>a</i><sub>3</sub> <i>a</i><sub>4</sub> <i>a</i><sub>5</sub> <sup></sup></b> 

<b><i>b</i><sub>1</sub> <i>b</i><sub>2</sub> <i>b</i><sub>3</sub> <i>b</i><sub>4</sub> <i>b</i><sub>5</sub> <i>c</i><sub>1</sub> <i>c</i><sub>2</sub> <i>c</i><sub>3</sub> <i>c</i><sub>4</sub> <i>c</i><sub>5</sub> <i>d</i><sub>1</sub> <i>d</i><sub>2</sub> <i>d</i><sub>3</sub> <i>d</i><sub>4</sub> <i>d</i><sub>5</sub> <i>e</i><sub>1</sub> <i>e</i><sub>2</sub> <i>e</i><sub>3</sub> <i>e</i><sub>4</sub> <i>e</i><sub>5</sub></b> 

<b> <sup></sup></b> 

**Convenção: o *i*-ésimo elemento de M1 corresponde a *k* = *i*. A *i*-ésima linha de M2 diz respeito *ax* = *i*; a *j*-ésima coluna de M2 equivale a *p* = *j*. A *i*-ésima linha de M3 indica *z* = *i*; a *j*-ésima coluna de MB relaciona-se a *k* = *j*.** 

**(a) Descreva o uso desse conjunto de tabelas para realizar a encriptação e decriptação entre dois usuários.** 

**(b) Demonstre que esse é um esquema seguro** 

**6. Realize a encriptação e decriptação usando o algoritmo RSA, como na Figura 9.5, para o seguinte:** 

**(a) *p* = 3; *q* = 11, *e* = 7; *M* = 5;** 

**(b) *p* = 5; *q* = 11, *e* = 3; *M* = 9;** 

**(c) *p* = 7; *q* = 11, *e* = 17; *M* = 8;** 

**(d) *p* = 11; *q* = 13, *e* = 11; *M* = 7;** 

**(e) *p* = 17; *q* = 31, *e* = 7; *M* = 2.** 

**Dica: a decriptação não é tão difícil quanto você pensa; use alguma sutileza.** 


**7. Em um sistema de chave pública usando RSA, você intercepta o texto cifrado *C* = 10 enviado a um usuário cuja chave pública é *e* = 5, *n* = 35. Qual é o texto claro *M*?** 

def decrypt\_public(c, chave\_publica):

`    `M = pow(c, chave\_publica.e, chave\_publica.n) #m = c^e mod n

`    `print("M = {0}".format(M))



`    `return M

chave\_publica = Chave\_publica(5, 35)

M = decrypt\_public(C, chave\_publica)

