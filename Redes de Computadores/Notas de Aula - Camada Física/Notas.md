## Notas de Aula - Camada de Enlace

### Meios de Transporte Físicos

- **PAR TRANÇADO**

- Cabos de Rede comuns, mais conhecidos e amplamente usados;
- Fios trançados para minimizar as interferências. Fios paralelos geram campos eletromagnéticos fortes o bastante para desviar eletrons, o que acaba gerando, por exemplo, linhas cruzadas

- Cada par são dois fios de cobre de 1mm enrolados;

- Fios **blindados** possuem uma capa a mais de um material metálico. São menos maleáveis e menos usados pelo preço elevado, considerando que pares trançados já isolam bem e fazem um bom controle dos campos eletromagnéticos;

- A categoria mais comum é a 5 (ver tabela nos slides e ver normas)

- Existe uma ordem a ser respeitadas ao cripar o cabo:
 > - Branco-verde
 > - Verde
 > - branco-laranja
 > - azul
 > - branco-azul
 > - laranja
 > - branco-marrom
 > - marrom

- Não seguir a norma desta ordem pode causar problemas em cabos que são mantidos por várias pessoas. O cabo funcionará inicialmente se as duas pontas forem cripadas na mesma ordem, entretanto, o 

- Na maior parte dos casos, os cabos verdes são utilizados para transmissão e os laranjas são utilizados para recepção. Alguns protocolos podem usar todos;

- Se algum dos fios (verde ou laranja) parar de funcionar/quebrar, o cabo não funciona mais. Não existe protocolo de substituição.

- O hub inverte transmissão e recepção. Caso dois computadores precisem ser conectados diretamente, um cabo cross(over)/cruzado precisa ser feito, onde um tem a ordem comum e o outro tem a seguinte ordem: 

 > - Branco-laranja
 > - Laranja
 > - branco-verde
 > - azul
 > - branco-azul
 > - verde
 > - branco-marrom
 > - marrom

- Cabos cross podem ser usados em hubs e switchs, pois esses equipamentos têm a percepçao automática de qual par é utilizado para recepção e qual é utilizado para transmissão. Termo: Auto MDI/MDI-X

- Caixas Conectoras: existem "tomadas" específicas para cabos de par trançado. Estas tomadas possuem cabos que vão até o **patch panel**, e depois são conectados no switch através do **patch chord**, que também é o que conecta a 'tomada' ao computador;


- **CABO COAXIAL**

- Cabos semelhantes aos usados para antena parabólica (?)/tv a cabo, mas com resisteência muito diferente, impossível de aproveitar para redes;
- Pouco usado para redes, mais amplamente usado em sistemas de televisão;
- Forma redes frágeis, considerando que a remoção do terminador ou da interrupção de alguma conexão em T
- Possui dois condutores não parelelos e isolados por uma camada de plástico. A "alma", ou condutor interno, é responsável pela transmissão/recepção de dados (não ao mesmo tempo), e o condutor externo é responsável pelo aterramento.
- Melhor blindagem e menos flexibilidade em relação ao par trançado;
- 

- **FIBRA ÓPTICA**
- 
