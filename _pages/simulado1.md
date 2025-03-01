# Simulado 1

## 1. Acesso Seguro a Recursos na AWS
**Pergunta:**  
Qual é o serviço da AWS que permite que aplicações acessem de forma segura e controlada recursos restritos de outros serviços dentro da AWS, utilizando políticas de permissões granulares e autenticação robusta?

**Resposta:**  
IAM Função/Papeis (Roles)

---

## 2. Provisionamento Automático de Instâncias
**Pergunta:**  
Um e-commerce lida, em média, com 2000 usuários diários. Em dias de aumento nas vendas, o sistema atinge picos de 3000 usuários, resultando em lentidão e, por vezes, indisponibilidade. Como automatizar o processo de provisionamento de instâncias adicionais de servidor para lidar automaticamente com essas cargas durante os períodos de pico?

**Resposta:**  
Utilizando o Auto Scaling.

---

## 3. Armazenamento de Dados de Auditoria com Baixo Custo
**Pergunta:**  
Durante a migração de sistemas, observou-se que há dados em uma aplicação que raramente são acessados e poderiam ser preservados em arquivos apenas para fins de auditoria. Qual serviço pode ser empregado para alcançar esse objetivo com o menor custo possível?

**Resposta:**  
S3 Glacier

---

## 4. Gestão de Versões de API
**Pergunta:**  
Uma aplicação disponibiliza dados por meio de APIs REST para várias aplicações externas. Considerando possíveis cenários de manutenção e evolução futuras, qual serviço pode auxiliar na gestão de múltiplas versões de uma API, garantindo a compatibilidade contínua com todos os seus consumidores?

**Resposta:**  
API Gateway

---

## 5. Criptografia para Segurança de Dados
**Pergunta:**  
A equipe de segurança da informação de uma empresa classificou um site como tendo alto risco de exposição de dados sensíveis devido à ausência de criptografia nas mensagens trocadas entre os usuários e os servidores. Qual serviço poderia ser eficaz para remediar esse problema?

**Resposta:**  
AWS Certificate Manager

---

## 6. Aceleração de Projetos com AWS IQ
**Pergunta:**  
Uma empresa deseja empregar o AWS IQ para agilizar a entrega de um projeto na nuvem. De que maneira esse serviço pode ser utilizado para atender às necessidades da empresa e acelerar o processo de implementação do projeto?

**Resposta:**  
Conectando especialistas da AWS para projetos de curto prazo.

---

## 7. Uso de Cloud com Flexibilidade e Gerenciamento
**Pergunta:**  
Utilização de recursos de rede, computadores virtuais e armazenamento de dados com alto nível de flexibilidade, gerenciamento e controle sobre os recursos de TI são características de qual tipo de uso de cloud?

**Resposta:**  
IaaS

> **Observação:** Pesquisar o que é BaaS

---

## 8. Catálogo de Aplicações de Terceiros
**Pergunta:**  
Qual serviço da AWS possui um catálogo onde os clientes podem encontrar aplicações desenvolvidas por terceiros, prontas para serem instaladas e executadas para atender as mais diversas necessidades de negócio?

**Resposta:**  
AWS Marketplace

---

## 9. Armazenamento de Arquivos com Sistema de Arquivos
**Pergunta:**  
Uma empresa está migrando parte de sua aplicação para a AWS e precisa de uma solução para armazenar arquivos que utilizam sistemas de arquivos. Qual serviço da AWS seria o mais adequado para atender a essa necessidade?

**Resposta:**  
Elastic File System (EFS)

---

## 10. Problemas de Permissão no CloudWatch
**Pergunta:**  
Após concluir os testes, homologações e implantação de uma aplicação, usuários relataram a impossibilidade de acessá-la em ambiente de produção. Na log do CloudWatch, uma mensagem de erro indica que a função Lambda enfrentou negação de acesso ao DynamoDB. Qual serviço precisa ser configurado para resolver este problema em produção?

**Resposta:**  
AWS IAM Roles

---

## 11. Organização e Armazenamento de Dados no S3
**Pergunta:**  
Quais são os componentes principais do Amazon S3 utilizados para organizar e armazenar dados? (Selecione 2 alternativas)

**Resposta:**  
- Buckets  
- Objetos

---

## 12. Endereço IP Estático e Substituição de Hosts
**Pergunta:**  
Como é possível manter a exposição constante de serviços em um mesmo endereço IP e facilitar a substituição simples dos hosts associados a esse endereço em sua infraestrutura?

**Resposta:**  
Utilizando um IP Elástico

---

## 13. Características do AWS Lambda
**Pergunta:**  
Qual das seguintes afirmações **NÃO** está relacionada ao AWS Lambda?

**Resposta:**  
Permite o gerenciamento total dos recursos de infraestrutura.

---

## 14. Benefícios do AWS Trusted Advisor
**Pergunta:**  
O AWS Trusted Advisor é um serviço de monitoramento e recomendação que auxilia o cliente a utilizar os recursos de sua conta de maneira alinhada com as melhores práticas para trazer muitos benefícios. Quais itens abaixo representam tais benefícios? (Selecione 3 alternativas)

**Resposta:**  
- Segurança  
- Performance  
- Otimização de Custos

---

## 15. Otimização de Custos com S3 Lifecycle
**Pergunta:**  
Uma empresa busca aprimorar a eficiência dos custos ao utilizar o serviço S3. Neste contexto identificou a presença de numerosos registros armazenados que poderiam ser removidos após decorridos 30 dias desde sua criação. Como seria possível otimizar essa situação?

**Resposta:**  
Configurando o S3 Lifecycle (Ciclo de Vida) para que os objetos expirem em 30 dias para serem automaticamente excluídos.

---

## 16. Conceito de Tolerância a Falhas
**Pergunta:**  
Qual das seguintes opções oferece a descrição mais precisa e abrangente do conceito de tolerância a falhas?

**Resposta:**  
A habilidade de um sistema permanecer em funcionamento mesmo se um dos seus componentes falhar.

---

## 17. AWS Free Tier (Nível Gratuito)
**Pergunta:**  
O que é o AWS Free Tier (Nível Gratuito) e quais são as suas categorias de serviços disponíveis?

**Resposta:**  
É um modelo de uso onde você não é cobrado na AWS. Suas categorias são:
- 12 meses de gratuidade
- Sempre gratuito
- Experimentação

---

## 18. Pilares do Well-Architected Framework
**Pergunta:**  
Quais dos seguintes itens fazem parte dos pilares do Well-Architected Framework? (Selecione 2 alternativas)

**Resposta:**  
- Excelência Operacional  
- Segurança

---

## 19. AWS Compute Optimizer e Machine Learning
**Pergunta:**  
Como o AWS Compute Optimizer emprega informações específicas para identificar configurações ideais de recursos na infraestrutura da AWS?

**Resposta:**  
Utilizando Machine Learning.

---

## 20. Registro e Configuração Rápida de Domínio
**Pergunta:**  
Uma empresa deseja lançar um novo produto e precisa criar um novo domínio público para associá-lo ao seu novo site. Qual é a maneira mais rápida e eficaz de realizar essa tarefa utilizando os serviços da AWS?

**Resposta:**  
Criar um novo domínio no Amazon Route 53.

---

## 21. Análise de Logs e Desempenho de Aplicações
**Pergunta:**  
Uma agência de viagens online tem a necessidade de armazenar, analisar e correlacionar dados de logs de seus aplicativos. Qual serviço da AWS é mais indicado para atender a essa demanda?

**Resposta:**  
Amazon OpenSearch

---

## 22. Planos de Suporte com Atendimento 24x7
**Pergunta:**  
Quais dos seguintes planos de suporte oferecem acesso ao atendimento ao cliente, whitepapers, documentações e fóruns de suporte 24x7? (Selecione 2)

**Resposta:**  
- Basic  
- Enterprise

---

## 23. Arquitetura Orientada a Eventos
**Pergunta:**  
Uma empresa deu início a um processo de transformação digital em todas as suas plataformas e optou por empregar uma arquitetura de sistemas orientada a eventos. Qual dos serviços a seguir pode ser utilizado como um barramento escalável de eventos para facilitar a implementação dessa arquitetura?

**Resposta:**  
Amazon EventBridge

---

## 24. Utilização do AWS Data Exchange
**Pergunta:**  
A Chief Technology Officer (CTO) de uma rede hospitalar almeja incorporar o AWS Data Exchange em suas plataformas. Para que finalidade esse serviço pode ser utilizado nesse contexto?

**Resposta:**  
Para compartilhar dados de pacientes com outras organizações de saúde.

---

## 25. Transformação de Arquivos com AWS Glue
**Pergunta:**  
Um sistema externo gera arquivos em um formato incompatível com o seu sistema. Qual serviço da AWS pode ser utilizado para realizar a transformação desses arquivos e integrá-los ao seu ambiente de forma eficiente?

**Resposta:**  
AWS Glue – serviço de ETL (Extração, Transformação e Carga).

---

## 26. Identificação de Vulnerabilidades com AWS Inspector
**Pergunta:**  
Uma empresa busca assegurar a segurança das instâncias de uma aplicação que está prestes a ser lançada. Qual é o serviço que auxilia na identificação de vulnerabilidades de segurança e riscos de exposição?

**Resposta:**  
AWS Inspector

---

## 27. Métodos de Pagamento para Instâncias EC2
**Pergunta:**  
Quais das seguintes opções são métodos de pagamento disponíveis para instâncias EC2?

**Resposta:**  
- Reserved (Reservado)  
- On-demand (Sob demanda)

---

## 28. Serviço Serverless para Consultas SQL no S3
**Pergunta:**  
Qual é o serviço serverless da AWS que permite a execução de consultas utilizando o padrão SQL para analisar e processar grandes volumes de dados armazenados no Amazon S3?

**Resposta:**  
Athena

---

## 29. Pilar de Confiabilidade no AWS Well-Architected
**Pergunta:**  
Em relação ao framework de melhores práticas arquitetônicas da AWS, qual pilar se dedica a assegurar que uma carga de trabalho execute sua função prevista de forma correta e consistente, e que essa carga de trabalho seja resiliente?

**Resposta:**  
Confiabilidade

---

## 30. Tipos de Suporte Ofertados pela AWS
**Pergunta:**  
Quais são os cinco tipos de suporte ofertados pela AWS?

**Resposta:**  
- Basic  
- Developer  
- Business  
- Enterprise On-Ramp  
- Enterprise

---

## 31. Funcionalidades do Amazon QuickSight
**Pergunta:**  
Quais são as principais funcionalidades do Amazon QuickSight?

**Resposta:**  
Criar Dashboards de BI com uso de Aprendizado de Máquina (Machine Learning).

---

## 32. Princípio de Design para Alta Demanda
**Pergunta:**  
Uma empresa de e-commerce enfrenta picos de tráfego durante promoções. Qual princípio de design de arquitetura é mais adequado para garantir alta disponibilidade e bom desempenho durante esses picos?

**Resposta:**  
Escalar horizontalmente.

---

## 33. Integração de Arquitetura Híbrida com AWS Storage Gateway
**Pergunta:**  
Uma empresa pretende manter suas cargas de trabalho on-premises e armazenar parte de seus arquivos na AWS, adotando uma arquitetura de nuvem híbrida. Qual serviço proporciona a integração necessária de armazenamento?

**Resposta:**  
AWS Storage Gateway

---

## 34. Banco de Dados Gerenciado com Automação Completa
**Pergunta:**  
Qual dos seguintes serviços de bancos de dados oferecidos pela AWS proporciona, por padrão, gerenciamento completo, incluindo automação de tarefas como backup, aplicação de patches, monitoramento e escalabilidade?

**Resposta:**  
DynamoDB

---

## 35. MFA - Multi-Factor Authentication
**Pergunta:**  
O que é o MFA - Multi-Factor Authentication (Autenticação Multi Fator)?

**Resposta:**  
É um serviço que inclui uma etapa adicional no processo de autenticação de acesso à conta da AWS através do Console Web.

---

## 36. Solução para Baixo Desempenho em Banco de Dados Relacional
**Pergunta:**  
Um time de desenvolvimento detectou baixo desempenho em um banco de dados relacional devido à alta concorrência de consultas e operações. Qual é a abordagem mais eficiente e econômica para solucionar esse problema?

**Resposta:**  
Utilizar Read Replicas.

---

## 37. Hospedagem de Site Estático
**Pergunta:**  
Uma agência de publicidade pretende lançar um site com conteúdo estático para a divulgação de um produto. Qual serviço seria mais apropriado e econômico para esse cenário?

**Resposta:**  
Simple Storage Service (S3)

---

## 38. Princípios do Pilar de Confiabilidade no Well-Architected Framework
**Pergunta:**  
Quais dos seguintes são princípios do pilar de confiabilidade no AWS Well-Architected Framework?

**Resposta:**  
- Implementar recuperação automática para falhas.  
- Planejar limites de capacidade e testar frequentemente.

---

## 39. Microsserviços em Containers sem Servidor
**Pergunta:**  
Um grupo de desenvolvedores com conhecimento limitado em infraestrutura deseja adotar uma arquitetura de microsserviços em containers sem servidor. Qual serviço pode auxiliá-los, dispensando o conhecimento especializado em containers?

**Resposta:**  
AWS Fargate

---

## 40. Auditoria de Ações na Infraestrutura AWS
**Pergunta:**  
Uma empresa precisa auditar sua infraestrutura na AWS para identificar ações manuais e não planejadas de desligamento de recursos. Qual serviço pode auxiliar nessa atividade?

**Resposta:**  
AWS CloudTrail

---

## 41. Depuração de Microsserviços
**Pergunta:**  
O desenvolvedor de uma empresa implementou um sistema baseado em microsserviços e necessita depurar cada um desses serviços para analisar performance e identificar melhorias. Qual serviço é mais apropriado para essa finalidade?

**Resposta:**  
AWS X-Ray

---

## 42. Execução de Tarefas em Lote
**Pergunta:**  
Um banco precisa executar milhares de tarefas de computação em lote com eficiência. Qual é o serviço mais indicado para essa necessidade?

**Resposta:**  
AWS Batch

---

## 43. Pesquisa de Conteúdo no Site
**Pergunta:**  
Uma agência deseja incorporar em seu site uma funcionalidade de pesquisa abrangente em todas as páginas e arquivos. Qual serviço SaaS da AWS oferece essa funcionalidade de forma integrada?

**Resposta:**  
Amazon CloudSearch

---

## 44. Armazenamento Block-level para Instâncias EC2
**Pergunta:**  
Qual é o serviço de alta performance desenvolvido para fornecer block storage para instâncias EC2?

**Resposta:**  
Amazon Elastic Block Storage (EBS)

---

## 45. Banco de Dados em Grafo Gerenciado
**Pergunta:**  
Qual é o serviço de banco de dados em grafo gerenciado pela AWS, que possibilita diversos tipos de relacionamentos entre nós, aplicável em contextos como redes sociais e cadeias logísticas?

**Resposta:**  
Amazon Neptune

---

## 46. Capacidade de Armazenamento do Amazon S3
**Pergunta:**  
Qual é a quantidade máxima de dados que pode ser armazenada no Amazon S3?

**Resposta:**  
A capacidade é virtualmente ilimitada.

---

## 47. Migração de Licenças para a AWS
**Pergunta:**  
Uma empresa deseja migrar suas licenças de software existentes para a AWS, mas precisa vinculá-las a hardware físico exclusivo. Qual a abordagem recomendada?

**Resposta:**  
Configurar um host dedicado no Amazon EC2 para garantir exclusividade de hardware físico e usar o AWS License Manager para rastrear e validar as licenças.

---

## 48. Armazenamento de Catálogos de Produtos
**Pergunta:**  
Um E-Commerce precisa armazenar catálogos de produtos, onde cada item possui atributos como descrição, preço, imagens e avaliações de clientes. Qual serviço de banco de dados é o mais adequado para essa finalidade?

**Resposta:**  
Amazon DynamoDB

---

## 49. Armazenamento Persistente e Escalável para EC2
**Pergunta:**  
Para garantir elasticidade e economia no uso do EC2, mantendo os arquivos de programas e sistemas em um armazenamento persistente e escalável, que pode ser anexado e desanexado conforme necessário, qual serviço da AWS deve ser utilizado?

**Resposta:**  
EBS

---

## 50. Banco de Dados Relacional Altamente Performático
**Pergunta:**  
Qual é o banco de dados relacional totalmente gerenciado pela AWS e que pode ser até 5x mais rápido que o MySQL?

**Resposta:**  
Aurora

---

## 51. Estratégia de Recuperação de Desastres com AWS RDS
**Pergunta:**  
Uma organização busca implementar uma estratégia de Recuperação de Desastres (DR) para suas aplicações. Qual a recomendação mais adequada para a utilização do AWS RDS?

**Resposta:**  
Implementar o RDS em Multi Regions (distribuir em regiões diferentes).

---

## 52. Usuário com Acesso Total à Conta AWS
**Pergunta:**  
Qual usuário possui acesso a todos os recursos da conta, utilizado para acessar o AWS Console pela primeira vez, mas que não é recomendado para uso diário?

**Resposta:**  
AWS account root user

---

## 53. Governança no AWS Cloud Adoption Framework
**Pergunta:**  
Qual das seguintes opções é um princípio essencial do AWS Cloud Adoption Framework (AWS CAF) relacionado à perspectiva de governança?

**Resposta:**  
Definição de políticas e monitoramento de conformidade.

---

## 54. Análise de Custos com AWS CostExplorer
**Pergunta:**  
Um time de desenvolvimento lançou o piloto de uma aplicação e o CTO solicitou uma análise dos custos de infraestrutura na AWS. Qual serviço fornece essas informações?

**Resposta:**  
AWS CostExplorer

---

## 55. Edição Remota de Código com Cloud9
**Pergunta:**  
Um desenvolvedor precisa modificar partes do código de uma aplicação, mas não possui acesso ao seu computador ou IDE. Como contornar essa situação utilizando serviços da AWS?

**Resposta:**  
Utilizando o Cloud9 através de um navegador de internet.

---

## 56. Monitoramento de Uso de Processamento e Memória
**Pergunta:**  
Uma empresa deseja acompanhar o percentual de utilização de processamento e memória em seus servidores durante um período específico. Qual serviço da AWS é adequado para essa necessidade?

**Resposta:**  
AWS CloudWatch

---

## 57. Classe de Armazenamento com Custos Elevados no S3
**Pergunta:**  
Qual das classes a seguir pode resultar em custos mais elevados no uso do S3?

**Resposta:**  
Standard

---

## 58. Pipeline Típica de CI/CD na AWS
**Pergunta:**  
Ao utilizar os serviços da AWS, qual é a sequência típica esperada em uma pipeline de CI/CD?

**Resposta:**  
CodeCommit, CodeBuild, CodeDeploy.

---

## 59. Criação de Bancos de Dados via Código
**Pergunta:**  
Uma organização deseja padronizar o processo de criação e configuração de todos os bancos de dados por meio de código, implementando isso automaticamente via CI/CD. Qual serviço é recomendado?

**Resposta:**  
AWS CloudFormation

---

## 60. Framework de Melhores Práticas Arquitetônicas
**Pergunta:**  
Com base nos princípios de excelência operacional, segurança, confiabilidade, desempenho eficiente, sustentabilidade e otimização de custos, qual é o framework que auxilia arquitetos na construção de aplicações seguras e otimizadas?

**Resposta:**  
AWS Well-Architected

---

## 61. Orquestração de Aplicações Sem Servidor
**Pergunta:**  
Uma empresa pretende desenvolver uma aplicação sem servidor utilizando Lambda, SQS e SNS. Qual serviço seria mais adequado para orquestrar e integrar esses recursos em fluxos de negócio?

**Resposta:**  
AWS Step Functions

---

## 62. Definição do AWS Wavelength
**Pergunta:**  
A equipe de Arquitetura de Soluções recomendou o uso do AWS Wavelength para melhorar o desempenho das aplicações. Qual a melhor definição para o AWS Wavelength?

**Resposta:**  
Uma região geográfica da AWS especialmente projetada para cargas de trabalho de baixa latência.

---

## 63. Estimativa de Custos Detalhada na AWS
**Pergunta:**  
Qual serviço da AWS é recomendado para estimar de forma detalhada e precisa os custos de implementação e operação dos diversos serviços, considerando diferentes cenários e variáveis?

**Resposta:**  
AWS Pricing Calculator

---

## 64. Análise de Sentimentos com AWS
**Pergunta:**  
Uma startup busca um serviço que identifique sentimentos em textos digitados durante conversas entre clientes e atendentes em um chat de e-commerce. Qual serviço pode ser utilizado?

**Resposta:**  
Amazon Comprehend

---

## 65. Classe de Armazenamento Padrão no S3
**Pergunta:**  
Qual é a opção de armazenamento padrão (default) do serviço S3?

**Resposta:**  
Standard
