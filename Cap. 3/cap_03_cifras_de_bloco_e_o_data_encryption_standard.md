<img src=header3.JPG>


Nome Completo: Allysson Guimarães

Questões retiradas do livro-texto da disciplina. 

1\. Responda os questionamentos a seguir: 

(a) Por que é importante estudar a cifra de Feistel? 

**Por se tratar de um modelo fundamental na criptografia, ele oferece uma estrutura eficiente e segura para a construção de algoritmos de cifragem.**

(b) Qual é a diferença entre uma cifra de bloco e uma cifra de fluxo?

**Uma cifra de bloco criptografa dados em blocos fixos, enquanto uma cifra de fluxo opera em bits individuais.**



(c) Por que não é prático usar uma cifra de substituição reversível qualquer do tipo mostrado na Tabela 3.1? 

**São inseguras, pois, elas não conseguem ocultar padrões e relações estatísticas nos dados originais**

(d) O que é uma cifra de produto? 

**É a combinação de duas ou mais cifras independentes para aumentar a segurança.**

(e) Qual é a diferença entre difusão e confusão? 

**Difusão consiste em espalhar e distribuir a influência de um dado de entrada por todo o resultado da cifragem.**

**Confusão, por outro lado, envolve tornar a relação entre a chave e o texto cifrado o mais complexa possível**

(f) Que parâmetros e escolhas de projeto determinam o algoritmo real de uma cifra de Feistel? 

**O número de rodadas, tamanho dos blocos de dados, chave, dentre outros.**

(g) Explique o efeito avalanche. 

**Consiste em realizar uma pequena alteração nos dados de entrada ou na chave que resulta em mudanças significativas nos dados de saída.**

2\. Qual(is) dos recursos abaixo estão presentes no projeto da rede de Feistel? Explique. 

(a) Tamanho do bloco e da chave; 

(b) Função da rodada; 

(c) Gerador de sub-chaves; 

(d) Todas as alternativas. 

**Todas as alternativas. O tamanho do bloco determina o tamanho dos dados de entrada e saída de cada rodada, enquanto o tamanho da chave influencia a complexidade e a segurança do algoritmo. A função de rodada é responsável por realizar operações de substituição e permutação nos dados em cada rodada. A geração adequada de sub-chaves é crucial para a segurança da cifra de Feistel.**

3\. Qual é o tamanho do texto claro no Data Encryption Standard (DES)? Explique. (a) 57; 

(b) 48; 

(c) 32; 

(d) 64. 

**O DES opera em blocos de 64 bits de dados de entrada, que são divididos em blocos menores durante o processo de cifragem.**



4\. A cifra de Feistel do algoritmo de encriptação utilizada no Data Encryption Standard (DES) utiliza quantos S-boxes? Explique. 

(a) 8; 

(b) 7; 

(c) 6; 

(d) 5. 

` `**DES utiliza 8 S-boxes. Os S-boxes são tabelas de substituição usadas para realizar operações de substituição nos dados em cada rodada do DES.** 

5\. O Data Encryption Standard possui uma chave de 56 bits, o que torna possível um espaço de 2<sup>56</sup> chaves possíveis. Essa sentença trata de ataque de. . . Explique. 

(a) Tempo; 

(b) Matemático; 

(c) Força-Bruta; 

(d) DoS. 

**Força-Bruta.**

6\. Demonstre, através de um exemplo, como realizar a cifragem de 16 bits (dois caracteres), em 2 rounds, em seguida, decifre o texto cifrado. Explique o processo passo a passo. Forneça um código Python/Sagemath com sua solução. 

7\. Considere uma cifra de Feistel composta de 16 rodadas com tamanho de bloco de 128 bits e tamanho de chave de 128 bits. Suponha que, para determinado *k*, o algoritmo de escalonamento de chave defina valores as oito primeiras chaves de rodada, *k*<sub>1</sub>*, k*<sub>2</sub>*, . . . , k*<sub>8</sub>, e depois estabeleça 

*k*<sub>9</sub> = *k*<sub>8</sub>*, k*<sub>10</sub> = *k*<sub>7</sub>*, k*<sub>11</sub> = *k*<sub>6</sub>*, . . . , k*<sub>16</sub> = *k*<sub>1</sub> 

Admita que você tenha um texto cifrado *S*. Explique como, com acesso a um oráculo de en criptação, você pode decriptar *c* e determinar *m* usando apenas uma única consulta a ele. Isso mostra que tal cifra é vulnerável a um ataque de texto claro escolhido. (Um oráculo de en criptação pode ser imaginado como um dispositivo que, dado um texto claro, retorna o texto cifrado correspondente. Os detalhes internos do dispositivo não são conhecidos, e você não pode abri-lo. Você só consegue obter informações do oráculo fazendo consultas a ele e observando suas respostas.) 

Livro-texto da disciplina: 

