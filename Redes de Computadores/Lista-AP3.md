### 1)	Diferencie transmissão Simplex, full-duplex e half-duplex.

> - Simplex é uma transmissão que ocorre em apenas um sentido. Ex: rádio e TV;
> - Half-duplex acontece nos dois sentidos, mas nunca ao mesmo tempo;
> - Full-duplex contece e ambos os sentidos, em frequências diferentes para sentidos direrentes. Ex: VoIP;

### 2)	Diferencie unicast, multicast, anycast e broadcast.

> - Unicast acontece quando uma transmissão é feita a uma máquina específica de um grupo;
> - Multicast acontece quando uma transmissão é feita a várias máquinas de um grupo;
> - Anycast contece quando uma transmissão é feita a uma máquina qualquer do grupo, geralmente a mais próxima;
> - Brodcast acontece quando uma transmissão é feita para todas as máquinas de um grupo;

### 3)	Qual é a diferença entre hubs, switches e roteadores?

Um hub tem várias linhas de entrada que ele conecta eletricamente.
Os quadros que chegam em quaisquer dessas linhas são enviados a todas as outras. Se dois
quadros chegarem ao mesmo tempo, eles colidirão, como ocorre em um cabo coaxial. Em outras
palavras, o hub inteiro forma um único domínio de colisão. Todas as linhas que chegam a um hub
devem operar na mesma velocidade. Os hubs diferem dos repetidores pelo fato de (normalmente)
não amplificarem os sinais de entrada e serem projetados para conter várias placas de linha, cada
uma com várias entradas, mas as diferenças são pequenas. Como os repetidores, os hubs não
examinam o endereços 802 nem os utilizam de forma alguma.

Os switches são semelhantes a pontes pelo fato de ambos basearem o roteamento em endereços
de quadro. Na verdade, muitas pessoas utilizam os dois termos de forma intercambiável. A principal
diferença é que um switch é usado com maior freqüência para conect ar computadores individuais,
como mostra a Figura 4.47(c). Como conseqüência, quando o host A da Figura 4.47(b) quer enviar
um quadro para o host B, a ponte recebe o quadro, mas simplesmente o descarta. Em contraste, na
Figura 4.47(c), o switch deve encaminhar ativamente o quadro de A até B, porque não há outro
caminho que o quadro possa seguir. Tendo em vista que cada porta do switch normalmente se
conecta a um único computador, os swit ches precisam ter espaço para muito mais placas de linha
do que as pontes destinadas a conectar apenas LANs. Cada placa de linha fornece espaço de buffer
para os quadros que chegam a suas portas. Como cada porta é seu próprio domínio de colisão, os
switches nunca perdem quadros devido a colisões. Porém, se os quadros chegarem com velocidade
maior que aquela em que podem ser retransmitidos, o switch poderá ficar sem espaço de buffer e
terá de começar a descartar quadros.

Quando um pacote entra em um roteador, o cabeçalho de quadro
e o final são retirados, e o pacote localizado no campo de carga útil do quadro (sombreado na
Figura 4.46) é repassado ao software de roteamento. Esse software utiliza o cabeçalho de pacote
para escolher uma linha de saída. No caso de um pacote IP, o cabeçalho do pacote conterá um
endereço de 32 bits (IPv4) ou de 128 bits (IPv6), mas não um endereço 802 de 48 bits. O software
de roteamento não vê os endereços de quadro e nem mesmo sabe se o pacote veio de uma LAN ou
de uma linha ponto a ponto.

### 4)	O cabeçalho da camada de enlace é sempre o mesmo ou depende da tecnologia? Qual o tamanho mínimo?



### 5)	O que é um endereço MAC e qual a sua relação com um endereço IP?

6)	Diferencie as topologias em estrela, em barra e em anel, citando vantagens e desvantagens.

7)	Explique para que serve e como funciona o protocolo CSMA/CD.

8)	O que é um domínio de colisão?

9)	Explique porque em cabos de rede metálicos com vários fios estes são agrupados em pares entrelaçados.

10)	Explique uma vantagem e uma desvantagem de cada meio de transmissão a seguir: par-trançado, fibra ótica, rádio, infravermelho, microondas.

11)	Porque a maioria das faixas de frequência é regulamentada por órgãos governamentais e não simplesmente livre para uso?

12)	Qual a importância dos repetidores e amplificadores em enlaces de comunicação?

13)	Diferencie as topologias em estrela, em barra e em anel, citando vantagens e desvantagens.

14)	Ao enviar um pacote para outra máquina, que tipo de consulta ARP é feita quando:
a.	O destino está na mesma rede local?
b.	O destino está em uma rede local diferente?
