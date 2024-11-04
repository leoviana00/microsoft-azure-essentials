<h1 align="center">📓 Guia para Criação de Máquinas Virtuais no Azure</h1>


## 📑 Menu

- [1️⃣ Introdução](#introdução)
- [2️⃣ Pré-requisitos](#pré-requisitos)
- [3️⃣ Passo a Passo para Criar uma Máquina Virtual](#passo-a-passo-para-criar-uma-máquina-virtual)
- [4️⃣ Benefícios de Usar Máquinas Virtuais no Azure](#benefícios-de-usar-máquinas-virtuais-no-azure)
- [5️⃣ Dicas de Segurança](#dicas-de-segurança)



## Introdução

As máquinas virtuais (VMs) no Azure são componentes fundamentais para a computação na nuvem, permitindo que você execute aplicações e serviços em um ambiente isolado e controlado. Este guia oferece um passo a passo detalhado para a criação de uma VM no Azure e destaca os principais benefícios de usar VMs na plataforma.


## Pré-requisitos

Antes de começar, certifique-se de ter:

- Uma conta ativa no [Microsoft Azure](https://portal.azure.com).
- Permissões suficientes para criar recursos no Azure (como assinante ou proprietário).



## Passo a Passo para Criar uma Máquina Virtual

### 1. Acesse o Portal do Azure

- Entre no [portal do Azure](https://portal.azure.com) com suas credenciais.

### 2. Navegue até a Criação de Recursos

- No menu lateral esquerdo, clique em **"Create a resource"**.
- Selecione **"Compute"** e, em seguida, **"Virtual Machine"**.

### 3. Configure as Informações Básicas

- **Subscription**: Escolha a assinatura onde a VM será criada.
- **Resource Group**: Selecione um grupo de recursos existente ou crie um novo.
- **Virtual Machine Name**: Defina o nome da sua VM.
- **Region**: Escolha a região onde a VM será hospedada.
- **Image**: Selecione o sistema operacional desejado (por exemplo, Windows Server, Ubuntu).
- **Size**: Escolha o tamanho da VM (CPU, memória).

### 4. Configuração de Acesso

- **Username**: Crie um nome de usuário para acessar a VM.
- **Authentication Type**: Escolha entre senha ou chave SSH.
- **Inbound Port Rules**: Defina as portas que serão abertas para o tráfego de entrada (ex: HTTP, SSH).

### 5. Configurações Avançadas (Opcional)

- **Disks**: Configure discos adicionais para armazenamento.
- **Networking**: Ajuste as configurações de rede, como VNet, subnets, IPs públicos.
- **Management**: Configure opções de monitoramento, backup, entre outros.

### 6. Revisar e Criar

- Revise todas as configurações definidas.
- Clique em **"Create"** para iniciar a criação da VM.

### 7. Acessar a Máquina Virtual

- Após a implantação, navegue até o recurso da VM e utilize as credenciais configuradas para acessar a máquina via RDP (Windows) ou SSH (Linux).



## Benefícios de Usar Máquinas Virtuais no Azure

### 1. **Escalabilidade**
   - As VMs no Azure permitem que você escale verticalmente ou horizontalmente conforme a demanda do seu aplicativo, garantindo performance e custo eficientes.

### 2. **Flexibilidade**
   - Com uma ampla variedade de imagens de sistema operacional e tamanhos de VM, você pode escolher a configuração que melhor se adapta às suas necessidades.

### 3. **Segurança**
   - As VMs no Azure oferecem várias camadas de segurança integradas, incluindo proteção contra DDoS, firewalls e encriptação de dados.

### 4. **Backup e Recuperação**
   - Azure fornece opções robustas de backup e recuperação, garantindo que seus dados estejam seguros e possam ser restaurados rapidamente em caso de falhas.

### 5. **Integração com Outros Serviços**
   - As VMs podem ser facilmente integradas com outros serviços do Azure, como Banco de Dados, Armazenamento, e Redes Virtuais, oferecendo uma solução completa na nuvem.

### 6. **Modelo de Pagamento Pay-as-You-Go**
   - Pague apenas pelo que você usa, permitindo otimizar os custos conforme a utilização da VM.

## Dicas de Segurança

- Utilize sempre senhas fortes ou chaves SSH para aumentar a segurança de acesso à VM.
- Defina regras claras no NSG para limitar as portas de entrada e proteger sua infraestrutura.
- Considere o uso de backups regulares e ative diagnósticos de monitoramento para garantir o bom funcionamento da VM.
