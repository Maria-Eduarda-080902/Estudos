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

Na revisão

- Hubs ampliam o domínio de colisão, enquanto switches e roteadores limitam;
- Hubs só repetem o sinal que recebem para todas as máquinas conectadas, enquanto o switch processa informação/endereços, e envia para todas as máquinas menos a que enviou para descobrir endereços e caminhos, possuindo aprendizado. Como o roteador atua na camada de rede, tem capacidade de processamento e possui informações sobre rotas.

### 4)	O cabeçalho da camada de enlace é sempre o mesmo ou depende da tecnologia? Qual o tamanho mínimo?

Depende da tecnologia. O tamanho mínimo é 0, já que algumas tecnologias não usam.

### 5)	O que é um endereço MAC e qual a sua relação com um endereço IP?

> Um endereço da camada de enlace é também denominado endereço de LAN, endereço físico ou endereço MAC (Media Access Control — controle de acesso ao meio). Para a maior parte das LANs (incluindo a Ethernet e as LANs 802.11 sem fio), o endereço MAC tem 6 bytes de comprimento, o que dá 248 endereços MAC possíveis. Tais endereços de 6 bytes costumam ser expressos em notação hexadecimal, com cada byte do endereço mostrado como um par de números hexadecimais. Apesar de os endereços MAC serem projetados como permanentes, agora é possível mudar o endereço de MAC de um adaptador via software.
>  Não existem dois adaptadores com o mesmo endereço, o IEEE gerencia o espaço físico de endereços MAC.

### 6)	Diferencie as topologias em estrela, em barra e em anel, citando vantagens e desvantagens.

#### Topologia Estrela

> É o tipo de configuração mais comum. A rede é organizada de forma que os nós sejam conectados a um hub central, que atua como um servidor. O hub gerencia a transmissão de dados pela rede. Ou seja, qualquer dado enviado pela rede viaja pelo hub central antes de terminar em seu destino.

> PRÓS:
> - Gerenciamento conveniente de um local central
> - Se um nó falhar, a rede ainda funciona
> - Os dispositivos podem ser adicionados ou removidos sem interromper a rede
> - Mais fácil de identificar e isolar problemas de desempenho

> CONTRAS:
> - Se o hub central falhar, toda a sua rede cairá
> - O desempenho e a largura de banda são limitados pelo nó central
> - Pode ser caro para operar


#### Topologia Barramento

> Também chamada de topologia de backbone, bus ou linha, orienta os dispositivos ao longo de um único cabo que vai de uma extremidade da rede à outra. Os dados fluirão ao longo do cabo conforme ele se desloca até seu destino.


> PRÓS:
> - Econômico para redes menores
> - Layout simples; todos os dispositivos conectados por meio de um cabo
> - Mais nós podem ser adicionados ao alongar a linha

> CONTRAS:
> - A rede é vulnerável a falhas de cabo
> - Cada nó adicionado diminui as velocidades de transmissão
> - Os dados só podem ser enviados em uma direção de cada vez

#### Topologia Anel

> Os nós são configurados em um padrão circular. Os dados viajam por cada dispositivo à medida que percorrem o anel. Em uma grande rede, repetidores podem ser necessários para evitar a perda de pacotes durante a transmissão. As topologias em anel podem ser configuradas como anel único (half-duplex) ou anel duplo (full-duplex) para permitir que o tráfego flua em ambas as direções simultaneamente.


> PRÓS:
> - Custo-beneficio
> - Barato para instalar
> - Fácil de identificar problemas de desempenho

> CONTRAS:
> - Se um nó cair, ele pode derrubar vários nós com ele
> - Todos os dispositivos compartilham largura de banda, o que pode limitar a taxa de transferência
> - Adicionar ou remover nós significa tempo de inatividade para toda a rede



### 7)	Explique para que serve e como funciona o protocolo CSMA/CD.

1. O adaptador obtém um datagrama da camada de rede, prepara um quadro da camada de enlace e coloca o quadro no buffer do adaptador.
2. Se o adaptador detectar que o canal está ocioso (ou seja, não há energia de sinal entrando nele a partir do canal), ele começa a transmitir o quadro. Por outro lado, se detectar que o canal está ocupado, ele espera até que não detecte energia de sinal, para então começar a transmitir o quadro.
3. Enquanto transmite, o adaptador monitora a presença de energia de sinal vinda de outros adaptadores usando o canal de difusão.
4. Se transmitir o quadro inteiro sem detectar energia de sinal de outros adaptadores, o adaptador terá terminado com o quadro. Por outro lado, se detectar energia de sinal de outros adaptadores enquanto transmite, ele aborta a transmissão (ou seja, para de transmitir seu quadro).
5. Depois de abortar, o adaptador espera por um tempo aleatório e depois retorna à etapa 2

### 8)	O que é um domínio de colisão?

> Domínio de colisão é uma área da rede na qual colisões de dados podem acontecer caso uma ou mais transmissões estejam sendo feitas simultaneamente. É um fenômeno que ocorre apenas em redes cujos nós tenham portas half-duplex, ou seja, não consigam transmitir e captar simultaneamente;

### 9)	Explique porque em cabos de rede metálicos com vários fios estes são agrupados em pares entrelaçados.

Fios trançados para minimizar as interferências. Fios paralelos geram campos eletromagnéticos fortes o bastante para desviar eletrons, o que acaba gerando, por exemplo, linhas cruzadas;

### 10)	Explique uma vantagem e uma desvantagem de cada meio de transmissão a seguir: par-trançado, fibra ótica, rádio, infravermelho, microondas.

#### Par-trançado
- Barato e fácil de encontrar, além de ser compatível com a maior parte das tecnologias.
- Decaimento da velocidade de transmissão conforme o comprimento do cabo aumenta. ATENUAÇÃO
- Ter regras específicas de conexão e recepção ao cripar o cabo;
- Interferência em cabos não blindados

#### Fribra Ótica
- Qualidade de transmissão excelente, pouquíssima perda de dados ([2^-15 - 2^-12])
- Baixíssima interferência;
- Baixíssima Atenuação;
- Alto preço de instalação e manutenção;
- Dificuldade de contratação e qualificação;
- Fragilidade e capacidade de reflexão de dados quando o cabo é dobrado a partir de certo ângulo;

#### Rádio
- As ondas de rádio são fáceis de gerar, podem percorrer longas distâncias e penetrar facilmente nos prédios; portanto, são amplamente utilizadas para comunicação, seja em ambientes fechados ou abertos. As ondas de rádio também são omnidirecionais, o que significa que elas viajam em todas as direções a partir da fonte; desse modo, o transmissor e o receptor não precisam estar cuidadosa e fisicamente alinhados.
- A transmissão omnidirecional pode ser uma desvantagem, já que a intensidade do sinal/taxa de transmis são vai se dissipar para todas os os sentidos, além de ser muito sujeita a interferências de outros canais;

#### Infravermelho
- É muito mais segura no que se trata de interferências, o que permite que qualquer pessoa consiga fazer transmissões por infravermelho sem precisar de licenças especiais. Por não atravessar sólidos, pode ser uma opção boa para ambientes fechados nos quais o sinal não poderá interferir em outros cômodos;
- Baixo consumo de energia;
- O sinal não atravessa objetos sólidos, então qualquer interferência física na frente da antena pode causar queda na rede e perda de dados;

#### Microondas
- Alta largura de banda, capacidade de transmitir mais dados;
- Alta mobiidade;
- Ondas cancerígenas;
- Interferência demais;
- Tendo em vista que as microondas viajam em linha reta, se as torres estiverem muito afastadas, a Terra acabará ficando entre elas (como acontece no caso de um enlace entre San Francisco e Amsterdam). Conseqüentemente, é preciso instalar repetidores a intervalos periódicos. Quanto mais altas são as torres, mais distantes elas podem estar umas da ou tras. A distância entre os repetidores aumenta de acordo com a raiz quadrada da altura da torre. 
- São basicamente ondas de rádio unidirecionais;
- A transmissão gasta muita energia;

### 11)	Porque a maioria das faixas de frequência é regulamentada por órgãos governamentais e não simplesmente livre para uso?

Basicamente, porque essas frequências estão sujeitas a interferência, sendo estas interferências tanto naturais quanto propositais por parte de usuários. Sendo assim, os governos se preocupam com questões de espionagem e de segurança de dados.

Na revisão: Se não existe regulamentação pela lei, faixas seriam usadas de tal maneira que existiria muita interferência. 

### 12)	Qual a importância dos repetidores e amplificadores em enlaces de comunicação?

Auxiliar na permanência, na linearidade da taxa de transmissão no meio de um enlace. Por exemplo, dois cabos de 50m com um repetidos no meio depredam o sinal metade do que um cabo de 100m, enquanto percorrem a mesma distância, aumentando a velocidade da transmissão e reduzindo perda de dados. O repetidor regenera o sinal, compreendendo o que está sendo transmitido e transmitindo novamente. O amplificador aumenta **todo** sinal que chega para ele, inclusive o ruído.

Amplificadores são praticamente inúteis em meios que possuem muito ruído, mas em meios como  fibra ótica com quase nenhum ruído é a melhor opção paraa redes de longa distância.

### 13)	Ao enviar um pacote para outra máquina, que tipo de consulta ARP é feita quando:
#### a.	O destino está na mesma rede local?
O IP verifica que o endereço de destino pertence à rede local e verifica na tabela ARP se a conversão já foi feita. Caso contrário, a consulta ARP é enviada via broadcast a todas as máquinas da rede. Todas as máquinas comparam o endereço IP do request com o seu próprio e só a máquina compatível responde diretamente para o host de origem e adiciona a relação IP/MAC à própria tabela. A máquina de origem recebe o reply e também adiciona a relação IP/MAC à sua tabela ARP;
#### b.	O destino está em uma rede local diferente?
A tabela de rotas da máquina é consultada para saber se existe uma rota conhecida para aquela máquina. Independente disso, a máquina de origem consulta sua tabela em busca de uma relação existente para o IP de pesquisa. Se não existir, um request é enviado via broadcast, contendo o endereço IP do roteador ao invés do endereço da máquina de destino. O roteador responde com seu MAC e a máquina de origem envia o pacote de dados para ele, que verifica se a máquina de destino é local ou externa. Se for externa, o processo é repetido. Se for local, o rotedor utiliza o ARP para obter o endereço físico da máquina de destino e envia o pacote diretamente para ela.
