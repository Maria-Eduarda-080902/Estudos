
### 1)	Cite e explique os cinco serviços da camada de rede.

### 2)	Qual a diferença entre roteamento intra-AS e roteamento inter-AS?

### 3)	Quais as características de um protocolo de roteamento por “estado do enlace” (link state)?

### 4)	Quais as características de um protocolo de roteamento por vetor de distância?

### 5)	Quais as diferenças entre o RIPv1 e o RIPv2?

### 6)	Por que existe o OSPF hierárquico? Explique como funciona, suas vantagens e desvantagens.

### 7)	Como é possível que dois pacotes enviados por uma mesma máquina e para o mesmo destino cheguem em ordem diferente da ordem de envio? Explique.

### 8)	Como funciona o programa “traceroute”?

### 9)	Explique rede, sub-rede e super-rede e máscara de rede.

### 10)	Diferencie unicast, multicast, anycast e broadcast.

### 11)	Como o Network Address Translation (NAT) funciona?

### 12)	Quais as vantagens do IPv6? Ele é realmente necessário?

### 13)	A qual classe pertencem os seguintes IPs:
a.	11101100111011001111111110110000

b.	11111100111011001111111000101000

c.	01101100111011001111011110110000

d.	11001100111011001111111011110010

e.	10.0.0.1

f.	128.0.10.1

g.	241.0.0.5

### 14)	Quais são o ip de “rede”, o ip de broadcast e máscara das seguintes redes?
a.	10.5.4.3/14

b.	192.168.168.192/27

c.	200.129.38.0/23

### 15)	Quantos computadores podem ser ligados à rede 200.129.36.0/22?

### 16)	Diga se as afirmações são VERDADEIRAS ou FALSAS, justificando sua resposta caso seja falsa.
a.	No roteamento vetor distância, se cada nó no domínio tem toda a topologia do domínio — lista dos nós e enlaces, que, interligados, incluem tipo, custo e condição dos enlaces —, o nó poderá usar o algoritmo de Dijkstra para construir a tabela de roteamento.

b.	Tanto no protocolo de roteamento OSPF quanto no RIP, a rota que um pacote de dados faz é sempre a mesma, já que os roteadores não percebem que há mais de um caminho para atingir o destino.

c.	Uma das desvantagens do protocolo RIPv1 é que ele define o caminho para atingir as redes com base na distância (em saltos) que é necessária para chegar até elas, não levando em conta o desempenho da rota.

d.	A Internet é formada por um elevado número de redes independentes ou sistemas autônomos (AS). Para interligar vários AS, é mais adequado utilizar o protocolo OSPF que o RIP, tendo em vista que o OSPF opera diretamente nos roteadores de borda de área.

e.	Dois roteadores que pertençam à mesma área irão conter bases de dados de estado de enlace distintas, pois cada roteador executa o seu próprio processo OSPF.

f.	O RIPv1 é embasado no algoritmo Bellman-Ford e opera com desempenho adequado para redes em pequena escala; porém, para redes com um maior número de elementos na camada de rede, o seu desempenho é ruim, se comparado ao tempo de convergência do OSPF.

g.	Um AS (sistema autônomo), ao se comunicar com outro AS, deverá efetuar uma troca de todas suas rotas internas, usando protocolos iGP, que podem ser o OSPF ou RIP, por exemplo.

h.	O protocolo RIP (Routing Information Protocol) utiliza a contagem de enlaces de rede como métrica. Dessa forma, se um pacote precisar passar por N redes para chegar ao seu destino final, o custo total dessa rota será N.

i.	O RIP (Routing Information Protocol) é um protocolo de roteamento que utiliza o algoritmo de roteamento denominado vetor distância.

j.	O OSPF é um protocolo IGP (Interior Gateway Protocol) de estado do enlace desenvolvido para operar em redes TCP/IP e para solucionar as limitações do RIP (Router Information Protocol).

k.	No protocolo OSPF, um roteador se comunica com seus vizinhos por multicast, em vez de broadcast, nos endereços 224.0.0.5 — com todos os roteadores — e 224.0.0.6 — com roteadores designados.

