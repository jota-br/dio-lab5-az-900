# Computação e Rede
É o serviço de fornecimento de recursos sob demanda.

### Máquinas virtuais
- São emulações de software de computadores fisicos.
- Tem seu processador, memória e armazenamento e rede virtual.
- É um modelo de IaaS.
- Permite a configuração do Conjunto de dimensionamento:
  - Utilizando VMs idênticas (em pares) no Domínio de falha e possibilitando a execução de atualizações utilizando estratégias no Domínio de Atualização;
    - O objetivo é garantir a disponibilidade das VMs, uma vez que a atualização e manutenção do OS e software é por conta da organização (modelo IaaS).
- Deverá ser configurado as opções de disponibildiade.
- Utilização ou não do Spot do Azure, recomendando apenas em desenvolvimento, pois irá ceder o processamento e por consequência derrubar a máquina e caso de necessidade por parte de outra organização que requer o uso de processamento no data center.
- Configurações de disco.
- Rede: criação de VNet para comunicação, pontos de extremidade públicos para acesso pela internet ou pontos de extermidade privados para acesso dentro da rede.
  - Se for necessário duas VNets se comunicarem a configuração do emparelhamento de rede é obrigatório.
  - Cuidar com a camada de rede e criação das VNets para evitar overlap.
 
### Área de Trabalho Virtual
- Permite a criação de VMs para utilização de forma remota, uma alternativa viável para utilização de ferramentas internas de uma organização.
- Pode ser utilizada por um pool de usuários ou se de uso pessoal.

### Serviços de contêineres
Serviços do tipo PaaS, que oferece ambientes virtualizados que podem escalar conforme a demanda.
- Instâncias de Contêiner: serviço que executa um contêiner no Azure.
- Aplicativos de Contêiner: serviço com instâncias de contêineres que pode balancear a carga e escalar.
- Serviço de Kubernetes do Azure (AKS): serviço para organização de contêineres com arquitetura distribuida gerindo o seus ciclos de vida.

### Azure Functions
Serviço PaaS para operações sem servidor.

É um serviços de execução de código baseado em eventos que não exige infraestrutura de servidor durante períodos inativos.
- Podemos utilizar imagens ou códigos
- Utilizar uma das pilhas de runtime disponível.
- Com suporte para Linux e Windows.

### Serviços de Aplicativos do Azure
Serviço ideal para implantar aplicativos Web e APIs de forma rápida. Serviço do tipo PaaS.
