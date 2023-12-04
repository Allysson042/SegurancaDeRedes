<img src=header5.JPG>


Nome Completo: Allysson Guimarães dos Santos Silva

Questões retiradas do livro-texto da disciplina. 

Conforme conversamos em sala de aula, as atividades devem ser realizadas para apresentação e discussão em sala, sempre nas aulas das quintas-feiras, atribuindo ao estudante uma nota de 0 ou 1 por cada atividade realizada e apresentada. 

1\. Qual foi o conjunto original de critérios usados pelo NIST para avaliar as cifras AES candidatas? 

**O NIST avaliou a segurança teórica, eficiência computacional, flexibilidade, simplicidade do algoritmo, segurança de implementação, análise de blocos e chave, e avaliação pública.**

2\. Qual foi o conjunto final de critérios usados pelo NIST para avaliar as cifras AES candidatas? 

**Segurança da criptográfica, eficiência computacional, simplicidade, flexibilidade, tamanho de bloco e chave, segurança contra ataques conhecidos, análise por pares independentes, e avaliação pública.** 

3\. Qual é a diferença entre Rijndael e AES? 

**Rijndael é o algoritmo de cifragem simétrica, enquanto AES (Advanced Encryption Standard) refere-se à configuração específica do Rijndael escolhida como o padrão de cifragem. AES tem um tamanho de bloco fixo de 128 bits e suporta tamanhos de chave de 128, 192 e 256 bits.**



4\. Responda: 

(a) Qual é a finalidade do array Estado? 

**No algoritmo AES uma matriz 4x4 armazena o estado intermediário durante as operações de cifragem e decifragem. Cada byte na matriz representa um elemento do bloco de dados de 128 bits. As operações do AES manipulam esse array durante o processo para garantir confusão e difusão nos dados, contribuindo para a segurança do algoritmo.**

(b) Como é construída a S-box? 

**A S-box no AES é construída por meio de operações matemáticas, incluindo inverso multiplicativo, permutação afim e aplicação de uma função de substituição não linear. Essas etapas são projetadas para criar uma tabela de substituição resistente a ataques criptoanalíticos, contribuindo para a segurança da cifra AES.**

(c) Descreva rapidamente o estágio SubBytes, ShiftRows, MixColumns, AddRoundKey, e o algoritmo de expansão de chave. 

**SubBytes**

`   `**- Cada byte no array de Estado é substituído por um valor correspondente na S-box.**

`   `**- Isso introduz confusão nos dados, contribuindo para a segurança do algoritmo.**

**ShiftRows**

`   `**- Nesta etapa, as linhas do array de Estado são deslocadas para a esquerda.**

`   `**- O deslocamento varia para cada linha, proporcionando difusão nos dados.**

`   `**- O objetivo é aumentar a dispersão dos bits dentro do bloco.**

**MixColumns**

`   `**- MixColumns é uma operação de mistura de colunas que afeta cada coluna do array de Estado.**

`   `**- Os dados em cada coluna são combinados de maneira linear, proporcionando mais difusão e confusão.**

`   `**- Essa etapa contribui significativamente para a difusão dos bits no bloco de dados.**

**AddRoundKey**

`   `**- Nesta fase, uma subchave derivada da chave principal é combinada com o array de Estado.**

`   `**- Cada byte do array é combinado com o byte correspondente da subchave usando uma operação XOR.**

`   `**- Isso introduz a chave na operação, sendo crucial para a segurança.**

**Algoritmo de Expansão de Chave**

`   `**- O algoritmo de expansão de chave gera as subchaves necessárias para cada rodada do AES.**

`   `**- A partir da chave original, são geradas subchaves através de operações como rotações, substituições e XOR com constantes específicas.**

`   `**- O número de rodadas determina quantas subchaves são geradas, e essas subchaves são utilizadas nas operações AddRoundKey em cada rodada.**

6\. Use a chave 1010 0111 0011 1011 para encriptar o texto claro "ok"conforme expresso em ASCII, ou seja, 0110 1111 0110 1011. Os projetistas do S-AES obtiveram o texto cifrado 0000 0111 0011 1000. E você? 

7\. Compare AES com DES. Para cada um dos seguintes elementos do DES, indique o elemento comparável no AES ou explique por que ele não é necessário no AES. 

(a) XOR do material da subchave com a entrada da função f. 

**O AES também utiliza uma operação semelhante, AddRoundKey, que envolve um XOR entre o array de estado e a subchave da rodada. No entanto, o processo é mais direto no AES, pois cada byte do estado é XOR diretamente com o byte correspondente da subchave.**

(b) XOR da saída da função f com a metade esquerda do bloco. 

**Este passo não é diretamente comparável no AES. No AES, a difusão dos bits é alcançada por meio de operações como SubBytes, ShiftRows e MixColumns, e não há um passo específico equivalente ao XOR mencionado.**

(c) função f. 

**SubBytes e a operação de MixColumns no AES desempenham funções semelhantes à função f do DES. Elas proporcionam confusão e difusão necessárias para a segurança do algoritmo.**

(d) permutação P. 

**O AES não possui uma operação específica equivalente à permutação P do DES. A difusão no AES é alcançada de maneira diferente, principalmente por meio da operação ShiftRows e MixColumns.**

(e) troca de metades do bloco. 

**Esta operação não é necessária no AES, pois o AES utiliza uma estrutura de blocos uniforme e opera diretamente em blocos de dados de tamanho fixo (128 bits). A troca de metades do bloco no DES é usada para misturar os dados entre as duas metades, o que não é uma consideração no AES.**

8\. (1 ponto-extra) Calcule a saída da transformação MixColumns para a seguinte sequência de bytes de entrada "67 89 AB CD". Aplique a transformação InvMixColumns ao resultado obtido para verificar seus cálculos. Altere o primeiro byte da entrada de "67"para "77", rea lize a transformação MixColumns novamente para a nova entrada e determine quantos bits mudaram na saída. 

Nota: você pode realizar todos os cálculos à mão ou escrever um programa que dê suporte a eles. Se escolher escrever um programa, ele deverá ser feito inteiramente por você; nesta tarefa, não use bibliotecas ou código fonte de domínio público (você pode se guiar pelos exemplos Sage disponibilizados). 

9\. (2 pontos-extra) Crie um software que possa encriptar e decriptar usando S-AES. Dados de teste: um texto claro binário de 0110 1111 0110 1011 encriptado com uma chave binária de 1010 0111 0011 1011 deverá dar o texto cifrado binário 0000 0111 0011 1000. A decriptação deverá funcionar da mesma forma. 

Livro-texto da disciplina: 

STALLINGS, William. Criptografia e segurança de redes. Princípios e práticas, Ed. 6. 2014. Pág 2 
