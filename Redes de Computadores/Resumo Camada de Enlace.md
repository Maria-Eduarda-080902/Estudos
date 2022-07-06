## Camada de Enlace de Dados

### Introdução

- **Nós** são qualquer equipamento que rode um protocolo da camada de enlace. **Enlaces** são canais de comunicação que conectam dois nós adjacentes no caminho ca comunicação;
- Considerando dado enlace, um nó transmissor encapsula o datagrama em um quadro da camada de enlace e o transmite para dentro do enlace;
- A **camada de enlace** tem a responsabilidade de transmitir datagramas de um nó para o nó mais próximo;


### Serviços

- Enquadramento de Dados:
> A maior parte dos protocolos da camada de enlace encapsula o datagrama em um quadro da camada de enlace antes de transmiti-lo. Um quadro tem diferentes composições dependendo do protocolo da camada de enlace, mas a estrutura padrão é que contenha campos de cabeçalho + o datagrama da camada de redes.
- Acesso ao Enlace
> Um protocolo de controle de acesso ao meio (MAC) define as regras sob as quais os quadros serão transmitidos.
- Entrega Confiável
> Assim como outras camadas oferecem este serviço, a camada de enlace também busca aperfeiçoar a entrega de dados, especialmente em enlaces que possuem alta taxa de erro, como transmissão sem fio, com a finalidade de reslver o problema localmente ao invés de forçar a retransmissão fim a fim


- Enquadramento, acesso ao enlace:
> - Encapsula datagramas em quadros acrescentando cabeçalhos.
> - Implementa acesso ao canal se o meio é compartilhado.
> - ‘endereços físicos’ usados nos cabeçalhos dos quadros para Identificar a fonte e o destino dos quadros .
- Entrega confiável entre dois equipamentos fisicamente conectados:
> - Já aprendemos como isso deve ser feito: TCP!
> - Raramente usado em enlaces com baixa taxa de erro (fibra, alguns tipos de par de fios trançados de cobre).
- Controle de fluxo:
> - Limitação da transmissão entre transmissor e receptor.
> - Detecção de erros:
> - Erros causados pela atenuação do sinal e por ruídos.
> - O receptor detecta a presença de erros e avisa o transmissor para reenviar o quadro perdido.
- Correção de erros:
> - O receptor identifica e corrige o bit com erro(s) sem recorrer à retransmissão.
- Half-duplex e full-duplex
> - Com half-duplex, os nós em ambas as extremidades do enlace podem transmitir, mas não ao mesmo tempo.

### Adaptadores de Rede

> Na maior parte, a camada de enlace é implementada em um adaptador de rede, às vezes também conhecido como placa de interface de rede (NIC). No núcleo do adaptador de rede está o controlador da camada de enlace, em geral um único chip de sistema especial, que executa vários serviços da camada de enlace (enquadramento, acesso ao enlace, detecção de erros etc.). Dessa forma, muito da funcionalidade do controlador da camada de enlace é realizado em hardware. Até o final dos anos 1990, a maioria dos adaptadores de rede eram placas fisicamente separadas porém agora cada vez mais adaptadores de rede estão sendo integrados à placa-mãe do hospedeiro — uma configuração chamada LAN-na-placa-mãe.
> No lado transmissor, o controlador separa um datagrama que foi criado e o armazena na memória do hospedeiro por camadas mais altas da pilha de protocolos, encapsula o datagrama em um quadro da camada de enlace (preenchendo os vários campos do quadro), e então transmite o quadro para um enlace de comunicação, seguindo o protocolo de acesso ao enlace. No lado receptor, um controlador recebe todo o quadro e extrai o datagrama da camada de rede. 
> Se o protocolo da camada de enlace efetuar uma verificação de erros, é o controlador transmissor que estabelece os bits de detecção de erros no cabeçalho de quadro e é o controlador receptor que executa a verificação de erros.
> 


### Mind Dump

> - O protocolo de roteamento define o caminho que o datagrama tomará através dos enlaces individuais. A responsabilidade da camada de enace não é, na verdade, definir o caminho que o pacote tomará, apenas garantir que ele está indo para o próximo nó do jeito certo. 
