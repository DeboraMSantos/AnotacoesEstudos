<div style="display: flex; align-items: center;">
    <img src="https://upload.wikimedia.org/wikipedia/commons/9/93/Amazon_Web_Services_Logo.svg" alt="AWS Logo" style="width: 100px; margin-right: 10px;">
    <h1 style="margin: 0;">Fundamentos Técnicos da AWS</h1>
</div>

<p>Anotações referente ao curso Fundamentos Técnicos da AWS na Plataforma AWS SKILL BUILDER</p>

<menu> 
    
- [Módulo 1: Introdução à Amazon Web Services](#módulo-1-introdução-à-amazon-web-services-aws)
- [Módulo 2: Computação da AWS](#m%C3%B3dulo-2-computa%C3%A7%C3%A3o-da-aws)
- [Módulo 3: Rede da AWS](#módulo-3-rede-da-aws)
- [Módulo 4: Armazenamento da AWS](#módulo-4-armazenamento-da-aws)
- [Módulo 5: Bancos de Dados](#módulo-5-bancos-de-dados)
- [Módulo 6: Monitoramento, Otimização e Serverless](#módulo-6-monitoramento-otimização-e-serverless)
  
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

### Modelos de implantação da computação em nuvem

A computação em nuvem oferece aos desenvolvedores e departamentos de TI a capacidade de se concentrar no que é mais importante, evitando trabalhos como aquisição, manutenção e planejamento de capacidade. Com o crescimento da popularidade da computação em nuvem, várias estratégias de implantação surgiram para atender a essas necessidades específicas de usuários distintos. Cada tipo de método de implantação disponibiliza diferentes níveis de controle, flexibilidade e gerenciamento. Entender as diferenças entre essas estratégias de implantação pode ajudar você a decidir qual conjunto de serviços é ideal para suas necessidades. 

### Modelos de implantação on-premises, na nuvem e híbrida.

#### On-premises

Antes da nuvem, empresas e organizações hospedavam e mantinham hardware, como equipamentos de computação, armazenamento e rede em seus próprios data centers. Muitas vezes, eles alocavam departamentos de infraestrutura inteiros para cuidar de seus data centers, o que resultou em operações dispendiosas que impossibilitaram algumas workloads e experimentações. 

À medida que o uso da internet se tornou mais difundido, a demanda por equipamentos de computação, armazenamento e rede aumentou. Para algumas empresas e organizações, o custo de manter uma grande presença física era insustentável. Para resolver esse problema, surgiu a computação em nuvem.

#### Nuvem

Computação em nuvem é a entrega de recursos de TI sob demanda pela internet, com pagamento conforme o uso. Com a computação em nuvem, as empresas não precisam gerenciar e manter hardware e data centers próprios. Em vez disso, empresas como a Amazon Web Services (AWS) têm e mantêm data centers e fornecem tecnologias e serviços de data center virtual para empresas e usuários pela internet.

#### Híbrida

Uma terceira opção é uma implantação híbrida. Esse tipo de implantação é uma maneira de conectar infraestrutura e aplicações entre recursos baseados em nuvem e recursos atuais que não se encontram na nuvem. O método mais comum de implantação híbrida entre a nuvem e a infraestrutura on-premises existente conecta os recursos da nuvem aos sistemas internos para estender e expandir a infraestrutura de uma organização na nuvem.

### Modelos de implantação de computação on-premises ou em nuvem.
Para ajudar a diferenciar entre executar workloads on-premises e na nuvem, considere um cenário em que os desenvolvedores devem implantar um novo recurso da aplicação. Antes da implantação, a equipe deseja testar o recurso em um ambiente de garantia de qualidade (QA) separado que tenha as mesmas configurações que o de produção. Em uma solução on-premises, um ambiente adicional exige que você compre e instale hardware, conecte o cabeamento necessário, forneça energia, instale sistemas operacionais e muito mais. Essas tarefas podem ser demoradas e caras. Enquanto isso, o tempo de comercialização do novo recurso aumenta enquanto os desenvolvedores esperam pelo ambiente de controle de qualidade (QA). 

Por outro lado, ao executar sua aplicação na nuvem, você pode replicar todo o ambiente de produção em questão de minutos ou até mesmo segundos. Em vez de instalar fisicamente o hardware e conectar o cabeamento, a solução é gerenciada pela internet.

O uso da computação em nuvem economiza tempo durante a configuração e remove tarefas redundantes e desnecessárias. Se você olhar para qualquer aplicação, verá que alguns de seus aspectos são muito importantes para sua empresa, como o código. No entanto, outros aspectos não são diferentes de qualquer outra aplicação que você possa fazer, por exemplo, a computação na qual o código é executado. Algumas tarefas comuns repetitivas não diferenciam sua empresa, como instalar máquinas virtuais (VMs) ou armazenar backups. Ao remover essas tarefas, você pode se concentrar no que é estrategicamente exclusivo para a sua empresa e deixar que a AWS cuide das tarefas demoradas que não a separam dos seus concorrentes. Chamamos isso de remoção de "trabalho pesado indiferenciado". É aí que a AWS se encaixa em tudo isso.



A AWS fornece serviços de computação em nuvem. Os recursos de TI mencionados na definição de computação em nuvem são produtos da AWS. Para a aplicação de diretório corporativo deste curso, você usará os produtos da AWS para arquitetar uma infraestrutura dimensionável, altamente disponível e econômica para hospedar a aplicação de diretório corporativo. Dessa forma, você pode disponibilizar a aplicação rapidamente, sem gerenciar hardware físico pesado.



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

## Interação com a AWS
Na AWS, toda interação é feita através de chamadas de API autenticadas e autorizadas, que podem ser realizadas por meio de três ferramentas principais: **Console de Gerenciamento da AWS**, **AWS Command Line Interface (CLI)** e **SDKs da AWS**.

### **Console de Gerenciamento da AWS:**
- **Interface Web:** Permite gerenciar os recursos da nuvem através de uma interface gráfica amigável.
- **Categorias de Serviços:** Os serviços são agrupados em categorias, como Computação, Armazenamento, Banco de Dados, entre outros.
- **Seletor de Região:** Permite escolher a região onde você deseja executar os serviços.

### **AWS CLI:**
- **Linha de Comando Unificada:** Ferramenta para gerenciar produtos AWS por meio de comandos.
- **Automação e Scripts:** Pode ser usada para automatizar processos, como a coleta diária de dados de servidores.
- **Código Aberto e Multiplataforma:** Disponível para Windows, Linux e macOS.

**Exemplo de uso da CLI:**
- Comando: `aws ec2 describe-instances`
- Resposta: Dados detalhados sobre as instâncias EC2 em execução.

### **SDKs da AWS:**
- **Integração com Linguagens de Programação:** Os SDKs (Kits de Desenvolvimento de Software) permitem integrar código de aplicação com os produtos da AWS.
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
*Conteúdo do módulo 2...*

## Módulo 3: Rede da AWS
*Conteúdo do módulo 3...*

## Módulo 4: Armazenamento da AWS
*Conteúdo do módulo 4...*

## Módulo 5: Bancos de Dados
*Conteúdo do módulo 5...*

## Módulo 6: Monitoramento, Otimização e Serverless
*Conteúdo do módulo 6...*
