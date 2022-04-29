### 1) Em que partes da topologia física da rede (não confundir com a arquitetura da rede) se implementam os protocolos de camada de aplicação e porquê?

*Nas bordas da rede, ou sistemas finais, pois são máquinas com softwares capazes de executar as aplicações e processar os dados, ao contrário do núcleo, cujas máquinas possuem softwares mais simples.*

### 2) Diferencie arquitetura cliente/servidor de arquitetura Peer-to-peer (ponto-a-ponto), com vantagens e desvantagens de cada uma.

> *Na arquitetura cliente-servidor, toda a informação a ser compartilhada está centralizada em uma máquina só (o servidor) e os hosts cliente apenas fazem solicitações a este servidor, não podendo fazer o papel de compartilhar informações. Enquanto isso, na arquitetura p2p, usuários diferentes detém informação e um host faz a solicitação dos dados diretamente à máquina detentora.*
<br><br> 
> *Vantagens da arquitetura cliente-servidor:*
> <li> Alta escalabilidade, rede evolutiva;
> **<li> Gerenciamento simples;
> <li> informação centralizada e de fácil acesso;
> <li> Segurança;

  
> *Desvantagens da Arquitetura Cliente-servidor:*
> <li> Servidor é um elo fraco. Qualquer problema que ocorra no servidor prejudica a rede inteira;
  
  
> *Vantagens da arquitetura P2P*
> <li> Perpetuação de arquivos. Com várias máquinas tendo cópias do arquivo, não existe um servidor que possa apagá-los ou alterá-los permanentemente;
> <li> Não vai existir um momento onde esta rede não funcionará, a não ser que a internet do mundo inteiro caia;
> <li> Com a repartição de dados, grandes conteúdos podem ser baixados em um intervalo de tempo muito menor;

  
> *Desvantagens da arquitetura P2P*
> <li> Aumenta a necessidade de "largura de banda" dedicada apenas a conexão conforme a rede aumenta;
> <li> Uma informação pode existir na rede e jamais ser acessada por alguém que procura, apenas por não solicitar à máquina certa;
> <li> Se uma máquina da qual o host que solicita a informação sai da rede, pode haver corrupção da informação. Ex: Se o usuário está baixando um filme, pode estar faltando uma cena.
> <li>  Grande exigência do desempenho do computador ao agir como um servidor;

  
### 3) Diferencie os principais requisitos de transporte que uma aplicação pode ter e dê exemplos de aplicação com tais requisitos.
  
<li> Tolerância a perda de dados:
  > Algumas aplicações exigem uma transferência de dados 100% confiável, enquanto outras toleram perda.
  > Por exemplo: Aplicações de tranferência de arquivos, aplicações de trocas de mensagens, emails, etc. não toleram perda e precisam que todos os dados enviados cheguem ao destino.
  > Enquanto aplicações de transmissão de audio e vídeo em tempo real toleram perdas de dados, considerando que a sincronização é mais importante do que a completude dos dados;
<li> Temporização:
  > Algumas aplicações exigem baixos atrasos para funcionarem.
  > Por exemplo: Jogos online não costumam tolerar muitos atrasos, e tais atrasos atrapalham o funcionamento do jogo;
  > Enquanto as aplicações menos toletantes a perda (transferência de arquivos, troca de mensagens, emails, etc) costumam trabahar bem mesmo com atrasos;
<li> Banda passante:
  > Algumas aplicações exigem uma taxa de transferência mínima para funcionarem corretamente.
  > Por exemplo: Audio e vídeo (armazenado ou em tempo real) geralmente exige uma banda minima, enquanto existem aplicações elásticas (transferência de arquivos, troca de mensagens, emails, etc) que buscam formas de transmitir os dados mesmo com uma taxa de transmissão menor que a ideal. 
  
### 4) Explique os métodos de formulário HTTP.

  > o método GET é utilizado para fazer "consultas" ou requisições ao servidor. Também utilizamos o GET quando os dados necessários para que o recurso correto seja encontrado devem permanecer na URL.
  > o método POST é utilzado para enviar dados para o servidor, seja para criar ou atualizar dados já existentes. Os dados enviados ao servidor não permanecem n URL, mas são armazenados no corpo da requisição HTTP;

### 5) Explique o que é proxy HTTP e como é feito o “proxy transparente” em HTTP.

  > Proxy: Entidade web existente em uma rede para servir de ponte conectando uma máquina ao restante da internet, fazendo solicitações em seu nome, recebendo informações externas antes de chegarem à máquina e lendo solicitações internas antes de irem diretamente à internet. São utilizados para bloquear certos tipos de acesso pré-determinados pelo usuário ou para bloquear certos tipos de arquivos indesejados.
  > Proxy transparente: Faz exatamente a mesma coisa que o Proxy, entretanto sem deixar o usuário saber que está sendo bloqueado. Geralmente substitui as mensagens de bloqueio por uma farsa, como algum erro de protocolo ou uma mensagem de que o site que o usuário tentou acessar está fora do ar, ou que o download não pôde ser completado. Há também o tipo que apenas desacelera a taxa de transmissão dedicada a rodar determinados conteúdos ou sites, especialmente em empresas, onde o acesso a certos pontos da rede, por lei, não pode ser bloqueado.

### 6) Explique porque se diz que o protocolo FTP é controlado “fora de banda”.

  > **"... o FTP usa duas conexões TCP paralelas para transferir um arquivo: uma
_conexão de controle_ e uma _conexão de dados_. A primeira é usada para enviar informações de controle entre os
dois hospedeiros — como identificação de usuário, senha, comandos para trocar diretório remoto e comandos de
“enviar” (put) e “receber” (get) arquivos. A conexão de dados é a usada para enviar de fato um arquivo. Como o
FTP usa uma conexão de controle separada, dizemos que ele envia suas informações de controle _fora da banda_."**

### 7) Explique porque é possível mandar mensagens usando o SMTP fazendo-se passar por outra pessoa, mesmo sem saber a senha da pessoa.

  > Porque o protocolo SMTP não exige autenticação de usuário nem da existência do endereço de email. Emails aleatórios podem ser criados na hora do envio d mensagm e senhas não são exigidas.

### 8) Quais as vantagens do protocolo IMAP em relação ao protocolo POP3?
  
 > O IMAP permite criação e acesso a pastas, e salva o estado da mensagem para ser acessado em diferentes dispositivos, enquanto o POP3 baixa as mensagens na máquina que o está acessando e fecha a conexão;

### 9) Explique como são organizados os servidores raiz do protocolo DNS.

  > **"Na Internet há 13 servidores DNS raiz (denominados de A a M) e a maior parte
deles está localizada na América do Norte. [...] Embora tenhamos nos referido a cada um dos 13 servidores DNS raiz como se fossem um servidor único, na realidade, cada um é um conglomerado de servidores replicados, para fins de segurança e
confiabilidade."**

### 10) Como é a configuração e o funcionamento da resolução de nomes reversa, isto é, de endereços IP para nomes de máquina?

  > 

### 11) Diferencie as redes P2P puras das redes P2P híbridas.

  > Nas redes P2P híbridas,existe um servidor que não guarda nada além de uma relação de quais máquinas possuem quais informações. Quando uma máquina procura por uma informação, o servidor retorna a informação de qual máquina a possui e o host que solicita estabelece uma conexão direta com a(s) máquina(s) que a possui(em); Na arquitetura P2P pura, não existe um servidor intermediário, apenas a conexão direta entre as máquinas.

### 12) Como funciona o protocolo Gnutella para busca de conteúdo?
  
  > Uma máquina faz uma solicitação para as máquinas com as quais tem contato. Se nenhuma delas possuir o conteúdo solicitado, elas repassarão a pergunta para a sua rede de contatos, e assim vai, até que uma máquina possua a informação solicitada. O limite de pulos de uma solicitação é 15, caso contrário algumas solicitações rodariam para sempre e sobrecarregariam a rede.

### 13) O que é multiplexação? Dê um exemplo não relacionado à camada de transporte.

  > Quando diversos canais de dados se juntam em um só enquanto seguem um mesmo caminho. A demultiplexação ocorre quando esse canal se separa em vários para enviar os dados a seus devidos destinos.
  > _"O trabalho de reunir, no hospedeiro de origem, porções de dados provenientes de diferentes portas, encapsular cada porção de dados com informações do cabeçalho (que mais tarde serão usadas na demultiplexação) para criar segmentos, e passar esses segmentos para a camada de rede é denominado multiplexação"._
  > Exemplo: Linha telefônica, TV digital, transmissão de satélite, etc.

### 14) Quais são as diferenças filosóficas entre TCP e UDP?

  > Enquanto o UDP dá mais valor à velocidade com a qual os dados são enviados e recebidos e menos à confiabilidade e integridade de tais dados, o TCP valoriza muito mais a integridade dos dados acima da velocidade de transmissão. 
  > <a href="https://www.alura.com.br/artigos/quais-as-diferencas-entre-o-tcp-e-o-udp?gclid=CjwKCAjw9qiTBhBbEiwAp-GE0e3QEgkj95Ra9QqZ71TNnbELsFHPfgsTyyXZhH4pu9nAp9bIhcQN8xoCiMEQAvD_BwE"> Alura: TCP e UDP </a>

### 15) Quais são as diferenças práticas entre o TCP e o UDP?

  > **" Há dois protocolos de transporte na Internet: TCP e UDP, e qualquer um pode levar mensagens da camada de aplicação. O TCP provê serviços orientados a conexão para suas aplicações. Alguns desses serviços são a entrega garantida de mensagens da camada de aplicação ao destino e controle de fluxo (isto é, compatibilização das velocidades do remetente e do receptor). O TCP também fragmenta mensagens longas em segmentos mais curtos e provê mecanismo de controle de congestionamento, de modo que uma origem reduz sua velocidade de transmissão quando a rede está congestionada. O protocolo UDP provê serviço não orientado a conexão para suas aplicações. É um serviço econômico que fornece segurança, sem controle de fluxo e de congestionamento."**
  > O UDP funciona sem um _aperto de mão_, ou seja, sem confirmação de recebimento de dados, o qu ajuda na velocidade.
  > **"Para manter a confiabilidade dos dados, o TCP utiliza um aperto de mãos de três vias, o _three way handshake_, também chamado de SYN,SYN-ACK,ACK.
<br>O nome _SYN,SYN-ACK,ACK_ é uma resumida descrição de como esse handshake funciona. A conexão entre dois hosts começa com o primeiro enviando ao segundo um pacote de sincronização (_SYN_chronize).
<br>O segundo host recebe esse pacote e responde com a confirmação do sincronização (_SYN_chronize-_ACK_nowledgment). O primeiro host, por fim, manda uma confirmação (_ACK_nowledge) para o segundo, assim estabelecendo a conexão."**

### 16) Em uma transmissão, como se identifica um processo específico em uma máquina? Dê exemplos.

  > Através das portas. Uma porta é um objeto abstrato de 16 bits utilizado exatamente para identificar processos de aplicações e que permite a comunicação entre duas máquinas. Existem portas bastante conhecidas (well-known ports) que servem a propósitos específicos.   
  > <li> 20 e 21 (FTP)
  > <li> 25 (SMTP)
  > <li> 80 (HTTP)
  > <li> 443 (HTTPS)
    
### 17) O que são sockets? Que funções são necessárias ao uso de sockets?

  > **"Qualquer mensagem enviada de um processo
para outro tem de passar pela rede subjacente. Um processo envia mensagens para a rede e recebe mensagens
dela através de uma interface de software denominada socket. Vamos considerar uma analogia que nos auxiliará
a entender processos e sockets. Um processo é semelhante a uma casa e seu socket, à porta da casa. Quando um
processo quer enviar uma mensagem a outro processo em outro hospedeiro, ele empurra a mensagem pela porta
(socket). O emissor admite que exista uma infraestrutura de transporte do outro lado de sua porta que transportará a mensagem pela rede até a porta do processo destinatário. Ao chegar ao hospedeiro destinatário, a mensagem passa pela porta (socket) do processo receptor, que então executa alguma ação sobre a mensagem."**
  > Sockets são interfaces de software através das quais processos enviam e recebem mensagens. Servem como "portas de entrada" de dados enviados pela rede.
  > 

### 18) Para que serve o checksum? Como ele funciona?

  > Checksum ou _soma de verificação_ serve para verificar se um arquivo é exatamente o mesmo antes e depois de sua transmissão, ou seja, para verificar corrupção do arquivo.
  > **"A soma de verificação é calculada usando uma função de hash e normalmente é lançada junto com o download. Para verificar a integridade do arquivo, um usuário calcula a soma de verificação usando um programa de soma de verificação e, em seguida, compara os dois para verificar se eles correspondem."**

### 19) Como são realizados o estabelecimento e o término de conexão do TCP?

  > **"Para manter a confiabilidade dos dados, o TCP utiliza um aperto de mãos de três vias, o _three way handshake_, também chamado de SYN,SYN-ACK,ACK.
<br>O nome _SYN,SYN-ACK,ACK_ é uma resumida descrição de como esse handshake funciona. A conexão entre dois hosts começa com o primeiro enviando ao segundo um pacote de sincronização (_SYN_chronize).
<br>O segundo host recebe esse pacote e responde com a confirmação do sincronização (_SYN_chronize-_ACK_nowledgment). O primeiro host, por fim, manda uma confirmação (_ACK_nowledge) para o segundo, assim estabelecendo a conexão."**
  > Dentro do cabeçalho de segmento TCP, existem seis campos de 1 bit que contêm a informação de controle usada para gerenciar os processos de TCP. Esses campos são:
  > <li>URG - Campo indicador de urgência
  > <li>ACK - Campo indicador de confirmação
  > <li>PSH - Função Push
  > <li>RST - Restabelecer a conexão
  > <li>SYN - Sincronizar números em sequência
  > <li>FIN - Não há mais dados do remetente
    
  > **"A fase de encerramento da sessão TCP é um processo de quatro fases, em que cada interlocutor responsabiliza-se pelo encerramento do seu lado da ligação. Quando um deles pretende finalizar a sessão, envia um pacote com a flag FIN ativa, ao qual deverá receber uma resposta ACK. Por sua vez, o outro interlocutor irá proceder da mesma forma, enviando um FIN ao qual deverá ser respondido um ACK."**


### 20) Como funciona a janela deslizante do TCP? Quais os modos de funcionamento e em que casos é feita a troca?

  > A janela deslizante do TCP serve como barreira, limitando a quantidade de dados que podem ser enviados a um receptor de acordo com quantos buffers de recebimento do receptor estão livres. Dados ficam no buffer de recebimento até serem lidos pela aplicação de recebimento.  
    
### 21) Como funciona o controle de fluxo do TCP?
  
    
    
### 22) Crie um protocolo de aplicação.

