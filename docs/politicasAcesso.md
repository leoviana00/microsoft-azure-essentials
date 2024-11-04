<h1 align="center">📓 Guia para Gerenciamento de Políticas de Acesso no Microsoft Azure</h1>


# Gerenciando Políticas de Acesso no Microsoft Azure

## Descrição

O gerenciamento de políticas de acesso no Microsoft Azure permite que você controle e monitore quem tem acesso aos seus recursos, garantindo segurança, conformidade e governança. O Azure Policy e o Azure Role-Based Access Control (RBAC) são as principais ferramentas utilizadas para definir e gerenciar esses acessos.

Este guia irá fornecer um passo a passo sobre como implementar e gerenciar políticas de acesso no Azure, bem como os benefícios desse processo.

## Índice

- [Passo a Passo](#passo-a-passo)
  - [1. Introdução ao Azure Policy](#1-introdução-ao-azure-policy)
  - [2. Criando Políticas de Acesso](#2-criando-políticas-de-acesso)
  - [3. Monitorando a Conformidade das Políticas](#3-monitorando-a-conformidade-das-políticas)
  - [4. Gerenciando Acessos com Azure RBAC](#4-gerenciando-acessos-com-azure-rbac)
- [Benefícios de Gerenciar Políticas de Acesso](#benefícios-de-gerenciar-políticas-de-acesso)


## Passo a Passo

### 1. Introdução ao Azure Policy

1. O **Azure Policy** permite que você crie, atribua e gerencie políticas que asseguram que seus recursos estão em conformidade com as regras corporativas.
2. Para acessar o Azure Policy:
   - Navegue até o portal do Azure e procure por "Azure Policy" na barra de pesquisa.
   - No painel do Azure Policy, você pode visualizar todas as políticas disponíveis e criar novas.

### 2. Criando Políticas de Acesso

1. **Criar uma Nova Política**:
   - No painel do Azure Policy, clique em **Criar Definição de Política**.
   - Selecione o tipo de política de acesso que deseja aplicar. Alguns exemplos incluem:
     - Bloquear a criação de recursos em regiões não permitidas.
     - Forçar o uso de redes virtuais específicas.
     - Limitar o tipo de máquinas virtuais que podem ser criadas.

2. **Atribuindo Políticas a um Escopo**:
   - Após criar a definição, atribua a política a um escopo específico, como uma assinatura, grupo de recursos ou recurso individual.
   - Defina parâmetros opcionais, como exceções ou exclusões para determinados usuários ou grupos.

### 3. Monitorando a Conformidade das Políticas

1. No painel do Azure Policy, você pode monitorar a conformidade de todos os recursos.
   - Acesse o painel de **Conformidade** para ver quais recursos estão em conformidade com as políticas e identificar aqueles que violam as regras estabelecidas.
   - Políticas com "Efeito de Negar" bloqueiam ações, enquanto políticas com "Efeito de Auditar" apenas alertam quando algo está fora de conformidade.

2. **Ações Corretivas**:
   - A ferramenta permite aplicar ações corretivas em recursos fora de conformidade, como reconfiguração de parâmetros ou remoção de acessos.

### 4. Gerenciando Acessos com Azure RBAC

1. O **Azure Role-Based Access Control (RBAC)** é um sistema que gerencia permissões de acesso baseadas em papéis dentro do Azure.
   - Você pode atribuir papéis a usuários, grupos ou aplicativos para controlar quem pode gerenciar, criar ou acessar recursos.
   
2. **Criando e Atribuindo Papéis**:
   - No painel do recurso ou grupo de recursos, clique em **Controle de Acesso (IAM)**.
   - Escolha **Adicionar função de atribuição** e selecione o papel adequado (por exemplo, Leitor, Colaborador, Proprietário).
   - Atribua o papel a um usuário ou grupo existente.

3. **Personalizando Papéis**:
   - O Azure permite criar papéis personalizados para necessidades específicas de acesso. Isso pode ser feito a partir do IAM ou diretamente do Azure CLI.
   - Defina permissões específicas e atribua ao escopo desejado.


## Benefícios de Gerenciar Políticas de Acesso

1. **Segurança Aprimorada**: Aplicar políticas de acesso específicas reduz o risco de uso indevido de recursos e protege a infraestrutura contra acessos não autorizados.
2. **Conformidade Automática**: O Azure Policy permite que você assegure que os recursos estão sempre em conformidade com os requisitos internos e externos, sem a necessidade de intervenção manual constante.
3. **Governança Eficiente**: Com o Azure RBAC, você garante que o acesso aos recursos seja concedido com base em papéis bem definidos, evitando a sobrecarga de permissões.
4. **Monitoramento Centralizado**: O painel de conformidade centraliza o monitoramento de todas as políticas de acesso, facilitando a auditoria e a detecção de violações de conformidade.
5. **Redução de Custos e Erros**: Aplicar políticas consistentes ajuda a reduzir custos ao prevenir a criação de recursos desnecessários ou ociosos, além de minimizar erros operacionais.

