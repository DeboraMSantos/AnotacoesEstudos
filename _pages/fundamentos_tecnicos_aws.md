<div style="display: flex; align-items: center;">
    <img src="https://upload.wikimedia.org/wikipedia/commons/9/93/Amazon_Web_Services_Logo.svg" alt="AWS Logo" style="width: 100px; margin-right: 10px;">
    <h1 style="margin: 0;">Fundamentos Técnicos da AWS</h1>
</div>

<p>Anotações referente ao curso Fundamentos Técnicos da AWS na Plataforma AWS SKILL BUILDER</p>

<menu> 
    
- [Módulo 1: Introdução à Amazon Web Services](#módulo-1-introdução-à-amazon-web-services-aws)
- [Módulo 2: Computação da AWS](#m%C3%B3dulo-2-computa%C3%A7%C3%A3o-da-aws)
- [Módulo 3: Infraestrutura Global e Confiabilidade](#módulo-3-infraestrutura-global-e-confiabilidade)
- [Módulo 4: Redes](#módulo-4-redes)
- [Módulo 5: Armazenamento e Bancos de Dados](#módulo-5-armazenamento-e-bancos-de-dados)
- [Módulo 6: Segurança](#módulo-6-segurança)
- [Módulo 7: Monitoramento e Análise](#módulo-7-monitoramento-e-análise)
- [Módulo 8: Definição de Preços e Suporte](#módulo-8-definição-de-preços-e-suporte)
- [Módulo 9: Migração e Inovação](#módulo-9-migração-e-inovação)
- [Módulo 10: A Jornada para a Nuvem](#módulo-10-a-jornada-para-a-nuvem)
- [Módulo 11: Noções Básicas do AWS Certified Cloud Practitioner](#módulo-11-noções-básicas-do-aws-certified-cloud-practitioner)

  
</menu>

# Módulo 1: Introdução à Amazon Web Services (AWS)

### Visão Geral do Curso
- **Zonas de Disponibilidade**: São regiões geográficas como América do Sul, Estados Unidos, etc.
- **Virtual Private Cloud (VPC) - Rede Privada**: É um serviço que permite a criação de uma rede virtual isolada dentro da infraestrutura da AWS.
- **Elastic Compute Cloud (EC2)**: Ele permite que você crie e execute máquinas virtuais escaláveis (chamadas de instâncias) na infraestrutura da AWS, sem precisar gerenciar o hardware físico.
- **Amazon S3 (Simple Storage Service)**: Usado para armazenar as fotos dos funcionários com capacidade de armazenamento ilimitado de qualquer tipo de arquivo.
- **Amazon CloudWatch**: Monitora a aplicação para garantir escalabilidade e tolerância a falhas.
- **Elastic Load Balancer (ELB)**: Distribui o tráfego entre as instâncias EC2.
- **Auto Scaling**: Escala automaticamente as instâncias de EC2 horizontalmente, conforme a demanda.
- **AWS IAM (Identity and Access Management)**: Controla o acesso aos recursos e gerencia identidades de forma segura.

### O que é a AWS?
A AWS é uma plataforma de computação em nuvem que oferece serviços de TI sob demanda pela internet. Isso permite que empresas eliminem a necessidade de gerenciar datacenters físicos, utilizando datacenters virtuais fornecidos pela AWS.

### Modelos de Implantação:  
  - **On-Premises:** Empresas mantém sua própria infraestrutura (data centers, hardware).  
  - **Nuvem:** Recursos são fornecidos pela internet com pagamento por uso, sem necessidade de gerenciar hardware físico.  
  - **Híbrida:** Combinação de recursos locais (on-premises) com a flexibilidade da nuvem, otimizando a infraestrutura.

### Benefícios:  
  Cada modelo fornece diferentes níveis de controle, flexibilidade e gerenciamento, permitindo que as empresas escolham a melhor estratégia de acordo com suas necessidades.
  
### Seis Vantagens da Computação em Nuvem
1. **Pagamento conforme o uso**: Pague apenas pelos recursos utilizados.
2. **Economia em escala**: Custo mais baixo devido ao uso agregado de vários clientes.
3. **Escalabilidade sem adivinhações**: Aumente ou reduza recursos conforme necessário.
4. **Velocidade e Agilidade**: Recursos de TI disponíveis em minutos com um clique.
5. **Economia de custos**: Concentre-se no seu negócio, deixando a infraestrutura nas mãos da AWS.
6. **Alcance Global**: Implante aplicações em várias regiões com baixa latência.

### Tipos de Computação em Nuvem
- **Nuvem Pública**: Serviços fornecidos por terceiros (como a AWS).
- **Nuvem Privada**: Infraestrutura própria, usada por uma única organização.
- **Nuvem Híbrida**: Combinação de nuvens públicas e privadas.

### Serviços Chave da AWS

### EC2 (Elastic Compute Cloud)
- Hospeda máquinas virtuais que podem ser escaladas conforme a demanda.

### S3 (Simple Storage Service)
- Armazenamento de objetos com capacidade ilimitada.

### IAM (Identity and Access Management)
- Gerenciamento de identidades e controle de acesso a recursos.

### CloudWatch
- Monitoramento de recursos e métricas para garantir alta disponibilidade.

### Auto Scaling
- Ajusta automaticamente a quantidade de instâncias EC2 de acordo com o tráfego.

### ELB (Elastic Load Balancer)
- Distribui o tráfego entre múltiplas instâncias EC2.

# Módulo 2: Computação da AWS
### EC2 (Elastic Compute Cloud)
- Hospeda máquinas virtuais que podem ser escaladas conforme a demanda.
- O EC2 permite que os usuários aluguem computadores virtuais, chamados "instâncias" 
- O usuário pode criar, lançar e terminar instâncias do servidor, conforme necessário 
- O usuário paga por hora pelos servidores ativos 
- O EC2 oferece controle detalhado para gerenciar a infraestrutura com escolhas de processadores, armazenamento e redes
#### Resumo dos Tipos de Instâncias EC2

  A diversidade de tipos de instâncias permite selecionar a configuração mais adequada às necessidades específicas da aplicação, garantindo eficiência e performance.
  
  As instâncias EC2 são comparadas aos funcionários de uma cafeteria, onde cada "funcionário" (instância) tem uma função específica para atender às demandas dos clientes.

#### Famílias de Instâncias

  - **Uso Geral:** Equilíbrio entre CPU, memória e rede, ideal para tarefas variadas como  servidores de jogos, servidores de aplicações  e repositórios de código.    
  - **Otimizadas para Computação:** Focadas em alto desempenho computacional para tarefas intensas, como servidores de jogos, computação de alto desempenho (HPC) e modelagem científica.    
  - **Otimizadas para Memória:** Recomendadas para cargas de trabalho que exigem grande quantidade de memória.    
  - **Otimizadas para Armazenamento:** São projetadas para cargas de trabalho que exigem alto acesso sequencial de leitura e gravação a grandes conjuntos de dados no armazenamento local. Projetadas para oferecer alto desempenho no acesso e processamento de dados armazenados localmente.    
  - **Computação Acelerada:** Utilizam aceleradores de hardware para cálculos com ponto flutuante, processamento gráfico e reconhecimento de padrões (semelhante ao funcionário que cria arte com café e leite).

#### Preços do Amazon EC2

- **Sob Demanda:** Paga apenas pelo tempo de execução (por hora ou por segundo), sem compromissos de longo prazo.

- **Savings Plans:** Oferece preços mais baixos mediante compromisso de uso consistente por 1 ou 3 anos por dolar, com economia de até 72%.

- **Instâncias Reservadas:** Indicadas para cargas de trabalho previsíveis, com descontos de até 75% em relação ao sob demanda.  
  *Opções de pagamento:* total antecipado, parcial ou sem pagamento inicial.

  Há dois tipos disponíveis de instância reservada a ***Standard Reserved Instances*** e ***Instâncias reservadas conversíveis***.  
  Com período de vigência disponíveis para 1 ou 3 anos, com maior economia no plano de 3 anos.
    
    - **Standard Reserved Instances:**  
      - Indicadas para cargas de trabalho com especificações definidas (tipo e tamanho da instância, plataforma, tenancy).  
      - Permite a reserva de capacidade se uma Zona de Disponibilidade for especificada.
    
    - **Instâncias Reservadas Conversíveis:**  
      - Oferecem maior flexibilidade para mudar entre diferentes Zonas de Disponibilidade ou tipos de instância, embora com desconto um pouco menor.
    
    - **Após o Período de Vigência:**  
      - A instância pode continuar funcionando como sob demanda, a menos que seja terminada ou substituída por uma nova reserva com atributos correspondentes.


- **Instâncias Spot:** Permitem solicitar capacidade excedente com descontos de até 90%, mas podem ser interrompidas com aviso de 2 minutos. Ideal para workloads tolerantes a interrupções.

- **Hosts Dedicados:** Servem para alocar hosts físicos exclusivos, atendendo requisitos de conformidade e garantindo tenant exclusivo.

### Scaling do AWS EC2

- **Conceito Básico:**  
  Assim como o café produzido por um funcionário em uma cafeteria, as instâncias EC2 "produzem" os recursos de computação necessários.

- **Elasticidade e Dimensionamento:**  
  - **Desafio On-Premises:**  
    - A demanda dos clientes varia ao longo do tempo, exigindo hardware suficiente para picos sem desperdiçar recursos na média.
  - **Solução AWS:**  
    - A capacidade pode ser ajustada automaticamente conforme a demanda, garantindo que os clientes sejam atendidos e reduzindo custos.

- **Redundância e Alta Disponibilidade:**  
  - Se uma instância falhar, outra é automaticamente provisionada, assegurando continuidade dos serviços.
  - O sistema é projetado para não ter pontos únicos de falha, mantendo o serviço disponível mesmo em situações críticas.

- **Amazon EC2 Auto Scaling:**  
  - **Scaling Dinâmico:** Responde em tempo real às variações de demanda.  
  - **Scaling Preditivo:** Ajusta a capacidade com base em previsões de demanda.  
  - **Combinação:** Integrar ambos os métodos permite uma resposta mais rápida e eficiente.

Este resumo sintetiza como a AWS utiliza elasticidade e dimensionamento para garantir serviços sob demanda, evitando desperdícios e melhorando a experiência do cliente.

- **Formas de Escalar:**
  - **Vertical:** Aumenta a potência das máquinas existentes.
  - **Horizontal:** Aumenta a quantidade de instâncias para lidar com a alta demanda.

- **Desacoplamento:**  
  Cada parte do sistema pode ser dimensionada separadamente, evitando provisionamento excessivo.

- **Amazon EC2 Auto Scaling:**
  - **Ajuste Dinâmico:** Adiciona ou remove instâncias conforme a demanda.
  - **Configurações do Grupo de Auto Scaling:**
    - **Capacidade Mínima:** Número mínimo de instâncias sempre ativas.
    - **Capacidade Desejada:** Número padrão de instâncias em operação.
    - **Capacidade Máxima:** Limite superior de instâncias mesmo em picos de demanda.
  - **Benefícios:**  
    - Otimiza custos, pois você paga somente pelo que é utilizado.
    - Garante uma experiência consistente para os clientes, sem sobrecarga ou desperdício de recursos.

### Direcionamento de tráfego com o Elastic Load Balancing   
- **Desafio de Distribuição:**  
  - Sem um sistema de roteamento, as solicitações (clientes) se acumulam desigualmente entre as instâncias (caixas), causando sobrecarga em alguns pontos e ociosidade em outros.

- **Função do ELB:**  
  - Atua como um "host" que direciona os clientes para a fila com menos carga, distribuindo uniformemente o tráfego entre as instâncias EC2.
  - Garante que, conforme o Auto Scaling adiciona ou remove instâncias, o tráfego seja roteado de maneira equilibrada e eficiente.

- **Benefícios:**  
  - Alta disponibilidade e desempenho, sem a necessidade de gerenciamento manual do balanceamento de carga.
  - Facilita uma arquitetura desacoplada, onde o front-end não precisa conhecer os detalhes do back-end, simplificando a gestão do tráfego.

### Sistema de mensagens e enfileiramento
- **Problema do Acoplamento Direto:**
  - No método tradicional, o operador de caixa passa o pedido diretamente para o barista.
  - Se o barista estiver ocupado ou indisponível, os pedidos podem atrasar ou ser perdidos.

- **Solução com Filas:**
  - Introdução de um buffer (fila) entre o operador e o barista permite que os pedidos sejam armazenados até serem processados.
  - Esse desacoplamento melhora a eficiência e isola falhas, garantindo que um componente não afete diretamente o outro.


#### Aplicações Monolíticas e Microsserviços

- **Aplicações Monolíticas:**
  - Constituídas por componentes fortemente acoplados (banco de dados, interface, lógica de negócios, etc.).
  - Falha em um componente pode levar à falha de toda a aplicação.

- **Microsserviços:**
  - Arquitetura baseada em componentes fracamente acoplados que operam de forma independente.
  - Se um componente falha, os demais continuam funcionando, evitando falhas em cascata.
  - Facilita a integração e comunicação por meio de serviços como Amazon SNS e Amazon SQS.

- **Serviços AWS:**
  - **Amazon SQS (Simple Queue Service):**
    - Enfileira mensagens para que possam ser processadas de forma assíncrona.
    - Garante que os pedidos (mensagens) sejam mantidos até que o consumidor os processe.
  - **Amazon SNS (Simple Notification Service):**
    - Implementa o modelo publish/subscribe, distribuindo mensagens para vários assinantes.
    - Pode enviar notificações para endpoints variados (e-mails, funções Lambda, SMS, etc.).

- **Benefícios da Abordagem com Filas:**
  - Permite a criação de arquiteturas desacopladas e resilientes.
  - Minimiza o impacto de falhas em cascata e melhora a escalabilidade dos sistemas.


    ### Comparação: Amazon SQS x Amazon SNS
    
    #### Amazon SQS (Simple Queue Service)
    - **Natureza:** Serviço de enfileiramento de mensagens.
    - **Funcionamento:**  
      - Mensagens são enviadas para uma fila onde ficam armazenadas até serem processadas por consumidores.
      - Ideal para comunicação assíncrona entre componentes, desacoplando produtores e consumidores.
    - **Características:**  
      - Garante a entrega das mensagens (com opções de filas FIFO ou padrão).
      - As mensagens permanecem na fila até serem processadas ou expirarem.
      - Útil para processos em lote, workflows e gerenciamento de cargas variáveis.
    
    ##### Amazon SNS (Simple Notification Service)
    - **Natureza:** Serviço de publicação/assinatura (pub/sub).
    - **Funcionamento:**  
      - Mensagens são publicadas em tópicos e distribuídas automaticamente a todos os assinantes.
      - A entrega é em tempo real para diversos endpoints (como e-mail, SMS, funções Lambda, ou até filas SQS).
    - **Características:**  
      - Não armazena mensagens para processamento posterior; a entrega é imediata.
      - Facilita o envio de notificações e alertas para múltiplos destinos simultaneamente.
      - Excelente para casos de uso que exigem comunicação instantânea e distribuição em larga escala.

    #### Resumo das Diferenças
    - **Modelo de Comunicação:**  
      - **SQS:** Ponto a ponto (fila) — armazena mensagens até que sejam processadas.
      - **SNS:** Pub/Sub — entrega mensagens para todos os assinantes instantaneamente.
    - **Uso Ideal:**  
      - **SQS:** Para desacoplar componentes e processar mensagens de forma assíncrona.
      - **SNS:** Para enviar notificações em tempo real e distribuir mensagens para vários destinos.
    - **Integração:**  
      - É comum usar SNS e SQS juntos; por exemplo, SNS pode distribuir notificações que são enfileiradas em SQS para processamento assíncrono.

        Esta combinação permite criar arquiteturas flexíveis, escaláveis e resilientes na AWS.
    #### Outros serviços de computação

- **Amazon EC2:**  
  - Máquinas virtuais que oferecem flexibilidade, confiabilidade e escalabilidade.  
  - Requer gerenciamento contínuo (patching, scaling, alta disponibilidade).

- **Computação Sem Servidor (Serverless):**  
  - **AWS Lambda:**  
    - Executa código em resposta a eventos sem a necessidade de provisionar ou gerenciar servidores.  
    - Escala automaticamente e é ideal para funções com duração de até 15 minutos.

- **Contêineres e Orquestração:**  
  - **Amazon Elastic Container Service (Amazon ECS) e Amazon Elastic Kubernetes Service (Amazon EKS):**  
    - Gerenciam e orquestram contêineres (usando Docker) para implantar aplicações em escala.  
    - Permitem maior eficiência e portabilidade sem acesso direto ao sistema operacional.
      
  - **AWS Fargate:**  
    - Plataforma sem servidor para execução de contêineres, eliminando a necessidade de gerenciar instâncias EC2.

# Teste de Conhecimento:
1. Você deseja usar uma instância do Amazon EC2 para uma carga de trabalho de processamento em lote. Qual seria o melhor tipo de instância do Amazon EC2 a ser usado?
- R: Otimizada para computação

2. Quais são as opções de duração do contrato para instâncias reservadas do Amazon EC2? (Selecione DUAS opções.)
- R1: 1 ano
- R2: 3 anos


3. Você tem uma carga de trabalho que será executada por um total de seis meses e consegue suportar interrupções. Qual seria a opção de compra mais econômica do Amazon EC2?
- R: Instância spot
  
4. Qual processo é um exemplo do Elastic Load Balancing?
- R: Garantir que nenhuma instância única do Amazon EC2 tenha que suportar a carga de trabalho completa sozinha.

5. Você deseja implantar e gerenciar aplicativos em contêineres. Qual serviço você deve usar?
- R: Amazon Elastic Kubernetes Service (Amazon EKS)

# Módulo 3: Infraestrutura Global e Confiabilidade
  
  - Se um evento (como um desfile, inundação ou queda de energia) bloquear uma unidade, os clientes podem simplesmente ir a outra próxima.
  - Essa rede de cafeterias garante que o serviço continue disponível, mesmo se uma unidade ficar indisponível.
  - A AWS opera em várias regiões pelo mundo, distribuindo os recursos entre múltiplos datacenters.
  - Se um datacenter falhar, as aplicações continuam disponíveis em outras regiões, assegurando tolerância a falhas.
  - Essa estratégia minimiza o risco de interrupção total dos serviços, mantendo a continuidade mesmo em situações adversas.

### Infraestrutura Global da AWS

- **Necessidade Comercial:**  
  Empresas precisam executar aplicações, armazenar dados e analisar informações. Antigamente, isso era feito em datacenters próprios, mas hoje a AWS oferece uma alternativa gerenciada.

- **Infraestrutura AWS:**  
  - A AWS constrói datacenters em grupos chamados **Regiões**.  
  - Cada região possui múltiplos datacenters que fornecem computação, armazenamento e outros serviços essenciais.  
  - Regiões são isoladas para garantir que os dados permaneçam sob jurisdição local, atendendo a requisitos de conformidade e governança.

- **Conectividade Global:**  
  - As regiões são interligadas por redes de fibra de alta velocidade, permitindo operações globais integradas.

- **Fatores para Seleção de Região:**  
  1. **Conformidade:** Necessidade de manter dados em determinadas jurisdições (ex.: Reino Unido, Alemanha).  
  2. **Proximidade:** Escolher regiões próximas aos clientes para reduzir a latência.  
  3. **Disponibilidade de Serviços:** Nem todas as regiões possuem todos os recursos; serviços novos podem ser lançados gradualmente.  
  4. **Preços:** Os custos podem variar conforme fatores locais, como impostos e custos operacionais.

  Ao escolher uma região, as empresas devem equilibrar conformidade, performance, disponibilidade de recursos e custo, garantindo que sua infraestrutura esteja próxima dos clientes e em conformidade com as leis locais.

#### Alta Disponibilidade com Zonas de Disponibilidade (AZs)

  - Executar uma aplicação em uma única instância ou datacenter (ou AZ) pode levar a interrupções caso ocorra um desastre.

#### Regiões
  - As regiões são locais geográficos onde a AWS hospeda seus datacenters. Exemplo: `us-east-1` (Norte da Virgínia), `sa-east-1` (São Paulo).
  - Cada região opera de forma independente e não compartilha dados sem consentimento do cliente
    
#### Zonas de Disponibilidade (AZs)
  -  As Zonas de Disponibilidade são datacenters localizados dentro de uma região.
     Exemplo: `us-east-1a` é uma AZ dentro da região `us-east-1` (Norte da Virgínia).
  - Os serviços podem ser implantados com escopo de Zona de Disponibilidade (AZ), Regional ou Global. 
  - Cada região é composta por múltiplas AZs, que são datacenters ou grupos de datacenters fisicamente separados e com infraestrutura redundante (energia, rede, conectividade).  
  - As AZs estão suficientemente distantes para evitar que um desastre afete todas simultaneamente, mas próximas o bastante para manter baixa latência.

#### Escopo dos Serviços AWS
- **Serviços Regionais**: AWS gerencia a durabilidade e disponibilidade dos dados entre AZs.
- **Serviços de AZ**: O cliente gerencia a replicação entre AZs para garantir a alta disponibilidade.
  
#### Prática Recomendada 
  - Implantar aplicações em pelo menos duas AZs dentro de uma mesma região para garantir continuidade do serviço em caso de falha de uma delas.
  - Serviços regionais (como o ELB) já operam em múltiplas AZs, facilitando a alta disponibilidade sem esforço adicional.

#### Benefício Final
  - Se uma AZ falhar, a aplicação continua operando nas demais, mantendo a disponibilidade e a resiliência da infraestrutura.


### Locais de Borda

- **Regiões e Proximidade:**  
  - As regiões AWS são áreas geográficas isoladas que permitem executar serviços essenciais.  
  - Escolher uma região próxima aos clientes melhora a latência.

- **Alta Disponibilidade:**  
  - Cada região é dividida em Zonas de Disponibilidade (AZs), datacenters fisicamente separados que garantem continuidade mesmo em caso de falhas.

- **Entrega de Conteúdo com Baixa Latência:**  
  - **Amazon CloudFront (CDN):**  
    - Armazena cópias em cache do conteúdo em locais de borda globalmente, proporcionando entrega rápida a usuários, independentemente de sua localização.      
  - **Amazon Route 53:**  
    - Serviço de DNS que direciona os clientes para os locais de borda com a menor latência.

- **AWS Outposts:**  
  - Permite executar uma versão local da AWS dentro do datacenter da empresa, para necessidades específicas que exigem operação on-premises.


  - A combinação de regiões, AZs, CloudFront, Route 53 e Outposts possibilita alta disponibilidade e desempenho otimizado para clientes em qualquer parte do mundo.
 
### Interação com a AWS
Na AWS, toda interação é feita através de chamadas de API autenticadas e autorizadas, que podem ser realizadas por meio de três ferramentas principais: **Console de Gerenciamento da AWS**, **AWS Command Line Interface (CLI)** e **SDKs da AWS**.

#### **Console de Gerenciamento da AWS:**
- **Interface Web:** Interface web que permite acessar e gerenciar serviços AWS rapidamente, com ferramentas de pesquisa, assistentes e fluxos de trabalho automatizados.
- **Categorias de Serviços:** Os serviços são agrupados em categorias, como Computação, Armazenamento, Banco de Dados, entre outros.
- **Seletor de Região:** Permite escolher a região onde você deseja executar os serviços.
- **AWS Console Mobile Application:**  
  Aplicativo móvel para monitorar recursos, visualizar alarmes e acessar informações de cobrança, suportando múltiplas identidades em sessão.

#### **AWS CLI:**
- **Linha de Comando Unificada:** Ferramenta para gerenciar produtos AWS por meio de comandos.
- **Automação e Scripts:** Pode ser usada para automatizar processos, como a coleta diária de dados de servidores.
- **Código Aberto e Multiplataforma:** Disponível para Windows, Linux e macOS.

**Exemplo de uso da CLI:**
- Comando: `aws ec2 describe-instances`
- Resposta: Dados detalhados sobre as instâncias EC2 em execução.

#### **SDKs da AWS:**
- **Integração com Linguagens de Programação:** Os SDKs (Kits de Desenvolvimento de Software) oferecem APIs específicas para diversas linguagens de programação que permitem integrar código de aplicação com os produtos da AWS.
- **Suporte a Múltiplas Linguagens:** Disponível para C++, Go, Java, JavaScript, .NET, Node.js, PHP, Python, Ruby, entre outros.
- **Exemplo de Código em Python:**
  ```python
  import boto3
  ec2 = boto3.client('ec2')
  response = ec2.describe_instances()
  print(response)
  ```
  Neste exemplo, o código usa o SDK do Python (boto3) para interagir com o serviço EC2 e listar as instâncias.

Essas ferramentas oferecem diferentes formas de acessar e gerenciar os recursos da AWS, desde uma interface visual até opções programáticas para automação e integração direta com código.

**Ferramentas de Automação e Gerenciamento de Infraestrutura:**
  - **AWS Elastic Beanstalk:**  
    - Automatiza o provisionamento de ambientes baseados no Amazon EC2.
    - Permite enviar código e configurações para que o serviço crie e gerencie recursos como instâncias EC2, balanceadores de carga, auto scaling e monitoramento.
    - Foca na aplicação, simplificando a criação e reimplantação de ambientes sem a necessidade de gerenciar cada recurso individualmente.
  
  - **AWS CloudFormation:**  
    - Ferramenta de infraestrutura como código (IaC) que utiliza templates (JSON ou YAML) para definir e provisionar recursos AWS de forma declarativa.
    - Garante implantações automatizadas, repetíveis e seguras, gerenciando as operações de API necessárias e revertendo alterações em caso de erros.
    - Permite a criação de ambientes idênticos em diversas contas e regiões, minimizando erros manuais.

- **Conclusão:**  
  - Para operações manuais e aprendizado, o Console é uma boa opção, enquanto a AWS CLI e os SDKs são essenciais para automação.  
  - Para gerenciamento de ambientes, o Elastic Beanstalk simplifica a implantação de aplicações e o CloudFormation possibilita a criação de infraestrutura como código, garantindo implantações seguras e consistentes.
  - 
### Teste de Conhecimento
#### 1. Qual das afirmações a seguir melhor descreve as Zonas de Disponibilidade?
R: Um único data center ou grupo de data centers em uma Região
#### 2. Qual declaração é VERDADEIRA para a infraestrutura global da AWS?
R: Uma Região consiste em três ou mais Zonas de Disponibilidade.
#### 3. Quais fatores devem ser considerados ao selecionar uma Região? (Selecione DUAS opções.)
R1: Conformidade com governança de dados e requisitos legais
R2: Proximidade com os clientes
#### 4. Qual declaração descreve melhor o Amazon CloudFront?
R: Um serviço global de entrega de conteúdo
#### 5. Qual site o Amazon CloudFront usa para armazenar cópias de conteúdo em cache para entregá-los mais rapidamente aos usuários em qualquer local?
R: Local de borda
#### 6. Qual ação você pode executar com o AWS Outposts?
R: Estender a infraestrutura e os serviços da AWS para diferentes locais, incluindo um data center on-premises.

# Módulo 4: Redes
#### VPC (Virtual Private Cloud)
- Seção isolada da nuvem AWS que permite definir uma rede virtual própria.  
- Permite criar **sub-redes (subnets)** para organizar recursos de forma lógica, definindo quais podem ser públicos ou privados.

#### Gateway de Internet (IGW)
- Necessário para que o tráfego da internet pública possa entrar e sair da VPC.  
- Funciona como a “porta de entrada” aberta ao público. Sem esse gateway, a VPC não é acessível externamente.

#### Gateway Privado Virtual (VGW)
- Possibilita criar uma conexão de VPN entre a VPC e uma rede privada (por exemplo, rede corporativa ou datacenter on-premises).  
- Permite tráfego criptografado de redes aprovadas, garantindo acesso seguro a recursos privados na VPC.

#### Conexão VPN vs. Tráfego de Internet
- A VPN utiliza a infraestrutura comum da internet, podendo sofrer problemas de latência ou congestionamento.  
- Mesmo criptografada, a conexão ainda está sujeita à rede pública.

#### AWS Direct Connect
- Oferece uma conexão física dedicada entre o datacenter local e a VPC.  
- Reduz custos, aumenta largura de banda e melhora a confiabilidade em relação à VPN, pois não compartilha a infraestrutura pública.

#### Em resumo
O **Amazon VPC** fornece controle sobre como os recursos na nuvem AWS são expostos ou protegidos. Você pode usar **gateways de internet** para recursos públicos, **gateways privados virtuais** para conexões VPN seguras e o **AWS Direct Connect** para uma conexão dedicada e mais confiável.

### Sub-redes e listas de controle de acesso à rede

#### 1. VPC (Virtual Private Cloud)
- É como um **castelo** (ambiente isolado) na AWS, onde você define quem entra e sai.
- Possui **gateways** (por exemplo, Internet Gateway) para comunicação externa.
- Dentro dela, você cria **sub-redes** (públicas e privadas) de acordo com necessidades de acesso e segurança.

#### 2. Sub-redes
- **Sub-rede Pública**:  
  - Possui acesso à internet via Internet Gateway.  
  - Hospeda recursos que precisam ser acessados externamente (ex.: servidores web).
- **Sub-rede Privada**:  
  - Não tem acesso direto à internet.  
  - Armazena recursos sensíveis (ex.: bancos de dados).  
  - Conexões de saída podem ser feitas por meio de um **NAT Gateway**, se necessário.

#### 3. NACL (Network Access Control List) – *Stateless*
- **Age no nível de sub-rede**, controlando o tráfego de entrada e saída (como um controle de passaporte).
- *Stateless*: não “lembra” requisições anteriores; cada pacote é analisado individualmente.
- Possui regras de permissão e negação:
  - **NACL padrão**: permite todo o tráfego, mas pode ser customizada.
  - **NACL customizada**: começa negando todo o tráfego até que você adicione regras de permissão.
  - Há sempre uma regra de **negação implícita** no final.

#### 4. Security Group (Grupo de Segurança) – *Stateful*
- **Age no nível de instância** (ex.: EC2).
- **Stateful**: “lembra” das conexões, permitindo o retorno do tráfego que foi originado pela instância.
- Por padrão:
  - **Tráfego de entrada negado** (todas as portas bloqueadas).
  - **Tráfego de saída permitido**.
- Você adiciona regras para **permitir** portas, protocolos e endereços IP específicos.

#### 5. Diferenças-Chave entre NACL e Security Group

| Característica           | NACL (Network ACL) | Security Group         |
|-------------------------|--------------------|------------------------|
| **Nível de atuação**    | Sub-rede           | Instância (EC2)        |
| **Tipo de filtragem**   | Stateless          | Stateful               |
| **Tráfego padrão**      | - Padrão permite tudo (NACL padrão)<br>- Customizada começa negando tudo | - Entrada negada<br>- Saída permitida |
| **Regras**              | Ordem importa (numérica) e há negação implícita | Sem ordem específica; se o tráfego corresponder a **qualquer** regra, ele passa |
| **Retorno de tráfego**  | Precisa de regra explícita de entrada e saída    | Lembra a conexão (retorno é liberado automaticamente) |

#### 6. Boas Práticas
- **Least Privilege**: permitir somente o mínimo necessário de acesso.
- **Sub-rede Pública**: hospeda o que precisa estar acessível ao público (web servers).
- **Sub-rede Privada**: hospeda dados sensíveis (bancos de dados); acessos externos podem ocorrer via NAT Gateway ou conexões VPN.
- **NACL**: controle mais amplo de tráfego entre sub-redes, bloqueando tentativas maliciosas no perímetro.
- **Security Group**: configurações específicas por instância, liberando apenas as portas necessárias.

#### 7. Outros Elementos de VPC
- **Internet Gateway**: permite que instâncias em sub-rede pública se comuniquem com a internet.
- **Gateway Privado Virtual (VGW)**: cria VPN para conectar data centers on-premises à VPC.
- **AWS Direct Connect**: conexão dedicada de alta velocidade entre o data center local e a AWS.


> **Em resumo**, entender a distinção entre NACL (nível de sub-rede, *stateless*) e Security Group (nível de instância, *stateful*) e saber configurar corretamente sub-redes públicas e privadas são pontos fundamentais para a certificação AWS.

### RedesGlobais
#### 1. DNS (Domain Name System)
- **Função**: Traduz nomes de domínio (ex.: `www.exemplo.com`) para endereços IP (ex.: `192.0.2.0`).
- **Analogia**: É como uma “lista telefônica” da internet.  
  - Quando o usuário digita um endereço no navegador, o **resolvedor DNS** do cliente solicita ao **servidor DNS** qual o IP correspondente ao domínio.

#### 2. Amazon Route 53
- **Serviço de DNS** gerenciado da AWS.
- Permite **rotear** usuários para recursos:
  - Instâncias do Amazon EC2, **load balancers**, ou até infraestrutura fora da AWS.
- **Gerenciamento de Domínios**:
  - Registrar novos domínios diretamente no Route 53.
  - Transferir registros DNS de outros registradores para manter tudo em um só lugar.
- **Políticas de Roteamento** disponíveis:
  - Baseada em **latência**: envia o usuário para a região mais próxima em termos de tempo de resposta.
  - **Geolocalização** ou **geoproximidade**: direciona usuários de acordo com sua localização geográfica.
  - **Weighted Routing** (roteamento por pesos): distribui tráfego conforme proporções definidas.

#### 3. Amazon CloudFront
- **CDN** (Content Delivery Network) da AWS.
- **Função**: Distribuir conteúdo estático e dinâmico (imagens, vídeos, arquivos) a partir de **locais de borda** próximos do usuário, reduzindo latência.
- **Exemplo de uso**:
  - Usuários na América do Norte recebem conteúdo de um local de borda em uma região próxima, como Oregon.
  - Usuários na Europa recebem o mesmo conteúdo de um local de borda em Dublin, melhorando o tempo de resposta.

#### 4. Integração Route 53 e CloudFront
1. O cliente solicita dados do site (por exemplo, `anycompany.com`).
2. **Route 53** faz a resolução de DNS, retornando o IP ou endpoint correspondente (ex.: `192.0.2.0`).
3. A solicitação do cliente é roteada para o **local de borda** mais próximo via **CloudFront**.
4. O **CloudFront** encaminha a solicitação para o **Application Load Balancer**, que direciona o tráfego para as instâncias do **Amazon EC2**.

#### 5. Benefícios Gerais
- **Menor latência**: conteúdo entregue de forma mais rápida ao usuário final.
- **Alta disponibilidade**: com roteamento e escalabilidade integrados.
- **Gestão facilitada**: administração de domínios e distribuição de conteúdo em um só lugar (AWS).


**Conclusão**: 
- **DNS** converte o domínio em IP para localizar a aplicação.
- **Amazon Route 53** oferece um DNS globalmente disponível, com roteamento avançado e registro de domínios.
- **Amazon CloudFront** melhora a performance ao distribuir conteúdo em locais de borda próximos ao usuário.



##  Teste seu conhecimento
#### 1. Qual declaração descreve melhor a lista de controle de acesso de rede-padrão de uma conta AWS?
R: Ela é stateless e permite todo o tráfego de entrada e saída.
#### 2. Qual declaração melhor descreve a resolução de DNS?
R: Converter um nome de domínio em um endereço IP
#### 3. Sua empresa tem um aplicativo que usa instâncias do Amazon EC2 para executar o site voltado para o cliente e instâncias de banco de dados do Amazon RDS para armazenar informações pessoais dos clientes. Como o desenvolvedor deve configurar a VPC de acordo com as práticas recomendadas?
R: Colocar as instâncias do Amazon EC2 em uma sub-rede pública e as instâncias de bancos de dados do Amazon RDS em uma sub-rede privada.
#### 4. Qual componente pode ser usado para estabelecer uma conexão privada dedicada entre o data center da sua empresa e a AWS?
R: AWS Direct Connect
#### 5. Qual declaração descreve melhor os grupos de segurança?
R: Eles são stateful e negam todo o tráfego de entrada por padrão.
#### 6. Qual componente é usado para conectar uma VPC à internet?
R: Gateway de internet
#### 7. Qual serviço é usado para gerenciar os registros de DNS para nomes de domínio?
R: Amazon Route 53

# Módulo 5: Armazenamento e Bancos de Dados
### Armazenamentos de instância e Amazon Elastic Block Store (Amazon EBS)


1. **Armazenamento em Nível de Bloco**
   - Equivale a “discos rígidos” que armazenam dados em blocos.
   - Atualizações são feitas apenas nos blocos modificados (eficiência para bases de dados e sistemas de arquivos).

2. **Armazenamento de Instância (Instance Store)**
   - Volumes físicos anexados ao host que executa a instância do EC2.
   - Dados são perdidos quando a instância é interrompida ou encerrada.
   - Útil para dados temporários ou que podem ser facilmente recriados (ex.: cache, arquivos de teste).

3. **Amazon EBS (Elastic Block Store)**
   - Serviço de armazenamento persistente em nível de bloco.
   - Volumes independentes do host físico; mantêm dados mesmo após interrupção ou encerramento da instância EC2.
   - É possível escolher tamanho, tipo de volume (SSD ou HDD), etc.
   - Ideal para aplicações que precisam manter dados críticos (como bancos de dados).

4. **Snapshots de EBS**
   - Backups incrementais: o primeiro snapshot copia todo o volume, os seguintes copiam apenas blocos alterados.
   - Permitem restaurar dados em caso de falha ou corrupção.
   - Boa prática: realizar snapshots regulares para proteger dados importantes.

**Conclusão**:  
- O armazenamento de instância é **efêmero**; só use para dados que podem ser perdidos.  
- O Amazon EBS oferece **persistência** e flexibilidade de tamanho/tipo, sendo adequado para workloads que requerem alto grau de disponibilidade de dados.  
- **Snapshots** são fundamentais para backup e recuperação de volumes do EBS.
  
### Amazon Simple Storage Service (Amazon S3)
#### 1. Conceito de Armazenamento de Objetos
- **Armazena dados como objetos** (dados + metadados + chave única).
- **Buckets**: “pastas” onde os objetos são armazenados.
- Ideal para **arquivos** (imagens, documentos, vídeos, backups, etc.).
- **Tamanho máximo de objeto**: 5 TB.

#### 2. Amazon S3
- Serviço de armazenamento em nível de objeto **altamente escalável e durável**.
- Possui **espaço praticamente ilimitado**.
- **Controle de acesso** via permissões (quem pode visualizar/editar).
- **Versionamento**: possível habilitar para manter histórico de alterações em objetos.
- **Hospedagem de site estático**: basta carregar arquivos HTML e habilitar a função de hosting.

#### 3. Storage Classes (Principais)
1. **S3 Standard**  
   - Acesso frequente.  
   - Armazenamento em pelo menos 3 Zonas de Disponibilidade (AZs).  
   - Alta disponibilidade e durabilidade (99.999999999%).  
   - Custo de armazenamento maior que classes para acesso infrequente.

2. **S3 Standard – Infrequent Access (IA)**  
   - Para dados acessados **raramente** mas precisam de **rápido acesso** quando necessário.  
   - Armazenado em pelo menos 3 AZs.  
   - Custo de armazenamento menor que Standard; custo de recuperação mais alto.

3. **S3 One Zone – IA**  
   - Armazena dados em **uma única AZ** (mais barato, porém menos resiliente).  
   - Para dados que podem ser recriados caso haja falha na AZ.

4. **S3 Intelligent-Tiering**  
   - Movimenta objetos automaticamente entre S3 Standard e IA conforme o padrão de acesso.  
   - Pequena taxa de monitoramento e automação mensal por objeto.

#### 4. Storage Classes de Arquivamento
1. **S3 Glacier Instant Retrieval**  
   - Acesso **imediato** (milissegundos) para dados arquivados.  
   - Custo menor que S3 Standard, mas voltado a dados de arquivo raramente acessados.

2. **S3 Glacier Flexible Retrieval**  
   - **Baixo custo** para arquivamento com recuperação de **minutos a horas**.  
   - Bom para armazenar registros antigos, fotos, vídeos que não precisam de acesso imediato.

3. **S3 Glacier Deep Archive**  
   - **Menor custo** de todas as classes, porém recuperação de **12 a 48 horas**.  
   - Ideal para retenção de longo prazo e conformidade.

4. **S3 Outposts**  
   - Para armazenamento em **ambientes on-premises** (AWS Outposts).  
   - Mantém dados próximos às aplicações locais que exigem alta performance ou requisitos de residência de dados.

#### 5. Políticas de Ciclo de Vida (Lifecycle Policies)
- **Movimentam objetos automaticamente** entre classes de armazenamento após determinado tempo.  
- Exemplos:
  - Ficar 90 dias em S3 Standard, depois mover para S3 Standard-IA por 30 dias.
  - Em seguida mover para S3 Glacier Flexible Retrieval para arquivo de longo prazo.

**Conclusão**:  
- O Amazon S3 **simplifica o armazenamento** de arquivos de todos os tipos.  
- Cada **storage class** equilibra **custo** e **disponibilidade** conforme a frequência de acesso e o tempo de retenção.  
- **Políticas de ciclo de vida** automatizam a migração de dados, reduzindo custos e esforço de gerenciamento.  
- **Versionamento** e **controle de acesso** fornecem maior segurança e rastreabilidade dos objetos.

#### Amazon EBS vs. Amazon S3 — Qual a Melhor Opção?

#### 1. Contexto Geral
- **Amazon EBS (Elastic Block Storage)**  
  - Armazenamento em **blocos**.  
  - Cada volume pode chegar até **16 TiB**.  
  - Persistente mesmo quando a instância EC2 é interrompida ou terminada.  
  - Atualizações acontecem em nível de blocos (não precisa regravar o arquivo inteiro).  

- **Amazon S3 (Simple Storage Service)**  
  - Armazenamento em **objetos** (pensa em arquivos inteiros).  
  - Armazena dados de forma **ilimitada**; cada objeto pode ter até **5 TB**.  
  - Garantia de durabilidade de **99.999999999%** (11 noves).  
  - Suporte nativo à Web (cada objeto tem sua própria URL).  
  - Custo efetivo e sem necessidade de gerenciar servidores (serverless).

#### 2. Comparando os Casos de Uso

#### Round 1: Aplicativo de Análise de Fotos
- **Milhões de imagens** para upload, indexação e visualização.
- S3 oferece:
  - Armazenamento **ilimitado**.  
  - URLs nativas para cada objeto.  
  - Alta durabilidade e sem preocupação extra de backup.  
  - Custos menores que EBS para armazenar grandes quantidades de dados estáticos.  
  - **Conclusão**: S3 vence para esse tipo de workload (objetos estáticos, acesso global, URLs públicas).

##### Round 2: Arquivo de Vídeo de 80 GB com Edição Constante
- **Edição frequente** de vídeo, com muitas mudanças pontuais.
- EBS oferece:
  - Armazenamento em **blocos** (atualiza só as partes alteradas).  
  - Evita regravar todo o arquivo cada vez que uma pequena mudança é feita.  
  - **Conclusão**: EBS vence para workloads que exigem mudanças constantes, pois S3 exigiria upload completo a cada alteração.

#### 3. Quando Usar Cada Serviço
- **S3**:  
  - Armazenamento de objetos “write once/read many”.  
  - Hospedagem de arquivos estáticos, imagens, documentos, arquivos de mídia.  
  - Acesso via URL e integração fácil com aplicações web (serverless).  
  - Altamente escalável para grandes quantidades de dados.

- **EBS**:  
  - Armazenamento de blocos para instâncias EC2.  
  - Ideal para bancos de dados, sistemas de arquivos, ou edições frequentes.  
  - Atualizações delta em nível de bloco.

#### 4. Conclusão
- **Não há um “vencedor universal”**. Cada serviço se destaca em **situações diferentes**:
  - **S3** para “upload/download de arquivos completos” e acesso distribuído.  
  - **EBS** para “escritas e leituras intensas” em nível de blocos, junto a EC2.  
- **Saiba qual é o padrão de uso da sua aplicação** para escolher o serviço (ou combinação) ideal.


### Amazon EFS (Elastic File System)

1. **Conceito de Sistema de Arquivos Compartilhado**  
   - Permite que **várias instâncias** (servidores, aplicações, etc.) acessem **simultaneamente** um repositório central de arquivos.
   - Ao contrário de **armazenamento em blocos** (EBS) ou **armazenamento de objetos** (S3), o EFS fornece um **sistema de arquivos** completo.

2. **Características do Amazon EFS**
   - **Gerenciado e elástico**: expande ou contrai de forma automática conforme você adiciona ou remove dados, sem necessidade de provisionamento prévio.
   - **Recurso regional**: armazena dados em **várias Zonas de Disponibilidade (AZs)**, oferecendo alta disponibilidade e redundância.
   - **Acesso simultâneo**: várias instâncias EC2 (em qualquer AZ da mesma região) podem **ler e gravar** no mesmo sistema de arquivos.
   - **Compatível** com servidores on-premises via **AWS Direct Connect** para cenários híbridos.

3. **Comparação EBS vs EFS**

| **Amazon EBS**                                   | **Amazon EFS**                                          |
|--------------------------------------------------|---------------------------------------------------------|
| **Nível de AZ**: um volume está ligado a uma AZ  | **Nível regional**: dados replicados em múltiplas AZs   |
| **É um “disco rígido”** para uma única instância  | **Várias instâncias** podem compartilhar ao mesmo tempo |
| Dimensionamento **fixo** (é preciso aumentar manualmente o volume) | **Cresce e diminui** automaticamente                   |
| Ideal para **bancos de dados** e aplicativos que precisam de armazenamento em bloco com alta IOPS | Ideal para **sistemas de arquivos compartilhados**, workflows que exigem múltiplos servidores acessando dados simultaneamente |

---

**Conclusão**:  
- O **Amazon EFS** é perfeito para cenários em que diferentes serviços ou instâncias precisam ler e gravar em um **mesmo sistema de arquivos** com escalabilidade automática.  
- O **Amazon EBS** continua sendo adequado para armazenamento em bloco vinculado a uma instância específica, em uma única AZ.  
- Cada serviço atende a necessidades de armazenamento distintas, então a escolha depende do padrão de acesso e uso dos dados.

### Amazon Relational Database Service (Amazon RDS)

Bancos de Dados Relacionais e Serviços AWS

#### 1. Conceito de Banco de Dados Relacional
- **Dados organizados em tabelas** (linhas/colunas), onde cada registro pode se relacionar a outro.
- **SQL (Structured Query Language)**: principal forma de interação (consultas, atualizações, etc.).
- Exemplos de RDBMS populares: MySQL, PostgreSQL, Oracle, SQL Server, etc.

#### 2. Opções na AWS
1. **Executar RDBMS em Instâncias EC2 (Lift & Shift)**
   - Você gerencia OS, armazenamento, patches, backups.
   - Prático para migração direta de ambientes on-premises.
2. **Amazon RDS**
   - Serviço gerenciado para bancos de dados relacionais.
   - Automatiza provisionamento de hardware, aplicação de patches, backups e alta disponibilidade.
   - Compatível com mecanismos: MySQL, PostgreSQL, MariaDB, Oracle, SQL Server e Amazon Aurora.

#### 3. Amazon Aurora
- **Banco de dados relacional** de nível empresarial.
- Compatível com MySQL e PostgreSQL, porém **mais rápido** (até 5x comparado a MySQL comum e 3x comparado a PostgreSQL comum).
- **Alta disponibilidade**: 6 cópias dos dados em 3 Zonas de Disponibilidade.
- **Backups contínuos** para o S3 e suporte a Point in Time Recovery.
- **Custo-efetivo**: reduz operações desnecessárias de E/S e mantém confiabilidade.

#### 4. Benefícios do RDS/Aurora
- **Menos trabalho operacional**: a AWS cuida de tarefas como upgrades, manutenção, backups.
- **Failover automático** e **alta disponibilidade**.
- **Escalabilidade**: fácil aumentar ou diminuir recursos (CPU, memória, armazenamento).
- **Segurança**: criptografia em repouso e em trânsito, integração com VPC e IAM.

**Conclusão**: Para armazenar dados relacionais na AWS, as opções variam desde gerenciar tudo em instâncias EC2 (lift & shift) até usar o **Amazon RDS** ou **Aurora**, que oferecem maior automação, confiabilidade e desempenho. A escolha depende das necessidades de controle, custo, desempenho e escalabilidade de cada aplicação.



### Amazon DynamoDB (Banco de Dados Não Relacional)

#### 1. Conceito de Banco de Dados Não Relacional (NoSQL)
- **Armazenamento em formato de chave-valor**, sem esquema rígido (cada registro pode ter atributos diferentes).
- Focado em alta **escalabilidade** e **baixa latência**.
- Não há consultas complexas que envolvem múltiplas tabelas; **consultas simples** baseadas em chaves.

#### 2. Características do DynamoDB
- **Sem servidor (Serverless)**: você não gerencia instâncias, patches ou infraestrutura.
- **Escalonamento automático**: ajusta capacidade para lidar com grandes variações de carga.
- **Altamente distribuído e replicado**: dados armazenados em múltiplas Zonas de Disponibilidade, garantindo alta disponibilidade.
- **Tempo de resposta em milissegundos**: ideal para aplicações que exigem latência muito baixa e alto throughput.

#### 3. Diferenciação de Bancos Relacionais
- **NoSQL**: maior **flexibilidade** de schema, mas consultas menos complexas.
- **Relacional (SQL)**: suporte a relações entre tabelas e consultas complexas, mas pode ter limitações de escalabilidade se não for bem planejado.

#### 4. Casos de Uso
- Aplicações web/móveis de grande escala, com variação de dados (atributos dinâmicos).
- Workloads com picos de tráfego massivos (ex.: grandes eventos de vendas, PrimeDay da Amazon).
- Cenários em que adicionar/remover atributos frequentemente se faz necessário sem alterar todo o schema.

#### 5. Exemplo Real
- **PrimeDay 2019**:  
  - 7,11 **trilhões** de chamadas de API ao DynamoDB em 48 horas.  
  - Pico de **45,4 milhões** de solicitações por segundo.  
  - Sem necessidade de gerenciar servidores ou infraestrutura.

**Conclusão**:  
O DynamoDB é um **banco de dados NoSQL** altamente escalável, com **latência de milissegundos**, sem gerenciamento de servidores. Ele traz flexibilidade de schema (chave-valor) e é ideal para aplicativos que precisam lidar com grande quantidade de acessos e dados variáveis.  




### Amazon Redshift (Data Warehouse para Análises Históricas em Grande Escala)

### 1. Contexto
- Bancos de dados transacionais (relacionais ou NoSQL) são ótimos para:
  - **Trabalho em tempo real**: leituras/escritas rápidas e confiáveis.
  - **Gestão de dados atuais** (estoques, vendas em tempo real, etc.).
- **Desafio**: Quando o volume e a variedade de dados tornam-se muito grandes, ou quando queremos **análises históricas** complexas, precisamos de uma solução especializada.

### 2. Conceito de Data Warehouse
- Focado em **analisar dados históricos** (ex.: volume de vendas, tendências ao longo do tempo).
- Permite **consultas complexas** para identificar insights (BI – Business Intelligence).
- Armazena dados vindos de diversas fontes (financeiro, estoque, varejo, etc.).

### 3. Amazon Redshift
- **Serviço de data warehouse na AWS**.
- Capaz de lidar com **petabytes** de dados e, com o recurso **Spectrum**, permite consultar **exabytes** de dados em um data lake (S3).
- Otimizado para:
  - **Consultas analíticas** complexas.
  - **Grande volume de dados** (Big Data).
  - **Alta performance**: pode ser até 10x mais rápido que bancos relacionais comuns em workloads analíticos.
- **Gerenciado**: reduz o fardo operacional de provisionar, escalonar e manter infraestrutura.

### 4. Quando Usar Redshift?
- **Análises de longo prazo**: vendas mensais, comportamento de clientes em um período, previsões.
- **Integração de múltiplas fontes**: dados de ERP, CRM, varejo, IoT, etc.
- **Big Data e BI**: construção de relatórios e dashboards que auxiliam a tomada de decisão.

**Conclusão**:  
Para **análise histórica** e **inteligência de negócios** em grande escala, o **Amazon Redshift** fornece um ambiente de data warehouse gerenciado, com desempenho otimizado para **consultas analíticas** que envolvem **quantidades massivas de dados**.

### AWS Database Migration Service (AWS DMS)

#### 1. Propósito
O **AWS DMS** (Database Migration Service) ajuda a **migrar bancos de dados** (relacionais ou não) para a AWS com **tempo de inatividade reduzido**. É possível:
- **Transferir dados** entre bancos de diferentes tipos (MySQL → Aurora, Oracle → PostgreSQL, etc.).
- **Manter o banco de dados de origem operacional** durante a migração, minimizando impacto em aplicativos.

#### 2. Casos de Uso Principais
1. **Desenvolvimento e Testes**
   - Permite testar aplicações em um ambiente com **dados de produção** sem afetar usuários reais.
2. **Consolidação de Banco de Dados**
   - Combina múltiplos bancos de dados em um único destino, simplificando a gestão.
3. **Replicação Contínua**
   - **Sincroniza dados** para fins de backup, relatórios ou carga de trabalho híbrida, ao invés de apenas uma migração pontual.

**Conclusão**:  
O AWS DMS **facilita a migração e replicação** de dados entre diversas origens e destinos, permitindo **baixos tempos de inatividade** e suporte a diversos tipos de bancos de dados, seja on-premises ou já na AWS.

### Serviços de banco de dados adicionais

1. **Uso de Banco de Dados Apropriado**  
   - Não existe um “banco de dados universal” para todos os casos.  
   - Selecione o tipo de banco de dados ou plataforma de armazenamento **com base nas necessidades** do projeto (escalabilidade, relacionamento, tipo de dado, latência etc.).

2. **Serviços Adicionais de Banco de Dados na AWS**
   - **Amazon DocumentDB**  
     - Compatível com cargas de trabalho do MongoDB.  
     - Ideal para armazenar documentos JSON (catálogos, perfis de usuário, gerenciamento de conteúdo).
   - **Amazon Neptune**  
     - Banco de dados de **grafos**.  
     - Perfeito para redes sociais, mecanismos de recomendação, detecção de fraudes.
   - **Amazon QLDB (Quantum Ledger Database)**  
     - Banco de dados **ledger imutável**.  
     - Mantém histórico completo, sem possibilidade de remoção de registros (auditabilidade).
   - **Amazon Managed Blockchain**  
     - Criação e gerenciamento de redes **blockchain** com frameworks de código aberto (Hyperledger Fabric, etc.).  
     - Adequado quando se deseja transações distribuídas sem autoridade central.
   - **Amazon ElastiCache**  
     - Camada de cache gerenciado para bancos de dados tradicionais e aplicações.  
     - Compatível com **Redis** e **Memcached**, reduzindo a latência de leituras repetidas.
   - **Amazon DynamoDB Accelerator (DAX)**  
     - Cache em memória para **DynamoDB**.  
     - Reduz latências de milissegundos para **microssegundos** em leituras de dados não relacionais.

3. **Conclusão**
   - Escolha a ferramenta com base no **caso de uso**:  
     - **Documentos** (Amazon DocumentDB),  
     - **Grafos** (Amazon Neptune),  
     - **Ledger Imutável** (Amazon QLDB),  
     - **Blockchain Distribuído** (Amazon Managed Blockchain),  
     - **Cache** (Amazon ElastiCache ou DAX).  
   - Utilize **a melhor opção** para cada demanda ao invés de forçar um modelo de dados único para todas as aplicações.



### Teste seu conhecimento
#### 1. Você quer armazenar dados que são acessados com pouca frequência, mas devem estar imediatamente disponíveis quando necessário. Qual storage class do Amazon S3 você deve usar?
R: S3 Standard-IA 
#### 2. Quais storage classes do Amazon S3 são otimizadas para dados de arquivamento? (Selecione DUAS opções.)
R1: Amazon S3 Glacier Flexible Retrieval
R2: Amazon S3 Glacier Deep Archive
#### 3. Qual(ais) afirmação(ões) é(são) VERDADEIRA(S) sobre os volumes do Amazon EBS e sistemas de arquivos do Amazon Elastic File System?
R: Os volumes do EBS armazenam dados em uma única Zona de Disponibilidade. Os sistemas de arquivos do Amazon EFS armazenam dados em várias Zonas de Disponibilidade.
#### 4.Você quer armazenar dados em um serviço de armazenamento de objetos. Qual serviço da AWS é o melhor para esse tipo de armazenamento?
R: Amazon Simple Storage Service (Amazon S3)
#### 5.Qual afirmação melhor descreve o Amazon DynamoDB?
R: 
Um serviço de banco de dados de chave-valor sem servidor
#### 6. Qual serviço é usado para consultar e analisar dados em um data warehouse?
R: Amazon Redshift

# Módulo 6: Segurança
## Modelo de Responsabilidade Compartilhada da AWS

Quando você usa a AWS, a segurança é uma responsabilidade compartilhada entre você e a AWS. Isso é conhecido como o "modelo de responsabilidade compartilhada," dividido em dois conceitos:

A AWS providencia a infraestrutura da nuvem, enquanto o cliente é responsável pela segurança do que implementa nessa infraestrutura.

![image](https://github.com/user-attachments/assets/f6bf140b-c64d-49b1-8e2f-4b31bb95a782)


### **Responsabilidades da AWS: Segurança *da* Nuvem**
A AWS é encarregada de proteger a infraestrutura que suporta todos os serviços oferecidos na AWS Cloud, o que envolve:

- **Software e Hardware**: Gerencia todos os aspectos da computação, armazenamento, bancos de dados e redes.
- **Infraestrutura Física**: Responsável pela segurança física dos data centers e pelo gerenciamento de toda a infraestrutura de hardware e software.
- **Proteção Global**: Cuida da segurança das Regiões AWS, Zonas de Disponibilidade e locais de borda, assegurando a integridade e a proteção física em todos os níveis da infraestrutura.
- **Segurança de Host e Virtualização**: Encarrega-se do sistema operacional do host e das camadas de virtualização, garantindo a separação e o isolamento apropriados dos recursos virtuais.

#### **Categorias de Serviços AWS e Responsabilidades Correspondentes:**

1. **Serviços de Infraestrutura** (ex.: Amazon EC2)
   - **Responsabilidade AWS**: Administração da infraestrutura básica e dos serviços essenciais.

2. **Serviços de Contêiner** (ex.: Amazon RDS)
   - **Responsabilidade AWS**: Gerenciamento da infraestrutura, serviços essenciais, sistema operacional e plataforma de aplicações.

3. **Serviços Abstratos** (ex.: Amazon S3)
   - **Responsabilidade AWS**: Administração da infraestrutura, do sistema operacional, das plataformas de aplicação, da criptografia do lado do servidor e da proteção de dados.

#### **Nota sobre Serviços de Contêiner da AWS**: 
Os "Serviços de Contêiner" da AWS referem-se a serviços que automatizam o gerenciamento de aplicações, não estando relacionados a contêineres Docker. Isso minimiza a responsabilidade dos clientes pelo gerenciamento da plataforma e infraestrutura, ficando sob a gestão da AWS.



### **Responsabilidades do Cliente: Segurança *na* Nuvem**
Como cliente da AWS, você tem a responsabilidade de proteger os recursos que implementa e utiliza na nuvem. Essas responsabilidades variam conforme o tipo de serviço AWS utilizado:

- **Dados do Cliente**: Responsabilidade total pela segurança dos dados.
- **Plataforma e Aplicações**: Inclui o gerenciamento de sistemas operacionais, aplicações e Identity and Access Management (IAM).
- **Configuração de Rede**: Abrange a configuração de sistemas operacionais, rede e firewall, além da criptografia de dados.

**Detalhamento por Categoria de Serviço:**
1. **Serviços de Infraestrutura**
   - **AWS**: Gerencia a infraestrutura e os serviços base.
   - **Cliente**: Gerencia o sistema operacional, a plataforma de aplicação, a criptografia e a segurança dos dados.

2. **Serviços de Contêiner**
   - **AWS**: Gerencia a infraestrutura, serviços base, sistema operacional e plataforma de aplicação.
   - **Cliente**: Responsável pela segurança dos dados do cliente, implementação de criptografia, e medidas de segurança como firewalls e backups.

3. **Serviços Abstratos**
   - **AWS**: Gerencia a infraestrutura, o sistema operacional, as plataformas de aplicação, e a criptografia do lado do servidor.
   - **Cliente**: Gerencia e protege os dados do cliente, incluindo a criptografia do lado do cliente.

Estas responsabilidades sublinham a importância do controle que você mantém sobre seus conteúdos e a necessidade de uma configuração e gestão cuidadosas, dependendo do tipo e da complexidade dos serviços utilizados na AWS.


## Proteja o usuário raiz da AWS

### Autenticação vs. Autorização
- **Autenticação**: Verifica a identidade do usuário (ex: e-mail e senha).
- **Autorização**: Define o que o usuário pode fazer (ex: ler, editar, criar).

### Usuário Raiz da AWS
- Conta criada inicialmente com acesso total a todos os produtos e dados.
- **Credenciais**: 
  - **Login**: E-mail e senha para o console de gerenciamento.
  - **Chaves de acesso**: ID e chave secreta para solicitações via CLI ou API.
- **Melhores práticas**:
  - Use uma senha forte.
  - Nunca compartilhe credenciais.
  - Desative/exclua as chaves de acesso, a menos que sejam necessárias.
  - Use o usuário raiz apenas para tarefas específicas.

### Autenticação Multifator (MFA)
- **MFA**: Adiciona segurança ao exigir dois métodos de autenticação (ex: senha + token de segurança).
- **Por que usar MFA?**: Protege contra o acesso indesejado, mesmo que uma senha seja comprometida.
- **Como habilitar MFA na AWS**:
  1. Primeiro, use e-mail e senha.
  2. Depois, insira um código gerado pelo dispositivo MFA.

### Tipos de Dispositivos MFA
- **MFA Virtual**: Aplicativos móveis que geram códigos únicos (ex: Google Authenticator).
- **Dispositivos de Hardware**: Chaveiros ou cartões que geram códigos numéricos.
- **U2F (Fator Universal de 2ª Geração)**: Dispositivo físico conectado via USB (ex: Yubikey).

Habilitar MFA é uma recomendação da AWS para maior segurança das contas e recursos.

## AWS Identity and Access Management


O AWS Identity and Access Management (IAM) é um serviço da AWS que permite gerenciar o acesso à sua conta e aos recursos da AWS. Ele define quem pode autenticar (fazer login) e quem pode autorizar (ter permissões) para usar os recursos. Com o IAM, é possível compartilhar acesso sem expor chaves ou senhas, oferecendo permissões granulares aos usuários para acessarem apenas o que for necessário.

### **Recursos do IAM:**
- **Global:** O IAM não é específico de uma região e funciona em todas as regiões da AWS.
- **Integração:** Já vem integrado com muitos serviços AWS.
- **Políticas de Senha:** Permite definir complexidade e rotação de senhas.
- **MFA:** Suporta autenticação multifator.
- **Federação de Identidades:** Permite que usuários de sistemas externos acessem temporariamente a conta AWS.
- **Gratuito:** O uso do IAM não gera custos adicionais.

### **Usuários e Grupos do IAM:**
- Um **usuário do IAM** é qualquer pessoa ou serviço que interage com a AWS. Cada usuário possui credenciais únicas e permissões definidas.
- Os **grupos do IAM** são coleções de usuários que herdam permissões atribuídas ao grupo, facilitando a gestão de acesso, por exemplo, separando grupos por função como "desenvolvedores" ou "administradores."

### **Credenciais do Usuário IAM:**
- Acesso ao **Console de Gerenciamento AWS** com usuário e senha.
- **Acesso Programático** via AWS CLI e APIs utilizando chaves de acesso.
- Gerenciar permissões diretamente nos usuários é possível, mas agrupar por grupos é uma prática recomendada para facilitar a administração.

### **Políticas do IAM:**
As **políticas** definem permissões para usuários, grupos e funções. Elas são escritas em JSON e têm quatro principais elementos:
- **Version:** Define a versão da linguagem de política.
- **Effect:** Especifica se a permissão é "Allow" (permitir) ou "Deny" (negar).
- **Action:** Determina as ações permitidas ou negadas (por exemplo, `iam:ChangePassword`).
- **Resource:** Especifica os recursos afetados.

### **Exemplos de Políticas:**
- **Política de Administrador:** Permite todas as ações em todos os recursos:
  ```json
  {
    "Version": "2012-10-17",
    "Statement": [{
      "Effect": "Allow",
      "Action": "*",
      "Resource": "*"
    }]
  }
  ```
- **Política Granular:** Permite que um usuário altere sua própria senha e obtenha suas próprias informações:
  ```json
  {
    "Version": "2012-10-17",
    "Statement": [{
      "Effect": "Allow",
      "Action": [
        "iam:ChangePassword",
        "iam:GetUser"
      ],
      "Resource": "arn:aws:iam::123456789012:user/${aws:username}"
    }]
  }
  ```

Essas políticas ajudam a gerenciar permissões específicas para os recursos da AWS, tornando o acesso seguro e organizado.


## Acesso baseado em função na AWS

### 1. Bloquear o Usuário Raiz
- O usuário raiz tem acesso total à conta.
- **Recomendações de Segurança**:
  - Não compartilhe credenciais.
  - Exclua chaves de acesso desnecessárias.
  - Habilite MFA para proteção adicional.

### 2. Princípio de Privilégio Mínimo
- Conceda apenas as permissões mínimas necessárias para cada tarefa.
- Comece com permissões básicas e adicione conforme a necessidade.

### 3. Uso Apropriado do IAM
- O IAM é para gerenciar o acesso a recursos da AWS.
- Não é usado para autenticação de sites ou segurança de sistemas operacionais/redes.

### 4. Preferir Funções do IAM
- As funções oferecem credenciais temporárias, expiram após 15 min a 36 horas.
- Mais seguro e flexível do que gerenciar usuários com credenciais de longo prazo.

### 5. Usar um Provedor de Identidade (IdP)
- Facilita o gerenciamento de identidades para equipes maiores.
- Usando um IdP, é possível associar funções do IAM para identidades federadas, centralizando a gestão de permissões.

### 6. Considere o AWS Single Sign-On (SSO)
- Ideal para organizações com muitos funcionários e várias contas AWS.
- Permite login único (SSO) para acessar várias contas e aplicações.
- Oferece integração com IdPs de terceiros para sincronizar usuários e grupos, separando claramente a gestão de identidade e acesso à nuvem.


### AWS Organizations

AWS Organizations é uma ferramenta para consolidar e gerenciar múltiplas contas AWS de uma empresa em um local central. Ao criar uma organização no AWS, é automaticamente criada uma raiz, que serve como contêiner principal para todas as contas na organização.

#### Características Principais

#### Controle Centralizado
- **Políticas de Controle de Serviço (SCPs)**: Permitem a administração centralizada das permissões, restringindo os serviços AWS, recursos e ações de API que usuários e funções podem acessar em cada conta.

#### Cobrança Consolidada
- A cobrança consolidada é facilitada pelo AWS Organizations, permitindo uma gestão financeira mais eficiente das várias contas.

#### Unidades Organizacionais (UO)
- **Agrupamento de Contas**: Contas podem ser agrupadas em Unidades Organizacionais (UO) para gerenciamento simplificado, especialmente útil para contas com requisitos de negócios ou segurança semelhantes.
- **Herança de Políticas**: Ao aplicar uma política a uma UO, todas as contas na UO automaticamente herdam as permissões especificadas na política.

#### Exemplo Prático

#### Passo 1: Estrutura Organizacional
- Imagine uma empresa com contas AWS separadas para os departamentos de Financeiro, TI, RH e Jurídico. Ao consolidar essas contas em uma organização, estabelece-se uma raiz.

#### Passo 2: Sem UO
- Os departamentos de Financeiro e TI são colocados diretamente sob a raiz por terem requisitos distintos, sem sobreposição com outros departamentos.

#### Passo 3: Com UO
- Os departamentos de RH e Jurídico são colocados em uma UO juntos, permitindo a aplicação de políticas comuns que cobrem ambos os departamentos.

#### Conclusão
- O uso de UOs permite o acesso facilitado aos serviços e recursos necessários, enquanto impede o acesso a serviços ou recursos desnecessários. Além disso, o acesso continua sendo gerenciado por meio do IAM para usuários, grupos e perfis.


### Conformidade - AWS Artifact

AWS Artifact é um serviço da AWS que fornece acesso sob demanda a relatórios de segurança e conformidade, bem como a contratos on-line relacionados ao uso de serviços AWS.

#### Principais Componentes do AWS Artifact

#### AWS Artifact Agreements
- **Descrição**: Permite visualizar, aceitar e gerenciar contratos para uma conta individual ou todas as contas no AWS Organizations.
- **Utilidade**: Especialmente útil para clientes sujeitos a regulamentações específicas, como a HIPAA nos EUA.
  
#### AWS Artifact Reports
- **Descrição**: Oferece relatórios de conformidade de auditores terceirizados que verificaram a adesão da AWS a normas e regulamentações de segurança globais, regionais e setoriais.
- **Utilidade**: Ideal para membros da equipe que precisam de evidências de conformidade para desenvolvimento de aplicações em ambientes regulados.
- **Exemplos de Relatórios**: Inclui certificações ISO da AWS, relatórios do Payment Card Industry (PCI), e Service Organization Control (SOC).

#### Centro de Conformidade para o Cliente
- **Recursos**: Contém histórias de conformidade de clientes, whitepapers, e documentação sobre conformidade, além de oferecer um plano de aprendizagem para auditores.
- **Finalidade**: Ajuda a entender como demonstrar conformidade usando a nuvem AWS em setores regulamentados.

#### Benefícios do AWS Artifact
- **Acesso Instantâneo**: Acesso imediato a documentos importantes sem a necessidade de solicitações formais.
- **Transparência de Conformidade**: Facilita a demonstração de conformidade com regulamentações necessárias para auditores e reguladores.
- **Gestão de Contratos**: Simplifica o gerenciamento de acordos legais e de conformidade para usuários de AWS Organizations.

### Ataques de Negação de Serviço (DoS e DDoS)

#### Analogia da Cafeteria
- **Problema**: Clientes fazem pedidos por telefone e nunca os retiram, bloqueando a linha para clientes legítimos.
- **Solução Tentativa**: Bloquear o número do telefone usado para fazer pedidos falsos.
- **Semelhança com DoS**: O comportamento é comparável a um ataque de negação de serviço, onde um invasor sobrecarrega um serviço para torná-lo indisponível.

#### Ataques de Negação de Serviço (DoS)
- **Definição**: Tentativa deliberada de tornar um site ou aplicação indisponível, inundando-o com tráfego excessivo até que fique sobrecarregado.
- **Impacto**: Usuários legítimos não conseguem acessar o serviço.

#### Ataques Distribuídos de Negação de Serviço (DDoS)
- **Cenário**: Múltiplas fontes (possivelmente coordenadas por um único ator) sobrecarregam um serviço, tornando difícil ou impossível bloquear os ataques devido ao número variado de fontes.
- **Complexidade**: Um único ator pode usar muitos computadores infectados para atacar, aumentando a escala e o impacto do ataque.

#### AWS Shield
AWS Shield é um serviço projetado para proteger aplicações contra ataques DDoS.

#### AWS Shield Standard
- **Cobertura**: Proteção automática para todos os clientes AWS, sem custos adicionais.
- **Proteção**: Mitiga os tipos mais comuns de ataques DDoS.
- **Funcionamento**: Utiliza técnicas de análise para detectar e mitigar tráfego mal-intencionado em tempo real.

#### AWS Shield Advanced
- **Custo**: Serviço pago com recursos avançados.
- **Capacidades**: Oferece diagnósticos detalhados de ataques e maior capacidade de detectar e mitigar ataques elaborados de DDoS.
- **Integração**: Funciona com Amazon CloudFront, Amazon Route 53, Elastic Load Balancing e pode ser integrado ao AWS WAF com regras personalizadas para uma proteção mais robusta.

### Serviços de Segurança da AWS

#### AWS Key Management Service (AWS KMS)
AWS KMS é um serviço que permite criar, gerenciar e usar chaves de criptografia para proteger seus dados.

- **Proteção de Dados**: Garante a segurança dos dados durante o armazenamento (criptografia em repouso) e durante a transmissão (criptografia em trânsito).
- **Gerenciamento de Chaves**: Oferece controles de acesso detalhados para gerenciamento de chaves de criptografia.
- **Controle**: Permite especificar quem pode gerenciar chaves e temporariamente desativar chaves quando necessário.

#### AWS WAF
AWS WAF é um firewall de aplicação web que protege aplicações web de ameaças comuns.

- **Funcionalidade**: Monitora e controla o tráfego de rede que chega às aplicações web.
- **Listas de Controle de Acesso**: Utiliza ACLs da web para bloquear ou permitir tráfego específico, protegendo contra solicitações mal-intencionadas.
- **Flexibilidade**: Permite configurar regras que definem quais solicitações devem ser bloqueadas ou permitidas.

#### Amazon Inspector
Amazon Inspector é um serviço que realiza avaliações automatizadas de segurança para identificar vulnerabilidades e desvios nas aplicações.

- **Avaliações Automatizadas**: Verifica automaticamente aplicações em busca de vulnerabilidades de segurança.
- **Relatórios de Segurança**: Fornece uma lista de descobertas de segurança, classificadas por nível de gravidade, com recomendações para correção.
- **Melhoria Contínua**: Ajuda a manter as práticas recomendadas de segurança, embora a responsabilidade final pela segurança recaia sobre o cliente.

#### Amazon GuardDuty
Amazon GuardDuty é um serviço de detecção de ameaças que protege sua infraestrutura AWS e recursos monitorando atividades suspeitas.

- **Monitoramento Contínuo**: Analisa logs de fluxo de VPC, logs de DNS e outros sinais para detectar atividades suspeitas.
- **Detecção Inteligente de Ameaças**: Utiliza aprendizado de máquina e inteligência de ameaças para identificar comportamentos anormais.
- **Resposta Automatizada**: Integra-se com AWS Lambda para permitir ações automáticas em resposta a descobertas de segurança.


## Teste de Conhecimento:

#### 1: Quais são os quatro principais fatores que você deve considerar ao escolher uma região?
R: Latência, preço, disponibilidade de serviços e conformidade
#### 2: Qual das opções a seguir melhor descreve a relação entre regiões, zonas de disponibilidade e datacenters?
R: As regiões são clusters de zonas de disponibilidade. As zonas de disponibilidade são clusters de datacenters.
#### 3: Qual das opções a seguir é um benefício da computação em nuvem?**
R: Obtenha alcance global em minutos
#### 4: Quais das opções a seguir são uma prática recomendada ao proteger um usuário raiz da AWS? (Selecione DUAS.)
R1: Habilitar multi-factor authentication (MFA) para o usuário raiz
R2: Desabilitar ou excluir as chaves de acesso associadas ao usuário raiz
#### 5: Quais tarefas são responsabilidades dos clientes? (Selecione DUAS opções.)
R1: Aplicação de patches em software em instâncias do Amazon EC2
R2: Definição de permissões para objetos do Amazon S3
#### 6: Você está configurando políticas de controle de serviço (SCPs) no AWS Organizations. A quais identidades e recursos as SCPs podem ser aplicadas? (Selecione DUAS opções.)
R1: Uma conta de membro individual
R2: Uma unidade organizacional (UO)
#### 7: Quais tarefas você pode concluir no AWS Artifact? (Selecione DUAS opções.)
R1: Acessar relatórios de conformidade da AWS sob demanda.
R2: Analisar, aceitar e gerenciar seus contratos com a AWS.
#### 8: Qual afirmativa descreve melhor uma política do IAM?
R: Um documento que concede ou nega permissões para serviços e recursos AWS
#### 9: Um funcionário precisa de acesso temporário para criar vários buckets do Amazon S3. Qual opção seria a melhor escolha para essa tarefa?
R: Função do IAM
#### 10: Qual afirmativa melhor descreve o princípio de menor privilégio?
R: Conceder apenas as permissões necessárias para executar tarefas específicas
#### 11: Qual serviço ajuda a proteger suas aplicações contra ataques distribuídos de negação de serviço (DDoS)?
R: AWS Shield
#### 12: Qual tarefa o AWS Key Management Service (AWS KMS) pode executar?
R: Criar chaves de criptografia.

# Módulo 7: Monitoramento e Análise

## Amazon CloudWatch

O **Amazon CloudWatch** é um serviço que oferece monitoramento e gerenciamento de métricas para recursos da AWS e aplicações executadas na Amazon Web Services. Ele coleta dados de monitoramento na forma de métricas, oferecendo insights operacionais de seus recursos AWS.

### Métricas

As métricas são pontos de dados que representam o desempenho de seus recursos. Os serviços AWS automaticamente enviam essas métricas para o CloudWatch, permitindo que você visualize e analise gráficos para entender como o desempenho mudou ao longo do tempo.

### Alarmes do CloudWatch

Você pode criar **alarmes** no CloudWatch para acionar ações automáticas se a métrica ultrapassar ou ficar abaixo de um limite definido. Por exemplo:

- **Cenário de Uso**: Suponha que instâncias do Amazon EC2 sejam usadas para desenvolvimento ou teste e ocasionalmente não sejam interrompidas pelos desenvolvedores, gerando custos desnecessários.
- **Solução**: Um alarme do CloudWatch pode ser configurado para interromper automaticamente uma instância do EC2 quando a utilização da CPU ficar abaixo de um limite específico por um período definido.
- **Notificações**: Você também pode optar por receber notificações quando esse alarme for acionado.

### Painel do CloudWatch

O **painel** do CloudWatch permite acessar e visualizar métricas de todos os seus recursos AWS em um único local. Você pode:

- Monitorar métricas como a utilização da CPU de instâncias EC2, o número de solicitações a um bucket do Amazon S3, entre outras.
- Personalizar painéis para diferentes necessidades comerciais, aplicativos ou recursos, facilitando a gestão e o monitoramento de operações específicas.


O CloudWatch é essencial para o monitoramento em tempo real e a automação de tarefas baseadas em métricas específicas, ajudando a otimizar o desempenho e reduzir custos operacionais.


# AWS CloudTrail

**AWS CloudTrail** é um serviço que registra chamadas de API na sua conta AWS, fornecendo detalhes como identidade do chamador, horário da chamada, endereço IP do chamador, entre outros. Esse log de ações ajuda você a monitorar e revisar as atividades dentro de sua infraestrutura AWS.

## Características Principais

- **Registros Detalhados**: Cada evento registrado inclui informações detalhadas sobre a ação executada.
- **Tempo de Atualização**: Os eventos geralmente são disponibilizados no CloudTrail em até 15 minutos após as chamadas de API.
- **Filtros de Pesquisa**: Permite a filtragem de eventos por data, usuário, tipo de recurso e outras especificações.

## Exemplo Prático

### Caso de Uso
Suponha que uma chamada de API no IAM criou um usuário chamado Mary. Usando o CloudTrail, você pode descobrir quem criou o usuário, quando e através de qual método.

### Resultados do CloudTrail
O registro no CloudTrail mostra que, em 1º de janeiro de 2020, às 9:00, o usuário do IAM John utilizou o console da AWS para criar o usuário Mary.

## CloudTrail Insights

Este recurso adicional permite a detecção automática de atividades de API incomuns, ajudando a identificar e responder a operações atípicas, como um número anormal de instâncias EC2 sendo iniciadas.

# AWS Trusted Advisor

**AWS Trusted Advisor** é um serviço que oferece orientações para otimizar recursos da AWS, melhorar a segurança e aumentar a eficiência operacional, baseando-se nas melhores práticas da AWS.

## Funcionalidades

- **Categorias de Análise**:
  - Otimização de custos
  - Desempenho
  - Segurança
  - Tolerância a falhas
  - Limites de serviço

- **Relatórios e Recomendações**: Fornece recomendações de ações e recursos para melhorar a configuração e performance dos seus recursos AWS.

## Painel do AWS Trusted Advisor

O painel no console AWS mostra uma visão geral das verificações e suas categorias:

- **Verificações Verdes**: Indicam configurações sem problemas detectados.
- **Investigações Laranjas**: Recomendam análise mais detalhada.
- **Ações Vermelhas**: Sugerem intervenções imediatas para resolver questões críticas.

### Benefícios

O AWS Trusted Advisor pode ser utilizado tanto para novos projetos e fluxos de trabalho quanto para a melhoria contínua de aplicações e recursos existentes, proporcionando um ambiente otimizado e seguro.

### Teste de conhecimento
#### 1. Quais tarefas você pode executar usando o AWS CloudTrail? (Selecione DUAS opções.)
R1: Rastrear atividades do usuário e solicitações de API em toda a infraestrutura da AWS
R2: Filtrar logs para auxiliar na análise operacional e na solução de problemas

#### 2. Quais ações você pode executar usando o Amazon CloudWatch? (Selecione DUAS opções.)
R1: Monitorar a utilização e o desempenho de seus recursos
R2: Acessar métricas em um único painel
#### 3. Qual serviço permite que você reveja a segurança de seus buckets do Amazon S3 verificando permissões de acesso aberto?
R: AWS Trusted Advisor
#### 4. Quais categorias estão inclusas no painel do AWS Trusted Advisor? (Selecione DUAS opções.)
R1: Desempenho
R2: Tolerância a falhas

OBS: Essas são as categorias:
  - Otimização de custos
  - Desempenho
  - Segurança
  - Tolerância a falhas
  - Limites de serviço


# Módulo 8: Definição de Preços e Suporte

### Nível Gratuito da AWS

O nível gratuito da AWS permite que você experimente determinados serviços da AWS sem custos, de acordo com três tipos de ofertas: Sempre gratuito, 12 meses gratuitos e Versões de teste. Este nível é ideal para novos clientes que querem testar os serviços AWS antes de se comprometerem financeiramente.

#### Sempre Gratuito

Ofertas que não expiram e estão disponíveis para todos os clientes AWS. Exemplos incluem:

- **AWS Lambda**: Até 1 milhão de solicitações gratuitas e 3,2 milhões de segundos de tempo de computação por mês.
- **Amazon DynamoDB**: 25 GB de armazenamento gratuito por mês.

#### 12 Meses Gratuitos

Estas ofertas são válidas por 12 meses a partir da sua inscrição na AWS e incluem:

- **Amazon S3 Standard**: Quantidades específicas de armazenamento gratuito.
- **Amazon EC2**: Limites para horas mensais de tempo de computação gratuito.
- **Amazon CloudFront**: Quantidades de transferência de dados gratuitos para fora.

#### Versões de Teste

Testes gratuitos de curto prazo que começam na data de ativação de um serviço específico. A duração do teste varia conforme o serviço:

- **Amazon Inspector**: Versão gratuita de 90 dias.
- **Amazon Lightsail**: 750 horas de uso gratuito em um período de 30 dias.

#### Benefícios

O nível gratuito da AWS é uma excelente forma de aprender sobre os serviços da AWS sem pressão financeira, proporcionando a empresas e desenvolvedores uma oportunidade de testar e entender melhor a plataforma antes de fazer qualquer investimento significativo.


### Como Funciona a Definição de Preço da AWS

A AWS utiliza um modelo de pagamento conforme o uso, permitindo flexibilidade e controle de custos para seus usuários. Abaixo estão descritas as três principais categorias de definição de preço na AWS.

#### Pague somente pelo que usar

- **Descrição**: Os usuários pagam apenas pelos recursos que usam, sem necessidade de contratos de longo prazo ou licenciamento complexo. Isso aplica-se a todos os serviços AWS, onde você paga conforme o consumo real de recursos como CPU, armazenamento e transferência de dados.

#### Pague menos ao fazer reserva

- **Descrição**: Ao reservar recursos, como instâncias do Amazon EC2 para usos prolongados, os usuários podem obter descontos significativos em comparação ao preço de instâncias sob demanda.
- **Exemplo**: Utilizar o Amazon EC2 Instance Savings Plans pode resultar em economias de até 72% em comparação com a capacidade equivalente da instância sob demanda para cargas de trabalho contínuas.

#### Pague menos com descontos baseados em volume, quando usar mais

- **Descrição**: A definição de preço da AWS também oferece descontos baseados no volume de uso, onde o custo unitário pode diminuir à medida que o consumo aumenta.
- **Exemplo**: O custo por GB de armazenamento usado no Amazon S3 é reduzido progressivamente com o aumento do volume de dados armazenados.

### Calculadora de Preços da AWS

A Calculadora de Preços da AWS permite aos usuários explorar e estimar os custos dos serviços AWS para seus casos de uso específicos. As estimativas podem ser organizadas por grupos, refletindo a estrutura organizacional, e depois compartilhadas através de links.

- **Funcionalidade**: Inserir detalhes como tipo de sistema operacional, requisitos de memória e de entrada/saída para obter comparações estimadas de custos entre diferentes tipos de instâncias EC2 e regiões AWS.

### Exemplos de Definição de Preços da AWS

- **AWS Lambda**: Se o uso estiver abaixo do nível gratuito, como 680 solicitações com uma duração total de 255 segundos, não há custos.
- **Amazon EC2**: Se os recursos utilizados estiverem dentro dos limites do nível gratuito, como uma instância em execução por 107 horas e 11 GB de EBS, não há custos.
- **Amazon S3**: Uso exemplificado em duas regiões com diferentes níveis de solicitações e uso de armazenamento, todas abaixo dos limites do nível gratuito, resultando em nenhum custo.


### Painel de Cobrança da AWS
Este painel é uma ferramenta essencial para monitorar, analisar e controlar os custos associados ao uso de serviços da AWS.

#### Acessando o Painel de Faturamento

- **Localização**: Acesse a aba de pesquisa e procure por 'faturamento' ou 'billing'.
- **Funcionalidades**: O painel de faturamento oferece um resumo das atividades financeiras, incluindo:
  - Previsão total para o mês atual.
  - Saldo atual dos gastos.
  - Movimento de tendência em relação ao mês anterior.
  
#### Detalhes do Painel

- **Serviços Ativos**: O painel mostra a quantidade de serviços ativos e o número de contas que você pode consolidar.
- **Regiões Ativas**: Total de regiões ativas para a sua conta.
- **Ranking de Gastos**: Visualização dos serviços que mais consomem recursos, com destaque para o Amazon SageMaker.

#### Tendências e Análises

- **Custos dos Principais Serviços**: Análise da tendência de custos pelos cinco principais serviços.
- **Linha do Tempo de Gastos**: Observação dos gastos dos últimos três meses e comparação com a média dos três meses anteriores.

#### Faturas Detalhadas

- **Acesso às Faturas**: Clique em 'faturas' para ver detalhes de um mês específico.
  - Resumo da fatura.
  - Quantidade de dólares gastos.
  - Informações de pagamento.
  - Gastos específicos por serviço.

#### Recursos Adicionais do Painel de Faturamento e Gerenciamento de Custos

- **Funcionalidades Adicionais**:
  - Compare o saldo atual do mês com o mês anterior e obtenha uma previsão para o próximo mês.
  - Visualize os gastos acumulados do mês por serviço.
  - Acesse o Cost Explorer para análises mais profundas e crie orçamentos.
  - Adquira e gerencie Savings Plans.
  - Publique relatórios de uso e custo.



### Cobrança Consolidada na AWS
Com a cobrança consolidada, gerenciar várias contas AWS se torna mais simples e econômico, permitindo uma gestão mais eficaz dos recursos e custos em uma organização grande.


#### AWS Organizations e Cobrança Consolidada

- **Descrição**: AWS Organizations permite gerenciar várias contas AWS, oferecendo a opção de cobrança consolidada.
- **Vantagem Principal**: Em vez de receber múltiplas faturas para cada conta, você recebe uma única fatura consolidada, facilitando o controle e a gestão financeira.

#### Funcionamento da Cobrança Consolidada

- **Faturas Únicas**: Todas as despesas das contas vinculadas são consolidadas em uma única fatura para o proprietário da organização.
- **Transparência**: Você pode visualizar detalhadamente o quanto foi gasto por cada conta vinculada, centralizando a informação e facilitando a análise de custos.

#### Benefícios da Cobrança Consolidada

- **Economia Compartilhada**: O uso acumulado no nível da organização pode resultar em descontos por volume.
- **Compartilhamento de Recursos**: Recursos como Saving Plans ou instâncias reservadas para EC2 podem ser compartilhados entre as contas na organização.
- **Custo Zero para o Recurso**: Utilizar a cobrança consolidada é um serviço gratuito dentro do AWS Organizations.

#### Exemplo de Implementação

1. **Criação da Organização**:
   - Adicione múltiplas contas AWS sob uma conta principal.
   - Gerencie todas as contas através de uma interface centralizada.

2. **Faturamento Consolidado**:
   - Receba os encargos de todas as contas vinculadas na fatura da conta principal.
   - Inclui detalhes de cada conta para uma visão clara do consumo.

3. **Compartilhamento de Benefícios**:
   - Combine o uso de todas as contas para obter preços mais baixos com base em descontos por volume.


### AWS Budgets

O AWS Budgets é uma ferramenta que permite criar orçamentos para gerenciar o uso do serviço, os custos associados e as reservas de instâncias dentro da AWS. Possui uma interface detalhada que permite explorar diversas configurações e opções, acessível através do painel de gestão do AWS.

#### Atualizações e Precisão

- **Frequência de Atualização**: As informações no AWS Budgets são atualizadas três vezes ao dia, o que permite monitorar com precisão o uso em relação aos valores orçados.
- **Utilidade**: Ajuda a manter o uso dentro dos limites desejados ou dos limites do nível gratuito da AWS.

#### Alertas Personalizados

- **Função**: Você pode definir alertas personalizados que notificarão você quando o uso estiver próximo ou ultrapassar o valor orçado.
- **Exemplo de Configuração de Alerta**: Se o orçamento para o Amazon EC2 for de USD 200 por mês, é possível configurar um alerta para ser notificado quando o uso atingir USD 100.

#### Uso Prático do AWS Budgets

- **Exemplo de Uso**: Ao definir um orçamento para o Amazon EC2, você pode ser proativo na gestão dos custos, evitando surpresas no final do mês.
- **Configuração de Alertas**: Esses alertas permitem uma resposta rápida a mudanças inesperadas no uso, assegurando que as decisões sobre gastos possam ser ajustadas em tempo real.



### AWS Cost Explorer

O AWS Cost Explorer é uma ferramenta analítica projetada para ajudar você a visualizar, interpretar e gerenciar os custos e o uso dos serviços AWS ao longo do tempo.

#### Funcionalidades

- **Relatório Padrão**: Inclui um relatório dos custos e do uso dos cinco principais serviços da AWS que mais acumulam custos.
- **Personalização**: Permite a aplicação de filtros e grupos personalizados para analisar dados de maneira mais específica.
  - **Exemplo de Análise**: Possibilidade de exibir o uso de recursos no nível por hora para uma análise mais detalhada.

#### Exemplo de Uso do AWS Cost Explorer

- **Painel**: Um exemplo típico de painel do AWS Cost Explorer mostra os custos mensais para instâncias do Amazon EC2 durante um período de seis meses.
  - **Visualização de Custos**: As barras em um gráfico podem separar os custos por tipos diferentes de instâncias do Amazon EC2, como t2.micro ou m3.large.
  - **Análise de Custos**: Permite a você fazer uma avaliação dos custos da AWS ao longo do tempo, o que ajuda a tomar decisões informadas sobre custos futuros e planejamento orçamentário.

#### Implicações para a Gestão de Custos

- **Planejamento Orçamentário**: A análise detalhada oferecida pelo AWS Cost Explorer auxilia no planejamento orçamentário, permitindo ajustes proativos nas estratégias de uso e alocação de recursos.
- **Decisões Estratégicas**: As visualizações e os relatórios gerados podem fundamentar decisões estratégicas, otimizando gastos e melhorando a eficiência operacional.

### Planos do AWS Support

A AWS oferece uma variedade de planos de suporte para atender às necessidades de diferentes tipos de usuários, desde pequenas startups até grandes empresas.

#### Basic Support
- **Disponibilidade**: Gratuito para todos os clientes da AWS.
- **Inclusões**: Acesso a documentação, whitepapers, fóruns de suporte, AWS Trusted Advisor (limitado), e AWS Personal Health Dashboard.

#### Developer Support
- **Ideal para**: Empresas experimentando com a AWS ou configurando testes.
- **Benefícios**: Suporte por email com tempo de resposta de 24 horas para questões gerais e menos de 12 horas para sistemas críticos danificados.

#### Business Support
- **Indicado para**: Empresas que operam cargas de trabalho de produção.
- **Tempo de Resposta**: 4 horas para sistemas de produção danificados e 1 hora para sistemas inoperantes.
- **Extras**: Acesso completo ao Trusted Advisor, suporte direto por telefone e gestão de eventos de infraestrutura por uma taxa extra.

#### Enterprise On-Ramp
- **Recomendado para**: Empresas migrando cargas de trabalho críticas.
- **Tempo de Resposta**: 30 minutos para questões críticas.
- **Gerenciamento**: Acesso a gerentes técnicos de contas (TAMs) para orientação proativa.

#### Enterprise Support
- **Projetado para**: Empresas executando cargas de trabalho de missão crítica.
- **Tempo de Resposta**: 15 minutos para questões críticas.
- **Suporte**: TAM designado, avaliações proativas, workshops e análises detalhadas.

#### Suporte de Concierge
- **Incluído em**: Planos Enterprise.
- **Funções**: Os TAMs fornecem gerenciamento de eventos de infraestrutura, análises da Well-Architected e análises de operações.

### Nota sobre TAMs
- Os TAMs são parte integral dos planos Enterprise, oferecendo orientação especializada para otimizar o uso de recursos da AWS e suporte personalizado conforme as necessidades do negócio.

### AWS Marketplace

O AWS Marketplace é um catálogo digital que oferece milhares de softwares de provedores independentes, permitindo que você encontre, teste e compre soluções de software prontas para uso na AWS.

#### Informações Disponíveis
- **Detalhes do Produto**: Informações sobre preços, suporte e avaliações de clientes.
- **Exploração por Setor e Caso de Uso**: Soluções específicas para diferentes indústrias, como saúde, com casos de uso detalhados.

#### Categorias do AWS Marketplace
- **Software de Infraestrutura**: Ferramentas para gerenciar e configurar infraestrutura de TI.
- **DevOps**: Soluções para desenvolvimento de aplicações, monitoramento e teste.
- **Produtos de Dados**: Ferramentas para gerenciamento e análise de dados.
- **Serviços Profissionais**: Consultoria e outros serviços profissionais para ajudar na implementação e gestão de tecnologias.
- **Aplicações de Negócios**: Software para operações de negócios como ERP, CRM, etc.
- **Machine Learning**: Modelos e ferramentas para implementar e gerenciar soluções de aprendizado de máquina.
- **Indústrias**: Soluções especializadas para setores específicos, como saúde, educação, e finanças.
- **Internet das Coisas (IoT)**: Produtos voltados para o desenvolvimento e gestão de dispositivos IoT.

#### Como Usar
- **Busca e Filtragem**: Pesquise produtos diretamente relacionados ao seu setor ou necessidade específica.
- **Avaliações e Preços**: Consulte as avaliações de outros usuários e compare as opções de preço para encontrar a melhor solução.

### Exemplos Práticos
- **Saúde**: Implementar soluções para proteção de prontuários de pacientes ou utilizar machine learning para prever riscos de saúde.
- **DevOps**: Encontrar ferramentas de automação para desenvolvimento e teste de aplicações.



### Teste de Conhecimento
#### 1. O nível gratuito da AWS inclui ofertas que ficam disponíveis para novos clientes AWS por um determinado período após a data de cadastro da AWS. Qual é a duração deste período?
R: 12 meses

#### 2. Qual plano do Support inclui todas as verificações do AWS Trusted Advisor pelo menor custo?
R: Business
#### 3. Qual ação você pode executar com a cobrança consolidada?
R: Combinar o uso entre contas para obter descontos de preços por volume.
#### 4. Qual ferramenta de definição de preço é usada para visualizar, entender e gerenciar o custo e o uso da AWS ao longo do tempo?
R: AWS Cost Explorer
#### 5. Qual ferramenta de preços permite receber alertas quando o uso do serviço excede um limite que você definiu?
R: AWS Budgets
#### 6. Sua empresa deseja ter suporte de um technical account manager (TAM) da AWS. Qual plano de suporte você deve escolher?
R: Empresarial de Grande Porte

#### 7. Qual serviço ou recurso é usado para encontrar software de terceiros que pode ser executado na AWS?
R: AWS Marketplace

# Módulo 9: Migração e Inovação
### AWS Cloud Adoption Framework (AWS CAF)

O AWS Cloud Adoption Framework ajuda as organizações a planejar e realizar a migração para a nuvem. O framework divide a adoção da nuvem em seis perspectivas principais, que abrangem tanto aspectos técnicos quanto de negócios.


### Utilizando o AWS CAF
O AWS CAF fornece um roteiro estruturado para organizações que buscam migrar para a nuvem, ajudando a identificar as áreas de mudança necessárias, planejar ações e mobilizar recursos adequados.

### Perspectivas do AWS CAF
#### Perspectiva de Negócio
- **Objetivo**: Alinhar as estratégias de TI e de negócios.
- **Participantes**: Gerentes de negócios, financeiros, proprietários de orçamento e stakeholders de estratégia.
- **Atividades**: Desenvolver casos de negócio para adoção da nuvem e alinhar metas de negócios e TI.

#### Perspectiva de Pessoas
- **Objetivo**: Gerenciar mudanças organizacionais para suportar a transformação para a nuvem.
- **Participantes**: Recursos humanos, equipe de gestão de pessoas.
- **Atividades**: Avaliar e desenvolver novas competências, treinamentos e mudanças organizacionais necessárias.

#### Perspectiva de Governança
- **Objetivo**: Alinhar estratégias de TI à estratégia de negócios e gerenciar riscos.
- **Participantes**: CIOs, gerentes de programas, arquitetos empresariais, analistas de negócios e gerentes de portfólio.
- **Atividades**: Atualizar habilidades, processos e governança para gerenciamento na nuvem.

#### Perspectiva de Plataforma
- **Objetivo**: Orientar a migração e implementação de soluções na nuvem.
- **Participantes**: CTOs, gerentes de TI, arquitetos de soluções.
- **Atividades**: Definir arquiteturas de sistemas, modelos e comunicação de estrutura de TI.

#### Perspectiva de Segurança
- **Objetivo**: Garantir que os objetivos de segurança sejam atingidos com visibilidade, controle, auditoria e agilidade.
- **Participantes**: CISOs, gerentes de segurança de TI, analistas de segurança.
- **Atividades**: Estruturar e implementar controles de segurança que atendam às necessidades organizacionais.

#### Perspectiva de Operações
- **Objetivo**: Gerenciar e operacionalizar cargas de trabalho de TI na nuvem.
- **Participantes**: Gerentes de operações de TI, gerentes de suporte de TI.
- **Atividades**: Definir e alinhar procedimentos operacionais e treinamentos para suportar operações na nuvem.


### Seis Estratégias de Migração para a Nuvem

Quando uma organização considera migrar aplicações para a nuvem, ela pode escolher entre seis estratégias principais. Cada estratégia de migração oferece diferentes benefícios e deve ser escolhida com base nos objetivos específicos de negócio e nas características técnicas das aplicações envolvidas.

#### Redefinir Hospedagem
- **Também conhecida como**: Lift-and-shift.
- **Descrição**: Consiste em mover aplicações para a nuvem sem fazer alterações na arquitetura. 
- **Caso de uso**: Ideal para empresas que desejam migrar rapidamente e a um custo menor.

#### Redefinir Plataforma
- **Também conhecida como**: Lift, tinker and shift.
- **Descrição**: Envolve pequenas otimizações na nuvem para melhorar a eficiência sem modificar a arquitetura central.
- **Caso de uso**: Útil para aplicações que se beneficiam de otimizações específicas de nuvem sem a necessidade de uma reformulação completa.

#### Refatorar/Rearquitetura
- **Descrição**: Reimaginar como uma aplicação é arquitetada utilizando recursos nativos da nuvem para melhorar funcionalidades, escalabilidade ou performance.
- **Caso de uso**: Recomendada para aplicações que precisam de melhorias significativas que não são possíveis em sua forma atual.

#### Recomprar
- **Descrição**: Substituição de aplicações existentes por versões comerciais disponíveis como SaaS.
- **Caso de uso**: Aplicável quando substituir aplicações antigas por soluções SaaS modernas traz benefícios como redução de custos e aumento de eficiência.

#### Reter
- **Descrição**: Manter certas aplicações no ambiente atual devido a restrições de refatoração ou prioridades de negócios.
- **Caso de uso**: Adequado para aplicações críticas que exigem uma transformação significativa ou que não oferecem retorno imediato se migradas.

#### Retirar
- **Descrição**: Eliminação de aplicações obsoletas ou desnecessárias.
- **Caso de uso**: Ideal para simplificar o ambiente de TI e reduzir custos ao descontinuar aplicações que não agregam valor.



### AWS Snow Family

A AWS Snow Family é uma série de dispositivos físicos projetados para facilitar o transporte físico de grandes volumes de dados para dentro e para fora da AWS. Abaixo, detalham-se os dispositivos que compõem esta família.

#### AWS Snowcone
- **Descrição**: O Snowcone é o menor membro da Snow Family, projetado para ser portátil e robusto, facilitando o transporte de dados em locais com limitações de espaço e conectividade.

#### AWS Snowball
- **Descrição**: O Snowball é um dispositivo de tamanho médio dentro da Snow Family que permite transferir grandes quantidades de dados de e para a nuvem da AWS. Existem versões específicas que suportam tarefas computacionais locais enquanto movimentam dados.

#### AWS Snowmobile
- **Descrição**: O Snowmobile é um serviço massivo de transferência de dados que pode acomodar até 100 petabytes por unidade. Consiste em um contêiner de 13,71 metros de comprimento montado em um caminhão semirreboque, ideal para mover enormes volumes de dados para a nuvem AWS em uma única viagem.

### Funcionalidades Comuns
- **Segurança e Gerenciamento**: Todos os dispositivos da Snow Family incorporam recursos avançados de segurança, monitoramento e gerenciamento da AWS.
- **Capacidade**: Varia de pequenas quantidades de dados com o Snowcone até exabytes com o Snowmobile, atendendo a diferentes necessidades e escalas de dados.
- **Propriedade e Gestão**: A AWS é responsável pela manutenção, gestão e segurança de todos os dispositivos da Snow Family.

### Utilização
- **Cenários de uso**: Os dispositivos são usados para migração de dados em massa, recuperação de desastres, conteúdo digital em larga escala, transferência de dados de pesquisa científica, entre outros.
- **Integração com a AWS**: Integrados plenamente com a AWS para oferecer uma solução coesa de transferência de dados e computação.

Esses dispositivos são projetados para resolver desafios específicos de transferência de dados em ambientes com limitações de conectividade ou grandes volumes de dados.

### Inove com os serviços da AWS

A AWS oferece uma ampla gama de serviços que permitem inovações significativas nas áreas de computação em nuvem, machine learning e inteligência artificial. Abaixo, você encontrará um resumo das possibilidades oferecidas pela AWS para fomentar a inovação em diferentes setores.

#### Aplicações sem servidor
- **Descrição**: Com a AWS, adotar aplicações sem servidor significa que não é necessário gerenciar, provisionar ou administrar servidores. A AWS gerencia a disponibilidade e a tolerância a falhas automaticamente.
- **Exemplo de Serviço**: AWS Lambda permite executar códigos sem a necessidade de gerenciar servidores, otimizando o foco dos desenvolvedores nas funcionalidades principais do produto em vez da infraestrutura.

#### Machine learning
- **Descrição**: O desenvolvimento de machine learning pode ser complexo e oneroso, mas a AWS simplifica esse processo com o Amazon SageMaker, que facilita a criação, o treinamento e a implantação de modelos de machine learning.
- **Benefícios**: Utilizando o machine learning, é possível analisar grandes volumes de dados, resolver problemas complexos e prever eventos futuros com maior precisão.

#### Inteligência artificial
- **Descrição**: A AWS disponibiliza uma série de serviços que utilizam inteligência artificial para oferecer soluções avançadas em diversas aplicações.
- **Serviços de IA**:
  - **Amazon CodeWhisperer**: Fornece sugestões de código inteligentes baseadas em comentários em inglês, padrões de código e práticas de segurança, incluindo os padrões do Open Worldwide Application Security Project e as melhores práticas de segurança da AWS.
  - **Amazon Transcribe**: Converte fala em texto.
  - **Amazon Comprehend**: Analisa padrões em textos.
  - **Amazon Fraud Detector**: Identifica atividades potencialmente fraudulentas.
  - **Amazon Lex**: Facilita a criação de chatbots interativos de voz e texto.

#### VMware Cloud na AWS
- **Descrição**: A infraestrutura VMware pode ser executada na AWS, permitindo uma migração suave e integrada das aplicações locais para a nuvem sem a necessidade de reformular as arquiteturas existentes.

#### AWS Ground Station
- **Descrição**: Para organizações interessadas em operações espaciais, o AWS Ground Station permite controlar satélites e processar dados espaciais na nuvem, pagando apenas pelo tempo de uso efetivo.

#### Outros destaques
- **AWS DeepRacer**: Uma plataforma experimental para desenvolvedores testarem técnicas de aprendizado por reforço em um ambiente de corrida lúdico.
- **Internet das Coisas (IoT)**: Ferramentas e serviços que permitem a comunicação e gestão de dispositivos IoT globalmente.


### Treinamento e Certificação AWS
- **Descrição**: O AWS Training & Certification oferece cursos e certificações que ajudam a manter os profissionais atualizados com as mais recentes tecnologias e melhores práticas recomendadas pela AWS.

### Amazon CodeWhisperer

Amazon CodeWhisperer é uma ferramenta de inteligência artificial para desenvolvimento de software que auxilia os desenvolvedores a escrever código mais eficiente e seguro. Aqui estão os principais benefícios e funcionalidades do Amazon CodeWhisperer:

#### Características Principais
- **Completar Código**: Utiliza processamento de linguagem natural para entender comentários e gerar código correspondente, facilitando a escrita de funções e blocos de código completos.
- **Análise de Contexto**: Ajusta sugestões de código para se alinhar ao estilo de codificação e às convenções de nomenclatura do projeto atual.
- **Verificação de Segurança**: Avalia o código contra padrões de segurança reconhecidos, como os do Open Worldwide Application Security Project, e práticas recomendadas de segurança da AWS.

#### Benefícios para Desenvolvedores
- **Automatização de Tarefas Repetitivas**: Simplifica o desenvolvimento ao automatizar tarefas repetitivas, economizando tempo dos desenvolvedores.
- **Aprendizado de Novas Linguagens**: Reduz a necessidade de dedicar horas para aprender novas linguagens, permitindo que os desenvolvedores utilizem sugestões de código adaptadas ao seu estilo.
- **Qualidade e Eficiência**: Garante a entrega de código de alta qualidade, ajudando a construir aplicações mais robustas e eficientes.

#### Segurança e Conformidade
- **Mitigação de Vulnerabilidades**: Ajuda a identificar e mitigar vulnerabilidades de segurança, protegendo a integridade da base de código.
- **Atualizações Contínuas**: Mantém as aplicações seguras e atualizadas com as últimas práticas de segurança.

#### Impacto Organizacional
- **Aceleração do Desenvolvimento**: Permite uma entrega mais rápida de soluções de software ao acelerar o processo de desenvolvimento.
- **Foco em Inovação**: Libera os desenvolvedores para se concentrarem em aspectos mais críticos do projeto, potencializando a inovação.

Para mais informações sobre como integrar e maximizar o uso do Amazon CodeWhisperer em seus projetos de desenvolvimento, visite a página oficial ou os recursos de aprendizado relacionados.


Estas são apenas algumas das inovações que a AWS oferece, cada uma com potencial para transformar setores e acelerar o desenvolvimento de novas soluções tecnológicas.


### Teste de Conhecimento
#### 1. Qual perspectiva do AWS Cloud Adoption Framework ajuda você a elaborar, implementar e otimizar sua infraestrutura da AWS com base em suas metas e perspectivas de negócio?
R: Perspectiva de plataforma
#### 2. Qual estratégia de migração envolve a mudança para um produto diferente?
R: Recomprar
#### 3. Qual é a capacidade de armazenamento do Snowball Edge Storage Optimized?
R: 80 TB
#### 4. Qual serviço ajuda você a criar, treinar e implantar rapidamente modelos de machine learning?
R: Amazon SageMaker



# Módulo 10: A Jornada para a Nuvem

# Módulo 11: Noções Básicas do AWS Certified Cloud Practitioner
