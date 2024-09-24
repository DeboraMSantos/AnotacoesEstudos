# Introdução

Estou dando início aos meus estudos em **AWS Cloud** e criei esta página para organizar minhas anotações ao longo da jornada. Feedbacks e sugestões são sempre bem-vindos e muito aceito! 💖

<div style="display: flex; align-items: center;">
    <img src="https://upload.wikimedia.org/wikipedia/commons/9/93/Amazon_Web_Services_Logo.svg" alt="AWS Logo" style="width: 100px; margin-right: 10px;">
    <h1 style="margin: 0;">Fundamentos Técnicos da AWS</h1>
</div>


## Módulo 1: Introdução à Amazon Web Services (AWS)

### Visão Geral do Curso
- **Zonas de Disponibilidade**: São regiões geográficas como América do Sul, Estados Unidos, etc.
- **Rede Privada (VPC)**: A aplicação será criada em uma **Virtual Private Cloud** (VPC) para isolar os recursos.
- **Elastic Compute Cloud (EC2)**: O backend será hospedado no EC2, que oferece máquinas virtuais escaláveis.
- **Amazon S3 (Simple Storage Service)**: Usado para armazenar as fotos dos funcionários com capacidade de armazenamento ilimitado de qualquer tipo de arquivo.
- **Amazon CloudWatch**: Monitora a aplicação para garantir escalabilidade e tolerância a falhas.
- **Elastic Load Balancer (ELB)**: Distribui o tráfego entre as instâncias EC2.
- **Auto Scaling**: Escala automaticamente as instâncias de EC2 horizontalmente, conforme a demanda.
- **AWS IAM (Identity and Access Management)**: Controla o acesso aos recursos e gerencia identidades de forma segura.

### O que é a AWS?
A AWS é uma plataforma de computação em nuvem que oferece serviços de TI sob demanda pela internet. Isso permite que empresas eliminem a necessidade de gerenciar datacenters físicos, utilizando datacenters virtuais fornecidos pela AWS.

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

## Infraestrutura Global da AWS

### Regiões
- As regiões são locais geográficos onde a AWS hospeda seus datacenters. Exemplo: `us-east-1` (Norte da Virgínia), `sa-east-1` (São Paulo).
- Cada região opera de forma independente e não compartilha dados sem consentimento do cliente.

### Zonas de Disponibilidade (AZs)
- As Zonas de Disponibilidade são datacenters localizados dentro de uma região.
- Exemplo: `us-east-1a` é uma AZ dentro da região `us-east-1` (Norte da Virgínia).
- Os serviços podem ser implantados com escopo de Zona de Disponibilidade (AZ), Regional ou Global.

### Escopo dos Serviços AWS
- **Serviços Regionais**: AWS gerencia a durabilidade e disponibilidade dos dados entre AZs.
- **Serviços de AZ**: O cliente gerencia a replicação entre AZs para garantir a alta disponibilidade.

## Serviços Chave da AWS

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
