# Lista de Recursos da AWS

A seguir, apresento uma lista organizada por grupos dos principais recursos da AWS – lembrando que a AWS possui centenas de serviços, então esta lista foca nos mais relevantes e amplamente utilizados – com uma breve descrição de sua função, ideias de uso, modelo de precificação e pontos de comparação quando aplicável.

---

## 1. Compute

### Amazon EC2 (Elastic Compute Cloud)
- **Função/Objetivo:** Provisão de máquinas virtuais (instâncias) configuráveis para hospedar aplicações.
- **Preço:** Modelo on-demand (por hora ou segundo), instâncias reservadas e spot, com variação conforme tipo de instância, região e uso de recursos.
- **Quando Utilizar:** Para aplicações que necessitam de controle total sobre o ambiente, customização e escalabilidade flexível.
- **Comparação:** Se precisar de uma abordagem sem servidor, compare com o AWS Lambda.

### AWS Lambda
- **Função/Objetivo:** Execução de código em resposta a eventos de forma serverless (sem gerenciar servidores).
- **Preço:** Cobrança baseada no número de invocações e na duração da execução (com camada gratuita generosa para muitos casos).
- **Quando Utilizar:** Quando a aplicação é orientada a eventos, com cargas variáveis e que podem se beneficiar da escalabilidade automática.
- **Comparação:** Ideal para workloads intermitentes ou pequenos, em contraste com o EC2 para cargas contínuas ou com requisitos específicos de configuração.

### AWS Elastic Beanstalk
- **Função/Objetivo:** Plataforma como Serviço (PaaS) que simplifica o deploy, o gerenciamento e a escalabilidade de aplicações web.
- **Preço:** Não há custo adicional pela própria ferramenta – você paga pelos recursos subjacentes (EC2, RDS, etc.).
- **Quando Utilizar:** Para deploy rápido de aplicações sem se preocupar com a infraestrutura detalhada.
- **Comparação:** É mais simples que gerenciar EC2 diretamente, mas com menos controle granular.

### Amazon ECS (Elastic Container Service) & EKS (Elastic Kubernetes Service)
- **Função/Objetivo:** Serviços gerenciados para orquestração de contêineres.
- **Preço:**  
  - **ECS:** Não possui cobrança própria (paga-se pelos recursos usados).  
  - **EKS:** Cobra uma taxa fixa por cluster, além dos recursos.
- **Quando Utilizar:** Para aplicações baseadas em contêineres; escolha o ECS para integração nativa com a AWS e o EKS se preferir o ecossistema Kubernetes.
- **Comparação:** ECS é mais simples para iniciantes, enquanto o EKS oferece maior flexibilidade com Kubernetes.

### AWS Fargate
- **Função/Objetivo:** Execução de contêineres sem a necessidade de gerenciar servidores, integrando-se com ECS/EKS.
- **Preço:** Cobrança baseada em recursos consumidos (vCPU e memória) durante a execução dos contêineres.
- **Quando Utilizar:** Para evitar a complexidade de provisionar e gerenciar clusters de contêineres; útil em workloads que demandam escalabilidade automática.

---

## 2. Armazenamento

### Amazon S3 (Simple Storage Service)
- **Função/Objetivo:** Armazenamento de objetos (arquivos, backups, imagens, etc.) com alta durabilidade e escalabilidade.
- **Preço:** Cobrança por GB armazenado, número de requisições e transferência de dados; variações conforme a classe de armazenamento (Standard, Intelligent-Tiering, Glacier, etc.).
- **Quando Utilizar:** Para armazenar dados estáticos, backups, arquivos de mídia e logs; ideal para distribuição via CDN com CloudFront.
- **Comparação:** Voltado para dados não estruturados, diferente do EFS ou EBS.

### Amazon EBS (Elastic Block Store)
- **Função/Objetivo:** Armazenamento em bloco para instâncias EC2, similar a discos rígidos virtuais.
- **Preço:** Cobrança baseada em GB provisionado e IOPS (para volumes otimizados) e uso de snapshots.
- **Quando Utilizar:** Para sistemas operacionais, bancos de dados e aplicações que exigem baixa latência e desempenho consistente.
- **Comparação:** Enquanto o S3 é orientado a objetos, o EBS é ligado diretamente às instâncias.

### Amazon EFS (Elastic File System)
- **Função/Objetivo:** Armazenamento de arquivos escalável e elástico, acessível por múltiplas instâncias EC2 simultaneamente.
- **Preço:** Cobrança por GB utilizado, com variações conforme o desempenho (Standard ou Infrequent Access).
- **Quando Utilizar:** Em cenários que exigem compartilhamento de arquivos entre servidores ou aplicações distribuídas.
- **Comparação:** Para armazenamento de arquivos distribuídos, o EFS supera o EBS, que é exclusivo a uma instância.

### Amazon Glacier (S3 Glacier)
- **Função/Objetivo:** Armazenamento de dados arquivísticos com custo extremamente baixo para dados acessados raramente.
- **Preço:** Cobrança por GB armazenado e taxa para recuperação de dados (mais lenta).
- **Quando Utilizar:** Para arquivamento e backup de longo prazo, onde a latência de recuperação não é crítica.

### AWS Storage Gateway
- **Função/Objetivo:** Integração entre ambientes on-premises e o armazenamento em nuvem, facilitando backups e migrações.
- **Preço:** Cobrança por gateway ativo e volume de dados transferidos.
- **Quando Utilizar:** Quando se necessita de uma ponte entre data centers locais e a AWS.

---

## 3. Bancos de Dados

### Amazon RDS (Relational Database Service)
- **Função/Objetivo:** Banco de dados relacional gerenciado para MySQL, PostgreSQL, SQL Server, Oracle e MariaDB.
- **Preço:** Cobrança por hora de instância, armazenamento provisionado, IOPS e licenciamento (quando aplicável).
- **Quando Utilizar:** Para aplicações que necessitam de bancos relacionais com alta disponibilidade, backups automáticos e escalabilidade.
- **Comparação:** Menos complexidade operacional do que gerenciar seu próprio banco em EC2.

### Amazon DynamoDB
- **Função/Objetivo:** Banco de dados NoSQL gerenciado com baixa latência e escalabilidade automática.
- **Preço:** Modelo de cobrança baseado em capacidade provisionada (ou on-demand) e armazenamento, com custos adicionais para backups e streams.
- **Quando Utilizar:** Para aplicações que exigem alta performance em leitura/gravação e que podem se beneficiar da escalabilidade horizontal.
- **Comparação:** Ideal quando a estrutura dos dados é não relacional e os requisitos de performance são intensos.

### Amazon Aurora
- **Função/Objetivo:** Banco de dados relacional compatível com MySQL e PostgreSQL, otimizado para alta performance e disponibilidade.
- **Preço:** Cobrança semelhante ao RDS, com melhorias de desempenho que podem reduzir custos em cargas intensas.
- **Quando Utilizar:** Quando se necessita de desempenho superior e escalabilidade em bancos relacionais, mantendo compatibilidade com MySQL/PostgreSQL.

### Amazon Redshift
- **Função/Objetivo:** Data warehouse gerenciado para análises de grandes volumes de dados.
- **Preço:** Cobrança por nó ou por hora, dependendo da configuração e tamanho do cluster.
- **Quando Utilizar:** Para análises complexas, BI e processamento de consultas em grandes datasets.
- **Comparação:** Focado em workloads analíticos, diferentemente dos bancos transacionais.

### Amazon DocumentDB
- **Função/Objetivo:** Banco de dados de documentos compatível com APIs do MongoDB.
- **Preço:** Cobrança baseada em instância, armazenamento e I/O.
- **Quando Utilizar:** Quando se precisa de um banco de dados de documentos com gerenciamento simplificado e escalabilidade.

### Amazon ElastiCache
- **Função/Objetivo:** Serviço de cache na memória compatível com Redis e Memcached para acelerar aplicações.
- **Preço:** Cobrança por instância e uso de memória.
- **Quando Utilizar:** Para reduzir a latência e melhorar o desempenho de aplicações com alta demanda de leitura.

---

## 4. Networking e Distribuição de Conteúdo

### Amazon VPC (Virtual Private Cloud)
- **Função/Objetivo:** Criação de uma rede virtual isolada na AWS onde os recursos podem ser executados de forma segura.
- **Preço:** Sem custo adicional para a criação da VPC; cobranças ocorrem para serviços complementares (ex.: NAT gateways).
- **Quando Utilizar:** Para isolar recursos e definir regras de segurança e controle de tráfego.

### Amazon Route 53
- **Função/Objetivo:** Serviço de DNS escalável e gerenciado, com funcionalidades de roteamento e monitoramento de saúde.
- **Preço:** Cobrança por zona hospedada, consultas DNS e verificações de saúde.
- **Quando Utilizar:** Para gerenciar domínios e roteamento de tráfego global com alta disponibilidade.

### Amazon API Gateway
- **Função/Objetivo:** Criação, gerenciamento e segurança de APIs RESTful e WebSocket.
- **Preço:** Cobrança por chamadas de API, transferência de dados e funcionalidades adicionais (como caching).
- **Quando Utilizar:** Para expor funcionalidades de backend via APIs seguras e escaláveis.
- **Comparação:** Pode ser integrado com Lambda para soluções serverless.

### Amazon CloudFront
- **Função/Objetivo:** Rede de Distribuição de Conteúdo (CDN) para entrega rápida de dados, vídeos e aplicações em escala global.
- **Preço:** Cobrança por transferência de dados e número de requisições, com variação por região.
- **Quando Utilizar:** Para reduzir latência e melhorar a experiência do usuário final, distribuindo conteúdos estáticos e dinâmicos.

### AWS Direct Connect
- **Função/Objetivo:** Conexão dedicada e privada entre data centers on-premises e a AWS.
- **Preço:** Modelo baseado na largura de banda e no uso da conexão, com custos fixos mensais.
- **Quando Utilizar:** Em cenários que demandam alta largura de banda, baixa latência e conexão segura com a AWS.

---

## 5. Segurança, Identidade e Conformidade

### AWS IAM (Identity and Access Management)
- **Função/Objetivo:** Gerenciamento de usuários, permissões e políticas de acesso aos recursos da AWS.
- **Preço:** Gratuito (alguns recursos avançados podem ter custos associados, conforme integrações).
- **Quando Utilizar:** Em todos os ambientes para garantir controles de acesso e segurança.

### AWS KMS (Key Management Service)
- **Função/Objetivo:** Gerenciamento e criação de chaves de criptografia, integrando-se com outros serviços da AWS.
- **Preço:** Cobrança por chave gerenciada e uso de solicitações (chamadas) de criptografia.
- **Quando Utilizar:** Sempre que dados sensíveis precisem ser criptografados para garantir conformidade e segurança.

### AWS Shield & AWS WAF
- **Função/Objetivo:**  
  - **Shield:** Proteção contra ataques DDoS.  
  - **WAF:** Filtragem de tráfego malicioso para aplicações web.
- **Preço:**  
  - **Shield Standard:** Gratuito.  
  - **Shield Advanced e WAF:** Cobrança baseada em configuração e uso.
- **Quando Utilizar:** Para proteger aplicações críticas e garantir segurança contra ameaças externas.

---

## 6. Analytics

### Amazon EMR (Elastic MapReduce)
- **Função/Objetivo:** Processamento de big data utilizando frameworks como Hadoop, Spark e Presto de forma gerenciada.
- **Preço:** Cobrança por instância e uso do cluster (modelos on-demand ou reservados).
- **Quando Utilizar:** Para processar grandes volumes de dados e realizar análises complexas.

### Amazon Kinesis
- **Função/Objetivo:** Plataforma para processamento de streams de dados em tempo real.
- **Preço:** Cobrança por shard (unidade de capacidade) e volume de dados processados.
- **Quando Utilizar:** Em cenários de monitoramento, análise de logs ou processamento de dados em tempo real.

### Amazon Athena
- **Função/Objetivo:** Serviço de consulta interativo que permite analisar dados diretamente no S3 utilizando SQL.
- **Preço:** Cobrança baseada na quantidade de dados escaneados por consulta.
- **Quando Utilizar:** Para análises ad hoc sem a necessidade de provisionar infraestrutura.

### Amazon QuickSight
- **Função/Objetivo:** Serviço de BI (Business Intelligence) para criação de dashboards e relatórios interativos.
- **Preço:** Cobrança por usuário (mensal) e por capacidade de processamento.
- **Quando Utilizar:** Para visualizar dados de forma interativa e integrar múltiplas fontes de dados.

### AWS Glue
- **Função/Objetivo:** Serviço de ETL (Extração, Transformação e Carga) serverless para preparação de dados para análise.
- **Preço:** Cobrança baseada no tempo de execução dos jobs e nos recursos utilizados.
- **Quando Utilizar:** Para automatizar fluxos de dados entre diferentes repositórios e preparar dados para analytics.

---

## 7. Machine Learning e Inteligência Artificial

### Amazon SageMaker
- **Função/Objetivo:** Plataforma integrada para construção, treinamento e implantação de modelos de machine learning.
- **Preço:** Cobrança separada para instâncias de treinamento, armazenamento e endpoints de inferência.
- **Quando Utilizar:** Para desenvolver e implantar soluções de ML sem a necessidade de gerenciar a infraestrutura subjacente.

### Amazon Rekognition
- **Função/Objetivo:** Serviço de análise de imagens e vídeos, com detecção de objetos, faces e moderação de conteúdo.
- **Preço:** Cobrança por imagem ou por minuto de vídeo processado.
- **Quando Utilizar:** Em aplicações que necessitam de reconhecimento facial, análise de mídia ou monitoramento de conteúdo visual.

### Amazon Comprehend
- **Função/Objetivo:** Serviço de processamento de linguagem natural para extrair insights e padrões a partir de textos.
- **Preço:** Cobrança por unidade de texto analisado (tokens).
- **Quando Utilizar:** Para análise de sentimentos, extração de entidades e categorização de textos.

### Amazon Lex, Polly e Translate
- **Função/Objetivo:**  
  - **Lex:** Criação de chatbots e interfaces de conversa.  
  - **Polly:** Conversão de texto em fala (TTS).  
  - **Translate:** Tradução automática de textos.
- **Preço:** Cobrança baseada em uso (número de requisições ou caracteres processados).
- **Quando Utilizar:** Para incorporar funcionalidades de linguagem natural, atendimento automatizado e acessibilidade em aplicações.

---

## 8. Internet das Coisas (IoT)

### AWS IoT Core
- **Função/Objetivo:** Conexão e gerenciamento de dispositivos IoT com comunicação segura e escalável.
- **Preço:** Cobrança por mensagem enviada/recebida e quantidade de dispositivos conectados.
- **Quando Utilizar:** Em projetos que envolvem dispositivos conectados, automação industrial e smart devices.

### AWS IoT Greengrass
- **Função/Objetivo:** Permite que dispositivos locais executem funções de computação, armazenamento e sincronização com a nuvem.
- **Preço:** Cobrança baseada no número de dispositivos e funcionalidades utilizadas.
- **Quando Utilizar:** Quando há necessidade de processamento local e resposta em tempo real, mantendo a integração com a AWS.

### AWS IoT Analytics
- **Função/Objetivo:** Serviço para coletar, processar e analisar dados de dispositivos IoT.
- **Preço:** Cobrança por processamento e armazenamento dos dados analisados.
- **Quando Utilizar:** Para transformar dados brutos de IoT em insights acionáveis.

---

## 9. Ferramentas para Desenvolvedores e Gerenciamento

### AWS CloudFormation
- **Função/Objetivo:** Provisionamento de infraestrutura como código (IaC) para modelar e automatizar a criação de recursos AWS.
- **Preço:** Gratuito – você paga apenas pelos recursos criados.
- **Quando Utilizar:** Para versionar e replicar ambientes de forma automatizada.

### AWS CodeCommit, CodeBuild, CodeDeploy e CodePipeline
- **Função/Objetivo:** Conjunto de ferramentas para versionamento de código, integração contínua (CI), deploy e automação de pipelines de desenvolvimento.
- **Preço:** Cada serviço possui modelo de cobrança por uso (ex.: repositórios, minutos de build, etc.).
- **Quando Utilizar:** Para implementar práticas de DevOps e automatizar ciclos de desenvolvimento e entrega.

### Amazon CloudWatch
- **Função/Objetivo:** Monitoramento e logging dos recursos e aplicações na AWS, com métricas, alarmes e dashboards customizados.
- **Preço:** Cobrança por coleta de métricas, logs e dashboards; existe camada gratuita limitada.
- **Quando Utilizar:** Em qualquer ambiente que necessite de monitoramento contínuo e análise de performance.

### AWS X-Ray
- **Função/Objetivo:** Ferramenta de tracing para analisar e depurar aplicações distribuídas, identificando gargalos e erros.
- **Preço:** Cobrança por dados processados e amostragem de requisições.
- **Quando Utilizar:** Para rastrear e melhorar a performance de aplicações complexas, especialmente em arquiteturas de microsserviços.

---

## 10. Migração e Transferência

### AWS Migration Hub
- **Função/Objetivo:** Centraliza o monitoramento de migrações de aplicações, servidores e bancos de dados para a AWS.
- **Preço:** Geralmente gratuito; alguns serviços complementares podem ter cobrança.
- **Quando Utilizar:** Ao planejar e executar a migração de workloads on-premises para a nuvem.

### AWS Database Migration Service (DMS)
- **Função/Objetivo:** Migração de bancos de dados de forma contínua e segura, com mínimo downtime.
- **Preço:** Cobrança baseada no tempo de execução e recursos utilizados durante a migração.
- **Quando Utilizar:** Para migrar bases de dados para a AWS com interrupção mínima das operações.

---

## Observações Gerais

- **Preço e Modelos de Cobrança:**  
  A AWS utiliza modelos variados (on-demand, reservado, spot, pay-as-you-go) que dependem da região, tipo de recurso e padrões de uso. Recomenda-se consultar a [página de precificação da AWS](https://aws.amazon.com/pt/pricing/) para informações atualizadas.

- **Comparações e Escolha de Serviço:**  
  A decisão entre serviços (por exemplo, EC2 vs. Lambda ou RDS vs. DynamoDB) deve levar em conta requisitos de controle, performance, escalabilidade, complexidade da aplicação e perfil de custo. Cada serviço possui pontos fortes e trade-offs que variam conforme o caso de uso.

- **Atualizações Constantes:**  
  A AWS está em constante evolução, lançando novos serviços e atualizações. Mantenha-se informado consultando a documentação oficial e os anúncios da AWS.

---

Esta visão geral organizada por grupos oferece uma base sólida para entender os principais recursos disponíveis na AWS, seus objetivos, modelos de preço e quando optar por cada um.
