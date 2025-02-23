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





## Módulo 1: Introdução à Amazon Web Services (AWS)

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




## Segurança e o modelo de responsabilidade compartilhada da AWS

Quando você usa a AWS, a segurança é uma responsabilidade compartilhada entre você e a AWS. Isso é conhecido como o "modelo de responsabilidade compartilhada," dividido em dois conceitos:

![image](https://github.com/user-attachments/assets/f6bf140b-c64d-49b1-8e2f-4b31bb95a782)


1. **Segurança *na* Nuvem (Responsabilidade da AWS)**: A AWS é responsável por proteger toda a infraestrutura que executa os serviços, incluindo:
   - Segurança física de datacenters, regiões e zonas de disponibilidade.
   - Gerenciamento de hardware, software, redes, e servidores físicos, além dos sistemas operacionais de host e camadas de virtualização.

   **Categorias de Serviços AWS e Responsabilidades da AWS:**

    1. **Serviços de Infraestrutura** (e.g., Amazon EC2)
    - **Responsabilidade AWS**: Gerenciar a infraestrutura subjacente e os serviços base.

    2. **Serviços de Contêiner** (e.g., Amazon RDS)
    - **Responsabilidade AWS**: Gerenciar a infraestrutura, serviços base, sistema operacional, e plataforma de aplicações.

    3. **Serviços Abstratos** (e.g., Amazon S3)
    - **Responsabilidade AWS**: Gerenciar a infraestrutura, sistema operacional, plataformas, criptografia do lado do servidor, e proteção de dados.

    **Observação sobre Serviços de Contêiner da AWS**: 

    Os serviços de contêiner da AWS se referem à abstração de aplicações que a AWS gerencia internamente, e não a contêineres Docker. Isso alivia a carga dos clientes em relação ao gerenciamento da plataforma e infraestrutura, ficando sob responsabilidade da AWS.


2. **Segurança *da* Nuvem (Responsabilidade do Cliente)**: Você, como cliente, é responsável por configurar e proteger os serviços e dados que utiliza. 
   - Dependendo do serviço AWS, sua responsabilidade varia: de configurar e gerenciar toda a segurança, até apenas controlar o acesso aos seus recursos e dados. 

    Portanto, sua carga de responsabilidade muda conforme o tipo de serviço AWS que você está usando.
    **Responsabilidades da AWS e do Cliente por Categoria de Serviço:**

    1. **Serviços de Infraestrutura**
    - **AWS**: Gerencia infraestrutura e serviços base.
    - **Cliente**: Gerencia sistema operacional, plataforma de aplicação, criptografia, e segurança dos dados.

    2. **Serviços de Contêiner**
    - **AWS**: Gerencia infraestrutura, serviços base, sistema operacional e plataforma de aplicação.
    - **Cliente**: Gerencia dados do cliente, implementa criptografia e segurança por meio de firewalls e backups.

    3. **Serviços Abstratos**
    - **AWS**: Gerencia infraestrutura, sistema operacional, plataformas, e criptografia do lado do servidor.
    - **Cliente**: Gerencia e protege dados do cliente, incluindo a criptografia do lado do cliente.


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



## Demonstração: implemente segurança com o AWS Identity and Access Management (IAM)

## Hospedagem de aplicação de diretório de funcionários

# Teste de Conhecimento:

**P: Quais são os quatro principais fatores que você deve considerar ao escolher uma região?**

R: Latência, preço, disponibilidade de serviços e conformidade

**P: Qual das opções a seguir melhor descreve a relação entre regiões, zonas de disponibilidade e datacenters?**

R: As regiões são clusters de zonas de disponibilidade. As zonas de disponibilidade são clusters de datacenters.

**P: Qual das opções a seguir é um benefício da computação em nuvem?**

R: Obtenha alcance global em minutos

**P: Quais das opções a seguir são uma prática recomendada ao proteger um usuário raiz da AWS? (Selecione DUAS.)**

R:  Habilitar multi-factor authentication (MFA) para o usuário raiz
    Desabilitar ou excluir as chaves de acesso associadas ao usuário raiz





---

## Módulo 2: Computação da AWS
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

## Módulo 3: Infraestrutura Global e Confiabilidade
  
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

## Módulo 4: Redes
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

## Módulo 5: Armazenamento e Bancos de Dados
*Conteúdo do módulo 5...*

## Módulo 6: Segurança
*Conteúdo do módulo 6...*

## Módulo 7: Monitoramento e Análise

## Módulo 8: Definição de Preços e Suporte

## Módulo 9: Migraçao e Inovação

## Módulo 10: A Jornada para a Nuvem

## Módulo 11: Noções Básicas do AWS Certified Cloud Practitioner
