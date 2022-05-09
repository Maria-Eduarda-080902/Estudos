# Lista 01 para a Prova

> Capítulos do Livro de Qualidade de Software para estudar: 1, 2, 4, 8 (ISO 9000), 10, 11, 12
> 
> Guia do Scrum
> 
> Livro Extreme Programming (Vinicius Teles) (opcional) https://engsoftmoderna.info/artigos/shape-up.html

### 1. Defina Qualidade de Software. Que motivação as empresas podem ter para implantação da qualidade do software?

> A definição mais básica de qualidade de software é: "Medida que confere se o software faz o que é esperado da forma esperada". Implantar qualidade de software, boas métricas e bons padrões ajuda a crescer em quesitos de maturidade, além de garantir a fidelidade de clientes e manter um bom nome no mercado. Produtos e processos de qualidade, apesar de precisarem de muito investimento, também são muito lucrativos.
### 2. Explique a diferença dos termos: erro, defeito e falha.

> **Erro**: Erro humano que causa o defeito no produto.
> 
> **Defeito**: Defeito é uma imperfeição do produto, que causa a interrupção total ou o mal-funcionamento do produto. Uma rotina mal aplicada, uma variável definida de maneira errada, etc.
> 
> **Falha**: Falha é o resultado errado que ocorre quando a parte defeituosa do produto é acessada.

> **O programador comete um _erro_, que gera um _defeito_ no código, que gera uma _falha_ na execução do produto.** 

### 3. Como funciona o sistema 5S?

> O sistema 5S é baseado na cultura japonesa, e, quando implementado, deve ajudar na melhora completa do ambiente, possibilitando o aumento da produtiviade e da qualidade de trabalho. Para ser aplicado, confia-se no bom senso das pessoas que trabalham no ambiente;

> **SEIRI – Senso de Utilização** : Separar o útil do inútil e descartar ou realocar tudo o que for inútil ao trabalho. Por exemplo, não faz sentido ter uma caixa de chocolates sobre a mesa de trabalho, então realoca-se a caixa para a geladeira. Isso ajuda a manter o ambiente visualmente mais limpo e livre de distrações, já que seu cérebro deixa de associar aquilo que estava sobre a mesa ao momento de trabalho;
> 
> **SEITON – Senso de Ordenação**: É importante ter lugares para cada objeto e ter cada objeto em seu lugar, e o principal meio para se alcançar essa organização é através de comunicação visual, sinalizações para que todas as pessoas que convivem no ambiente consigam entender e seguir.
> 
> **SEISOU- Senso de Limpeza**: Encontrar meios de eliminar o quanto possível as principais fontes de sujeita, para evitar perdas de materiais e, ainda mais, perda de tempo quando há a necessidade de limpar a mesa. Tanto para o Seiri quanto para o Seisou, é importante ter um local de descarte imediato próximo ao local.
> 
> **SEIKETSU – Senso de Saúde**: O objetivo é manter um ambiente favorável à saúde e à higiente, tanto fisiológica quanto mental.
> 
> **SHITSUKE – Senso de Autodisciplina** : Este é o coração da cultura dos 5s. Não deve ser necessário um fiscal para saber se todos os princípios estão sendo cumpridos, mas cada pessoa envolvida no ambiente de trabalho deve ter o **bom senso** de seguir com esta cultura por entendr como é benéfica a todos.

### 4. Como os fatores humanos podem contribuir para qualidade do software?

> Programadores cansados cometem erros que podem causar falhas grandes no software, além de não se preocuparem em pensar na melhor forma de programar alguma funcionalidade. Testadores cansados e estressados deixam passar casos de teste. E assim vai. Pessoas infelizes e desconfortáveis no ambiente de trabalho cometem erros muitas vezes graves, afetando a qualidade do produto e o andamento do projeto. 
> 
> Por desenvolvimento de software se tratar de trabalho intelectual não repetitivo, o estado mental daquele que o desenvolve afeta diretamente o produto.

### 5. Cite e explique algumas práticas de organizações maduras para buscar a qualidade de software.

> **Interação com o cliente**: Empresas maduras costumam tratar o cliente como um parceiro que deve estar bem envolvido no desenvolvimento dos contratos e dos produtos, visto seu objetivo em comum com a equipe de desenvolvimento. Desta forma, ambos os lados podem compreender bem as dificuldades e as capacidades do outro, tornando o entendimento mútuo mais fácil. Também é sempre interessante encontrar o equilíbrio entre bons contratos e conversas informais até o resultado final.
> 
> **Gerenciamento de projetos**: Fazer planos realistas e honestos é a melhor prática de gerenciamento de projetos, com a análise e gerência contínua de riscos e boas métricas para calcular prazos e custos, além de sempre buscar referências em projetos anteriores para entender o que funciona e o que não.
> 
> **Métricas**: Analisar e avaliar diversos aspectos de projetos anteriores e de projetos em andamento ajuda a empresa a entender quais são as medidas realistas e o que pode melhorar, e isto se direciona para diversas áreas: prazos, produtividade, tamanho de entregas, frequência de reuniões com o cliente, tempo para coleta e elicitação de requisitos.
> 
> **Treinamento e coaching**: Treinamentos formais para novos contratados e formação contínua para _"senpais"_. Desta forma, há a padronização nos processos de desenvolvimento de software e tanto novos contratados quanto veteranos conseguem sentir que são eles, os desenvolvedores, que formam de verdade a empresa, sentindose valorizados. Também é uma boa prática ter funcionários acostumados a ter treinamentos frequentemente, já que reduz a necessidade de novos contratos a cada vez que uma nova tecnologia precisa ser implementada.
> 
> **Revisões por pares**: Se um membro da equipe produz um artefato, este é revisado por outro membro. Isto soluciona o problema do apego de alguém àquilo que produz, deixando passar erros e problemas que alguém imparcial não deixaria passar.

### 6. Diferencie Qualidade do Processo e do Produto.

> A **qualidade do produto** se mede conforme o que era esperado deste determinado prodto e avaliando como ele foi entregue. Por exemplo, é esperado que um sistema de estoque possa realizar a inserção de dados de um produto em um banco de dados e que possa retornar estas informações para o usuário corretamente. Este sistema realiza isso? Claro, existem outras métricas, mas este é o básico.
> 
> A **qualidade do processo** pode ser medida coforme os projetos realizados com o tal processo forem analisados. Por exemplo, deve existir uma faixa de qualidade na qual os projetos realizados com este processo estão, e o processo deve se ajustar até que todos os produtos estejam nesta faixa.
> 
### 7. Faça uma comparação detalhada dos objetivos e atividades da garantia da qualidade e do controle da qualidade.

<table border="1" cellspacing="0" cellpadding="5" bordercolor="#000000">
<tr>
	<td><strong>Quality Assurance</strong></td>
	<td><strong>Quality Control</strong></td>
</tr>
<tr>
	<td>1.	Garantia da qualidade garante que o processo é definido e apropriado.</td>
	<td>1.	As atividades de controle da qualidade focam na descoberta de defeitos em i específicos.</td>
</tr>
<tr>
	<td>2.	Metodologia e padrões de desenvolvimento são exemplos de garantia da qualidade.</td>
	<td>2.	Um exemplo de controle da qualidade poderia ser: "Os requisitos definidos são os requisitos certos?".</td>
</tr>
<tr>
	<td>3.	Garantia da qualidade é orientada a processo.</td>
	<td>3.	Controle da qualidade é orientado a produto.</td>
</tr>
<tr>
	<td>4.	Garantia da qualidade é orientada a prevenção.</td>
	<td>4.	Controle da qualidade é orientado a detecção.</td>
</tr>
<tr>
	<td>5.	Foco em monitoração e melhoria de processo.</td>
	<td>5.	Inspeções e garantia de que o produto de trabalho atenda aos requisitos especificados.</td>
</tr>
<tr>
	<td>6.	As atividades são focadas no inicio das fases no ciclo de vida de desenvolvimento de software.</td>
	<td>6.	As atividades são focadas no final das fases no ciclo de vida de desenvolvimento de software.</td>
</tr>
<tr>
	<td>7.	Garantia da qualidade garante que você está fazendo certo as coisas e da maneira correta.</td>
	<td>7.	Controle da qualidade garante que os resultados do seu trabalho são os esperados conforme requisitos.</td>
</tr>
</table>


### 8. Cite Ferramentas e Técnicas utilizadas no controle da Qualidade.

> **Revisões**: Usar checklists com problemas recorrentes, seguir processos estruturados de revisão, criar produtos com base em revisões futuras;
> 
> **Coleta e estimativa de dados**: Manter um registro consistente de trabalho e de determinadas atividades ao longo dos projetos realizados. Desta forma, métricas podem ser aplicadas a partir dos dados coletados e o processo pode ser avaliado conforme aquilo que a empresa deseje melhorar em termos de qualidade.
> 
> **Custos associados com qualidade**:
> - Custos de investimento:
> São custos com treinamentos, aquisição de ferramentas e equipamentos, tempo de projeto dedicado a atividades como revisão, etc. Este tipo de custo deve ser otimizado de forma que a melhora do processo sempre ocorra e as equipes estejam sempre bem preparadas e satisfeitas e de forma a não extrapolar gastos com coisas desnecessárias.
> - Prejuízos:
> Custos com atendimento ao cliente, tempo gasto para corrigir defeitos no produto ou grandes problemas com equipamento. A melhor forma de reduzir estes custos é a melhora e adaptação contínua do processo.
> 
### 9. Que atividades o papel do SQA desempenha?

> **Teste de Software (V&V)**: O teste de software é usado para verificar que requisitos funcionais e não-funcionais foram devidamente implementados.
> 
> **Controle da Qualidade (Quality Control):** O controle da qualidade é definido como um processo e métodos usados para monitorar o trabalho e observar se os requisitos estão sendo satisfeitos.
> 
> **Gerenciamento de Configuração de Software (SCM - Software Configuration Management):** O SCM é responsável por identificar, rastrear e controlar mudanças nos elementos do software de um sistema. O SCM controla a evolução do sistema de software , gerenciando versões dos componentes de software e seus relacionamentos. O propósito é identificar todos os componentes inter-relacionados do software e para controlar sua evolução através das várias fases no ciclo de vida de desenvolvimento de software.

### 10. Como são realizadas as auditorias de qualidade?

> Uma pessoa ou equipe fora da área auditada (ou seja, fora da equipe de gerência de projeto ou simplesmente que não esteja envolvida pessoalmente no desenvolvimento do processo/produto) recebe treinamento e documentação específica, além de listas de verificação apontando detalhes que precisam ser verificados de maneira mais detalhada. Com toda a preparação feita, a equipe auditora se insere no ambiente de produção para observar a realização das atividades para, então, fazer um relatório contendo todas as faltas encontradas, todos os pontos observados, além de documentar também o que está funcionando. A partir daí, é feito um acompanhamento dos resultados ações corretivas impementadas, além da avaliação da necessidade de uma reauditoria. Todo este processo deve ser documentado e arquivado para auditorias futuras.
> 
### 11. No tocante à garantia de qualidade de software, está relacionada com uma de suas funções:
a) inspeções de requisitos;

b) testes de comparações;

**c) auditorias;**

d) criação da estrutura analítica do projeto (WBS);

e) reengenharia de processos.
### 12. Considere as afirmações relacionadas ao controle de qualidade de um projeto de software: Sobre as afirmações, pode-se dizer que está correto o contido apenas em



**a) I.**
> É realizado em todas as fases do ciclo de vida de um projeto (ao final delas)

b) II.

c) III.

d) I e III.

e) II e III.
### 13. Explique porque o processo SCRUM permite um aumento da produtividade e do aumento da qualidade do produto final.

> Tanto o produto como o processo são frequentemente reavaliados durante todo o período de produção. Desta forma, a equipe se reinventa e melhora o processo de desenvolvimento conforme necessário, aumentando a produtividade, e novos requisitos são aceitos com bastante flexibilidade, logo, o produto sempre atenderá às necessidades **atuais** do cliente
### 14. Baseado na figura abaixo, descreva DETALHADAMENTE como funciona o SCRUM (cada um dos itens destacados na figura).

> A partir de uma **visão do produto**, ou seja, do que o cliente tem em mente para o produto final, é dividida em partes, geralmente em funcionalidades ou requisitos no **backlog do produto**. A equipe reduz tais requisitos/exigências a um **backlog selecionado**, onde os requisitos alcançáveis e realistas do projeto estão. A partir do backlog selecionado, cada sprint **(período de até um mês dedicado ao desenvolvimento)** é planejada no **sprint planning**, uma reunião da equipe onde é determinado quantas e quais **novas funcionalidades** serão entregues. Lembrando que o objetivo geral é entregar um produto funcional ao fim de cada sprint. Ao final, é feita uma **revisão da sprint**, onde o backlog da sprint é comparado com o produto entregue ao fim dela. A **retrospectiva da sprint** é um momento de autoavaliação da equipe e da análise de várias métricas e registros que a equipe fez ao longo da sprint.
> 
### 15. Comente sobre as diferenças entre o desenvolvimento tradicional e o desenvolvimento ágil.

> Enquanto o desenvolvimento tradicional focava em entregar um enorme produto pronto com requisitos imutáveis e contratos extremamente fechados desde o começo do ciclo e vida do software, além de exigir documentações extensas e geralmente deixar o cliente de fora do processo de desenvolvimento, as metodologias ágeis buscam ser mais flexíveis no que se trata de definição de requisitos e na documentação, buscando uma boa comunicação constante e direta no período de desenvolvimento, além de buscar envolver o cliente em todo o processo do software.

### 16. Faça uma comparação das práticas do XP e do Scrum. Você pode fazer uma análise comparativa pelas fases do ciclo de vida que essas práticas atuam.

> As práticas e os valores do SCRUM são bastante genéricos e voltados mais para o processo. Apesar de ser amplamente utilizado para desenvolvimento de software, o scrum pode ser também facilmente adaptado a outros âmbitoa, o que seria mais difícil com XP, já que este possui princípios e práticas que focam bastante na qualidade do código, inclusive estabelecendo padrões para como este deve se parecer, como por exemplo a prática de refatoração, de projeto simples e de integração contínua.
> 
### 17. Os métodos ágeis de desenvolvimento de software como eXtreme Programming – XP consideram um conjunto de valores fundamentais derivados do manifesto ágil. Assim, estes métodos valorizam MENOS:
a) os indivíduos e a interação entre eles, do que os processos e ferramentas.

b) o software funcionando, do que uma documentação abrangente.

c) a colaboração com o cliente, do que negociação de contratos.

d) a resposta rápida a mudanças, do que seguir um plano previamente definido.

**e) a rigorosidade dos processos, do que a adaptação às mudanças.**
### 18. São exemplos de práticas da programação extrema (extreme programming):
a) integração contínua e releases longas e raras.

**b) programação em pares e refatoração**

c) presença do cliente e excesso de horas extras.

d) ausência de testes e planejamento incremental.

e) releases longas e raras e excesso de horas extras

### 19. Explique a técnica de estimativa Planning Poker.

> É uma técnica utilizada para alinhar e expor a visão de cada participante sobre o projeto em questão e sobre as histórias de usuário. Cada participante recebe um total de 13 cartas, de 0 a 100 na sequência Fibonacci, um ponto de interrogação e uma com uma imagem de café (que sugere uma pausa). A cada rodada, os jogadores estimam um valor para determinada história conforme os critérios que lhe vierem, e então, quando todos mostrarem suas cartas, os jogadores que estimaram o maior valor e o menor valor expõem suas razões para iniciar uma discussão sobre o valor da história.
> 
### 20. Descreva como funciona a metodologia shape-up.
### 21. Cite 3 diferenças do shape-up para outras metodologias ágeis.
### 22. Qual o propósito das Normas:
a) ISO 9001

b) ISO 9126 e 25000

> **ISO 9126**: Tem como objetivo definir um conjunto de características e subcaracterísticas que um bom software deve buscar, conforme seu objetivo principal, visando definir padrões de qualidade para produtos finais de Software.
> a
> **ISO 25000** : Tem como objetivo criar uma estrutura para a avaliação da qualidade de produtos de software;

### 23. O objetivo de uma organização, ao implementar os padrões da ISO 9001:2008, é
a) estabelecer um plano detalhado de projeto, para um produto inovador no mercado que supere as expectativas de seus clientes.

b) definir os indicadores corporativos de governança de processos.

c) ter um método de gerenciar os processos para que sejam construídos produtos que satisfaçam as expectativas de seus clientes.

d) controlar o funcionamento financeiro da empresa, desdobrando quais partes do custo de TI podem ser repassadas para as áreas clientes.

e) especificar a compra de uma ferramenta de gestão de TI adequada para o bom funcionamento dos processos.
### 24. A norma internacional ISO/IEC 9126-1 define um modelo para a avaliação da qualidade dos processos de desenvolvimento de software em geral, em que cada processo pode ser avaliado quanto a seis características. Trata-se de modelo genérico que pode ser utilizado por qualquer organização produtora de software.
(x) Certo ( ) Errado
### 25. Dentre os atributos de um software de qualidade, incluem-se:
a) controlabilidade, dependabilidade e eficiência

b) controlabilidade, eficiência e manutenibilidade

c) eficiência, imutabilidade e manutenibilidade

**d) eficiência, manutenibilidade e usabilidade**

e) imutabilidade, manutenibilidade e usabilidade
### 26. No tocante à garantia de qualidade de software, está relacionada com uma de suas funções:
a) inspeções de requisitos;

b) testes de comparações;

**c) auditorias;**

d) criação da estrutura analítica do projeto (WBS);

e) reengenharia de processos.
### 27. Em uma organização foram coletados os dados representados nos gráficos a seguir, para as medidas número de requisitos alterados após aprovação inicial e número de requisitos aprovados inicialmente. Analisando os gráficos, o que é possível concluir? Por quê?

> Que requisitos mudam conforme o tempo passa e necessidades mudam, especialmente com o bombardeio de informação no mundo e a velocidade com a qual eventos decorrem no mundo. Durante qualquer projeto, são necessárias revisões de requisitos, para que, ao fim, o produto continue sendo satisfatório. A mudança de requisitos é natural.

### 28. Defina duas medidas de acordo com o objetivo de medição abaixo utilizando o método GQM (Goal-Question-Metric). Para cada medida informe: nome, descrição, Fórmula de cálculo, tipo de medida, Procedimento de coleta e armazenamento, Procedimento de análise, Procedimento de Divulgação. Objetivo de Medição: Reduzir a quantidade de defeitos do projeto.
### 29. Associe cada característica da ISO 25000 a sua respectiva subcaracterística de qualidade:
1.Satisfação (3) Acessibilidade

2.Manutenibilidade (5) Confidencialidade

3.Usabilidade ( ) Conforto

4.Portabilidade (1) Testabilidade

5.Segurança (4) Substituibilidade

ISO / IEC 25010 - Modelos de sistema e qualidade de software: descreve o modelo, consistindo em características e sub-características, para qualidade de produto de software e qualidade de software em uso. O modelo de qualidade do produto definido na ISO / IEC 25010 compreende as oito características de qualidade relacionadas a seguir:
<table>
<tr>
<td>
Adequação Funcional: Essa característica representa o grau em que um produto ou sistema fornece funções que atendem às necessidades declaradas e implícitas quando usadas sob condições especificadas. Essa característica é composta das seguintes sub-características:
</td>
<td>
	
- Completude Funcional (Functional Completeness)
- Correção Funcional (Functional Correctness)
- Adequação Funcional (Functional Appropriateness)
	
</td>
</tr>
<tr>
<td>
Eficiência de Desempenho - Essa característica representa o desempenho em relação à quantidade de recursos usados nas condições declaradas. Essa característica é composta das seguintes sub-características:
</td>
<td>
	
- Comportamento Temporal (Time Behavior)
- Utilização de Recursos (Resource Utilization)
- Capacidade (Capacity)
	
</td>
</tr>
<tr>
<td>
Compatibilidade - Grau para o qual um produto, sistema ou componente pode trocar informações com outros produtos, sistemas ou componentes, e / ou executar suas funções necessárias, enquanto compartilha o mesmo ambiente de hardware ou software. Essa característica é composta das seguintes sub-características:
</td>
<td>
	
- Co-existência (Co-existence)
- Interoperabilidade (Interoperability)
	
</td>
</tr>
<tr>
<td>
Usabilidade - Grau em que um produto ou sistema pode ser usado por usuários específicos para atingir metas especificadas com eficácia, eficiência e satisfação em um contexto específico de uso. Essa característica é composta das seguintes sub-características:
</td>
<td>
	
- Reconhecimento de Adequabilidade (Appropriateness Recognizability)
- Aprendizagem (Learnability)
- Operacionalidade (Operability)
- Proteção Contra Erros do Usuário (User Error Protection)
- Estética da Interface do Usuário (User Interface Aesthetics)
- Acessibilidade (Accessibility)
	
</td>
</tr>
<tr>
<td>
Confiabilidade - Grau para o qual um sistema, produto ou componente executa funções especificadas sob condições especificadas por um período de tempo especificado. Essa característica é composta das seguintes sub-características:
</td>
<td>
	
- Maturidade (Maturity)
- Disponibilidade (Availability)
- Tolerância à Falhas (Fault Tolerance)
- Recuperabilidade (Recoverability)
	
</td>
</tr>
<tr>
<td>
Segurança - Grau para o qual um produto ou sistema protege informações e dados para que pessoas ou outros produtos ou sistemas tenham o grau de acesso a dados adequado aos seus tipos e níveis de autorização. Essa característica é composta das seguintes sub-características:
</td>
<td>
	
- Confidencialidade (Confidentiality)
- Integridade (Integrity)
- Não Repúdio (Non-repudiation)
- Autenticidade(Authenticity)
- Prestação de Contas(Accountability)
	
</td>
</tr>
<tr>
<td>
Manutenção / Manutenibilidade - Essa característica representa o grau de eficácia e eficiência com o qual um produto ou sistema pode ser modificado para melhorá-lo, corrigi-lo ou adaptá-lo a mudanças no ambiente e nos requisitos. Essa característica é composta das seguintes sub-características:
</td>
<td>
	
- Modularidade(Modularity)
- Reusabilidade(Reusability)
- Analisabilidade(Analysability)
- Modificabilidade(Modifiability)
- Testabilidade(Testability)
	
</td>
</tr>
<tr>
<td>
Portabilidade - Grau de eficácia e eficiência com o qual um sistema, produto ou componente pode ser transferido de um hardware, software ou outro ambiente operacional ou de uso para outro. Essa característica é composta das seguintes sub-características:
</td>
<td>
	
- Adaptabilidade(Adaptability)
- Instalabilidade(Installability)
- Replacibilidade(Replaceability)  
	
</td>
</tr>
</table>

### 30. Identifique pelo menos uma medida para cada uma das subcaracterísticas de qualidade abaixo indicando o nome da medida, a fórmula de cálculo e sua interpretação:
- Confidencialidade (subcaracterística de segurança): grau em que um produto ou sistema garante que os dados são acessíveis somente por pessoas autorizadas.
- Modificabilidade (subcaracterística de manutenibildiade): grau em que um produto ou sistema pode ser modificado de forma eficiente e eficaz sem a introdução de defeitos ou sem degradação de sua qualidade.
- Comportamento no tempo (subcaracterística de eficiência de desempenho): grau em que os tempos de resposta e de processamento e taxas de transferência de um produto ou sistema, no desempenho das suas funções, atende aos requisitos.
### 31. Cite 3 boas práticas de um programa de medição e 3 fatores críticos para implantação de um programa de medição.
