
### 1)	Cite e explique os cinco serviços da camada de rede.

> - Encapsulamento: Enviar pacotes dentro de pacotes IP para poderem ser transportados independentemente da sua
> - Roteamento: Capacidade de __repassar__ pacotes e de criar rotas para enviar um pacote de um endereço a outro
> - Fragmentação: Capacidade de separar pacotes grandes demais para serem transportados pelo enlace de uma vez só e reunir seus fragmentos ao chegar ao destino.
> - Internetworking/Interconexão: Capacidade de 
> - Endereçamento: Cada host possui um endereço para que possa receber e enviar pacotes e ser encontrado pelos demais nós da rede;

### 2)	Qual a diferença entre roteamento intra-AS e roteamento inter-AS?

> - **Intra-AS** ocorre dentro de um AS, com suas próprias regras e protocolos, muitas vezes priorizando o desempenho sobre as regras.
> - **Inter-AS** ocorre entre ASses através dos roteadores de borda, através do protocolo BGP, priorizando criar uma linguagem única que permita a comunicação corretamente e leve em consideração regras e políticas das ASses

### 3)	Quais as características de um protocolo de roteamento por “estado do enlace” (link state)?

> **LINK STATE** : 
> 
> - Informação global: todos os roteadores se comunicam com todos os roteadores para cosntruir uma base de dados de conexões e um mapa de topologia de rede que será comum a todos os roteadores;
> - Melhores rotas para os dados: Cada roteador utilza o mapa topológico da rede para calcular as rotas dos dados que mais lhe beneficiem;
> - Escalabilidade quase impossível, considerando que **todos** os roteadores se comunicam com **todos** os roteadores;
> - a complexidade da implementação do algoritmo de estado de enlace para o pior caso é de ordem n ao quadrado: O(n^2);
>  https://www.youtube.com/watch?v=rLYpzzRYRNk

### 4)	Quais as características de um protocolo de roteamento por vetor de distância?

> Informação centralizada: Cada roteador possui uma tabela de rotas própria que envia aos seus vizinhos periodicamente. Os vizinhos agregam às próprias tabelas o que lhes interessar e repassam a própria tabela para os vizinhos periodicamente e assim por diante;
> Ocorre por FLOOD (inundação);
> Roteador recebe informações dos vizinhos assim que entra na rede;
> https://www.youtube.com/watch?v=8SQLVMJJ5T4

### 5)	Quais as diferenças entre o RIPv1 e o RIPv2?

### 6)	Por que existe o OSPF hierárquico? Explique como funciona, suas vantagens e desvantagens.

### 7)	Como é possível que dois pacotes enviados por uma mesma máquina e para o mesmo destino cheguem em ordem diferente da ordem de envio? Explique.

> - Mudanças de roteamento, caminhos diferentes
> - Fragmentação

### 8)	Como funciona o programa “traceroute”?

> Explicando de uma maneira simples, o comando tracert verifica o tempo de acesso a um determinado IP de um servidor.
> Para isso, ele usa valores de tempo de vida útil, conhecidos como TTL (Time To Live). O TTL é a quantidade de saltos entre dispositivos dados por um pacote até o destino.
> Ao longo do caminho percorrido pelo pacote, cada roteador decrementa o pacote em no mínimo 1 antes de encaminhá-lo.
> Quando o TTL atinge o valor zero, o computador de origem recebe do roteador uma mensagem de tempo excedido, indicando o descarte do pacote.
> O comando tracert mostrará uma lista de roteadores intermediários que devolvem essas mensagens de tempo excedido. Com isso, é possível identificar onde esse descarte de pacote está ocorrendo.
> a
> Para perceber o que é de fato o atraso em uma rede de computadores, podemos utilizar o Traceroute, programa de diagnóstico que pode ser executado em qualquer hospedeiro da Internet. Quando o usuário especifica um nome de hospedeiro de destino, o programa no hospedeiro de origem envia vários pacotes especiais em direção àquele destino. Ao seguir seu caminho até o destino, esses pacotes passam por uma série de roteadores. Um deles recebe um desses pacotes especiais e envia à origem uma curta mensagem, contendo o nome e o endereço do roteador. 
> Mais especificamente, suponha que haja N – 1 roteadores entre a origem e o destino. Então, a fonte enviará N pacotes especiais à rede e cada um deles estará endereçado ao destino final. Esses N pacotes especiais serão marcados de 1 a N, sendo a marca do primeiro pacote 1 e a do último, N. Assim que o enésimo roteador recebe o enésimo pacote com a marca n, não envia o pacote a seu destino, mas uma mensagem à origem. Quando o hospedeiro de destino recebe o pacote N, também envia uma mensagem à origem, que registra o tempo transcorrido entre o envio de um pacote e o recebimento da mensagem de retorno correspondente. A origem registra também 
o nome e o endereço do roteador (ou do hospedeiro de destino) que retorna a mensagem. Dessa maneira, a origem pode reconstruir a rota tomada pelos pacotes que vão da origem ao destino e pode determinar os atrasos de ida e volta para todos os roteadores intervenientes. Na realidade, o programa Traceroute repete o processo que  acabamos de descrever três vezes, de modo que a fonte envia, na verdade, 3 N pacotes ao destino. O RFC 1393 descreve detalhadamente o Traceroute.

### 9)	Explique rede, sub-rede e super-rede e máscara de rede.

> - **REDE:** Uma faixa de endereços vizinhos que se conectam (vizinhos);
> - **SUB-REDE:** Partes separadas desta faixa de endereços;
> - **SUPER-REDE:** Quando duas ou mais faixas se conectam;

### 10)	Diferencie unicast, multicast, anycast e broadcast.

> - Unicast: Transmissão feita por um emissor, destinada a apenas um receptor na rede;
> - Multicast: Transmissão feita de um emissor para vários receptores na rede (não necessariamente todos);
> - Anycast: Transmissão feita de um emissor para o endereço mais próximo de um grupo de receptores na rede;
> - Broadcast (difusão): É a transmissão feita de um emissor para todos os receptores da rede.

### 11)	Como o Network Address Translation (NAT) funciona?

### 12)	Quais as vantagens do IPv6? Ele é realmente necessário?

### 13)	A qual classe pertencem os seguintes IPs:
a.	11101100111011001111111110110000

b.	11111100111011001111111000101000

c.	01101100111011001111011110110000

d.	11001100111011001111111011110010

e.	10.0.0.1 **A**

f.	128.0.10.1 **B**

g.	241.0.0.5 **C**

### 14)	Quais são o ip de “rede”, o ip de broadcast e máscara das seguintes redes?
a.	10.5.4.3/14

b.	192.168.168.192/27

c.	200.129.38.0/23

### 15)	Quantos computadores podem ser ligados à rede 200.129.36.0/22?



### 16)	Diga se as afirmações são VERDADEIRAS ou FALSAS, justificando sua resposta caso seja falsa.
a.	No roteamento vetor distância, se cada nó no domínio tem toda a topologia do domínio — lista dos nós e enlaces, que, interligados, incluem tipo, custo e condição dos enlaces —, o nó poderá usar o algoritmo de Dijkstra para construir a tabela de roteamento.

> **FALSO**. Isto se trataria do roteamento por estado de enlace;

b.	Tanto no protocolo de roteamento OSPF quanto no RIP, a rota que um pacote de dados faz é sempre a mesma, já que os roteadores não percebem que há mais de um caminho para atingir o destino.

> **FALSO** O protocolo OSPF utiliza o protocolo de roteamento link state e é capaz de recalcular rotas;

c.	Uma das desvantagens do protocolo RIPv1 é que ele define o caminho para atingir as redes com base na distância (em saltos) que é necessária para chegar até elas, não levando em conta o desempenho da rota.

d.	A Internet é formada por um elevado número de redes independentes ou sistemas autônomos (AS). Para interligar vários AS, é mais adequado utilizar o protocolo OSPF que o RIP, tendo em vista que o OSPF opera diretamente nos roteadores de borda de área.

> **FALSO** a comunicação inter-AS é feita através do protocolo BGP, que é global para todos os roteadores de borda;

e.	Dois roteadores que pertençam à mesma área irão conter bases de dados de estado de enlace distintas, pois cada roteador executa o seu próprio processo OSPF.

> **FALSO** a base de dados de enlace é a mesma, PORÉM, cada nó da rede realiza um cálculo distinto para decidir a melhor rota para o envio dos pacotes;

f.	O RIPv1 é embasado no algoritmo Bellman-Ford e opera com desempenho adequado para redes em pequena escala; porém, para redes com um maior número de elementos na camada de rede, o seu desempenho é ruim, se comparado ao tempo de convergência do OSPF.

g.	Um AS (sistema autônomo), ao se comunicar com outro AS, deverá efetuar uma troca de todas suas rotas internas, usando protocolos iGP, que podem ser o OSPF ou RIP, por exemplo.

h.	O protocolo RIP (Routing Information Protocol) utiliza a contagem de enlaces de rede como métrica. Dessa forma, se um pacote precisar passar por N redes para chegar ao seu destino final, o custo total dessa rota será N.

i.	O RIP (Routing Information Protocol) é um protocolo de roteamento que utiliza o algoritmo de roteamento denominado vetor distância.

j.	O OSPF é um protocolo IGP (Interior Gateway Protocol) de estado do enlace desenvolvido para operar em redes TCP/IP e para solucionar as limitações do RIP (Router Information Protocol).

k.	No protocolo OSPF, um roteador se comunica com seus vizinhos por multicast, em vez de broadcast, nos endereços 224.0.0.5 — com todos os roteadores — e 224.0.0.6 — com roteadores designados.

