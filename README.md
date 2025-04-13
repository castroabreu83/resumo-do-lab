# resumo-do-lab
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Benefícios da nuvem - Laboratório.

No laboratório "Benefícios da Nuvem", tive a oportunidade de explorar os principais conceitos relacionados à computação em nuvem e como a plataforma Microsoft Azure se destaca nesse cenário. Um dos pontos mais marcantes foi o aprendizado sobre os Acordos de Nível de Serviço (SLAs) oferecidos pela Microsoft Azure.

Os SLAs são compromissos contratuais que definem o nível mínimo de qualidade que a Microsoft garante para os seus serviços na nuvem, incluindo disponibilidade, desempenho e conectividade. Esses acordos asseguram que os recursos contratados estarão acessíveis por um percentual significativo do tempo. No portal de criação do Azure, é possível configurar opções que impactam diretamente a disponibilidade dos serviços, como o uso de Zonas de Disponibilidade, redundância geográfica e replicação de dados.

Além disso, aprendi que a escolha de configurações de alta disponibilidade, como a distribuição de aplicativos em múltiplas regiões ou zonas, pode garantir níveis de SLA superiores, chegando a 99,99% ou mais, dependendo do serviço contratado. Isso reflete diretamente na confiabilidade das aplicações, mitigando interrupções e garantindo uma melhor experiência ao usuário final.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Tipos de Serviço de nuvem - Laboratório.

Na aula, foram abordados os principais conceitos e práticas para a criação e gerenciamento de máquinas virtuais (VMs) no Azure. O conteúdo foi dividido nos seguintes tópicos principais:

Na aula, foram abordados os principais conceitos e práticas para a criação e gerenciamento de máquinas virtuais (VMs), banco de dados, e estratégias de backup no Azure. O conteúdo foi dividido nos seguintes tópicos:

1. Criação de Máquinas Virtuais no Azure

2. Imagens de Máquina Virtual

3. Arquitetura de VMs

4. Criação de Banco de Dados no Azure

5. Tipos de Backup no Azure

   Foi dada maior ênfase a criação d ebanco de dados onde foram abordados os subtópicos.

a)Escolha do tipo de banco de dados com base na aplicação.
b)Seleção de tamanho, escalabilidade e região.
c)Configuração de usuários, autenticação e permissões.
d)Backup e Recuperação:
e)Azure oferece backups automáticos com pontos de restauração configuráveis.
f)Restauração de banco de dados para uma nova instância em caso de falhas.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Componentes de arquitetura do Azure - Laboratório.

Criar grupos de recursos
Entre no portal do Azure.

Selecione Grupos de recursos.

Selecione Criar.

![image](https://github.com/user-attachments/assets/8707b2db-8f1e-4dd6-a429-12bee60e9009)

Insira os valores a seguir:

Assinatura: Selecione sua assinatura do Azure.

Grupo de recursos: insira um nome para o novo grupo de recursos.

Região: selecione uma localização do Azure, como EUA Central.

![image](https://github.com/user-attachments/assets/5902b8f6-5054-47c6-8116-6bd8e5179a13)

Selecione Examinar + criar.

Selecione Criar. Leva alguns segundos para criar um grupo de recursos.

Selecione Atualizar no menu superior para atualizar a lista de grupos de recursos e, em seguida, selecione o grupo de recursos recém-criado para abri-lo. Ou selecione Notificação (o ícone de sino) na parte superior e, em seguida, selecione Ir para o grupo de recursos para abrir o grupo de recursos recém-criado.

![image](https://github.com/user-attachments/assets/a31d5d91-f251-46be-926a-87d1ede89157)

Listar os grupos de recursos
Entre no portal do Azure.

Para listar os grupos de recursos, selecione Grupos de recursos.

Para personalizar as informações exibidas para os grupos de recursos, configure os filtros. A captura de tela a seguir mostra as outras colunas que você pode adicionar à exibição:

![image](https://github.com/user-attachments/assets/6f7aa0bd-8096-4a8b-8fd8-2fb2f9ff9f42)


--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Principais Tipos de Armazenamento no Azure
1. Blob Storage
Ideal para armazenar dados não estruturados: imagens, vídeos, backups, logs, documentos etc.

Tipos de blobs:

Block Blob (mais comum – arquivos)

Append Blob (logs, dados contínuos)

Page Blob (discos de VMs)

Suporta integração com CDN, replicação e políticas de acesso.

2. File Storage (Azure Files)
Compartilhamento de arquivos baseado em nuvem, acessível via SMB e NFS.

Pode ser mapeado como unidade de rede em Windows, Linux e Mac.

Excelente para substituir servidores de arquivos locais.

3. Queue Storage
Armazena mensagens para comunicação assíncrona entre componentes de aplicativos.

Usado em sistemas distribuídos, filas de trabalho e processamento em segundo plano.

4. Table Storage
Banco NoSQL para armazenar grandes volumes de dados estruturados e com acesso rápido.

Ideal para logs, catálogos e dados que não exigem relações complexas.

5. Disk Storage
Discos gerenciados usados por máquinas virtuais (VMs).

Tipos: HDD padrão, SSD padrão e SSD premium.

Oferece alta performance e durabilidade.

🔐 Segurança e Redundância
O Azure Storage oferece:

Criptografia em repouso (Storage Service Encryption)

Controle de acesso com RBAC e SAS Tokens

Replicação automática dos dados, com opções como:

LRS (Local)

ZRS (Zona)

GRS (Geo)

RA-GRS (Leitura georredundante)

⚙️ Ferramentas e Acessos
Portal Azure – interface gráfica para gerenciamento

Azure CLI / PowerShell – comandos automatizados

AzCopy – ferramenta de linha de comando para transferir dados

SDKs e APIs REST – integração com apps e sistemas

-------------------------------------------------------------------------------------------------------------------------------------------------------------------

O que dá para fazer com o Entra ID?
✅ Autenticação e Acesso
Login seguro com MFA (autenticação multifator)

Single Sign-On (SSO) para acessar diversos aplicativos com um único login

Suporte a logins com biometria, senha, chave de segurança ou app autenticador

✅ Gerenciamento de Identidades
Criar e gerenciar usuários, grupos e funções

Atribuir permissões e políticas de acesso baseadas em função (RBAC)

✅ Acesso Condicional
Permite definir regras de segurança, como:

"Se o usuário estiver fora do país, pedir MFA"

"Se estiver em um dispositivo não confiável, bloquear o acesso"

✅ Integração com Apps
Funciona com apps SaaS como:

Microsoft 365

Salesforce

Zoom

GitHub

Também suporta aplicativos personalizados usando OAuth, OpenID Connect ou SAML

✅ Identidade Híbrida
Pode ser integrado com o Active Directory local (AD DS), permitindo uma identidade unificada com sincronização de usuários.

🛡️ Segurança e Conformidade
Microsoft Defender for Identity integrado

Relatórios de segurança e risco

Suporte a políticas de Zero Trust

Conformidade com GDPR, ISO, SOC e outros padrões

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
O Azure TCO Calculator (Calculadora de Custo Total de Propriedade) é uma ferramenta gratuita da Microsoft que ajuda você a entender quanto pode economizar ao migrar do ambiente local (on-premises) para a nuvem Azure.

Ele não mostra preços de serviços individuais, mas sim uma comparação completa entre os custos atuais do seu datacenter e os custos estimados na nuvem.

🎯 Para que serve?
O TCO Calculator serve para:

Avaliar economias de longo prazo ao migrar para o Azure

Justificar uma decisão de migração com dados financeiros claros

Apresentar os custos atuais vs. custos no Azure

Apoiar gestores e times de TI na tomada de decisão estratégica

🧮 O que ele considera na análise?
A ferramenta avalia o custo atual do seu ambiente local, incluindo:

Custo On-Premises	Custo no Azure
Hardware	Máquinas Virtuais
Licenças de software	Licenciamento em nuvem
Energia elétrica	Inclusa no custo do Azure
Mão de obra e suporte	Automatização e gestão simplificada
Espaço físico	Eliminado na nuvem
Você insere informações como:

Número de servidores

Capacidade de armazenamento atual

Custos com pessoal de TI

Energia e refrigeração

Licenças de software

E o resultado é um relatório claro, com gráficos e estimativas, mostrando:

Custo total atual (on-premises)

Custo estimado no Azure

Economia projetada em 1, 3 e 5 anos

🆚 Diferença entre TCO Calculator e Calculadora de Preços do Azure:

Azure TCO Calculator	            |    Calculadora de Preços do Azure
-----------------------------------------------------------------------
Estima economia de migração	   |    Estima custo mensal de uso
Foco em ambientes on-premises	   |    Foco em serviços individuais no Azure
Custo total em longo prazo	      |    Custo específico por serviço
Usa dados do ambiente atual	   |    Usa configurações que você deseja contratar

----------------------------------------------------------------------------------------------------------------------------------------------------------------

O Service Trust Portal (STP) é uma plataforma da Microsoft que fornece transparência e informações detalhadas sobre segurança, conformidade e privacidade dos serviços em nuvem da Microsoft, incluindo Azure, Microsoft 365 e Dynamics 365.

✨ Principais recursos do STP:
Relatórios de auditoria e conformidade (como ISO, SOC, NIST)

Detalhes sobre como a Microsoft protege os dados

Acesso ao Compliance Manager, que ajuda empresas a rastrearem sua própria conformidade

Biblioteca de documentos com Guias de Segurança, Avaliações de Risco e Controles de Segurança

📍 Acesso: https://servicetrust.microsoft.com

📜 Certificações, Regulamentos e Padrões
No STP, você encontra certificações reconhecidas internacionalmente, que mostram que a Microsoft cumpre os principais padrões de segurança e privacidade, como:

ISO/IEC 27001, 27017, 27018 — Segurança da informação e proteção de dados na nuvem

SOC 1, SOC 2, SOC 3 — Relatórios de controles internos

GDPR (Europa) e LGPD (Brasil) — Regulamentações de privacidade de dados

FedRAMP, NIST, CSA STAR — Normas dos EUA para serviços governamentais e em nuvem

HIPAA — Requisitos para dados de saúde

Essas certificações são importantes para empresas que precisam garantir conformidade legal e segurança dos dados ao usar o Azure.

📂 Documentos Aplicáveis
Esses documentos estão disponíveis no STP e incluem:

Relatórios de Auditoria (SOC, ISO)

Avaliações de Risco

Guias de Implementação Segura

Relatórios de Impacto da Privacidade

Listas de Controles de Segurança

Esses materiais ajudam profissionais de compliance, jurídico e TI a tomar decisões informadas sobre a adoção dos serviços Microsoft.

🗂️ Resource Groups (Grupos de Recursos)
No Azure, um Resource Group é uma unidade lógica que agrupa recursos relacionados de uma aplicação (como VMs, bancos de dados, redes, etc.).

Benefícios:
Gerenciamento centralizado: aplicar tags, políticas e permissões

Organização lógica de recursos por projeto, ambiente ou aplicação

Permite monitorar e controlar custos de forma separada

Pode ser usado para implantar, atualizar ou deletar recursos em lote

🔒 Locks (Bloqueios de Recursos)
Os Resource Locks são usados para proteger recursos contra modificações ou exclusões acidentais. Podem ser aplicados a recursos individuais ou grupos inteiros.

Tipos de bloqueio:
ReadOnly (Somente Leitura): impede modificações ou ações operacionais (como iniciar/encerrar VMs)

CanNotDelete (Não pode excluir): impede que o recurso seja excluído, mas permite edições

Esses bloqueios são importantes para manter a integridade de ambientes críticos.

📊 Microsoft Purview
O Microsoft Purview é um conjunto de soluções para governança de dados, conformidade, proteção da informação e gerenciamento de riscos.

Recursos do Purview:
Catálogo de dados: permite mapear, classificar e entender onde estão os dados

Data Loss Prevention (DLP): evita vazamentos de dados sensíveis

Gerenciamento de riscos internos: detecta comportamentos suspeitos

Governança e conformidade: ajuda a atender normas como LGPD e GDPR

Purview é ideal para organizações que lidam com dados confidenciais e precisam gerenciar o ciclo de vida e a segurança da informação.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------

O Azure Resource Manager (ARM) é o serviço de gerenciamento de recursos que permite implantar, atualizar e gerenciar recursos do Azure. Ele oferece uma interface unificada e permite organizar, controlar o acesso e aplicar políticas aos recursos.

Características:
Modelos ARM (JSON): Para implantar recursos de maneira declarativa.

Suporte a grupos de recursos: Organiza e gerencia recursos.

Controle de acesso e políticas: Implementa RBAC e políticas para governança.

🔧 2. Azure Bicep
O que é?
O Azure Bicep é uma linguagem de infraestrutura como código (IaC) desenvolvida pela Microsoft, que simplifica a criação de modelos do Azure Resource Manager (ARM).

Características:
Sintaxe simplificada em comparação com o formato JSON.

100% compatível com ARM.

Suporte a validação e intellisense para facilitar a escrita de scripts.

Melhor legibilidade e menos verboso do que JSON.

🔧 3. Terraform
O que é?
O Terraform é uma ferramenta de infraestrutura como código (IaC) de código aberto que permite criar, modificar e versionar a infraestrutura de maneira segura e eficiente. Embora o Terraform seja multi-cloud, ele também oferece integração nativa com o Azure.

Características:
Suporta várias plataformas de nuvem: Azure, AWS, GCP, entre outras.

State files: Mantém o estado da infraestrutura e detecta mudanças.

Modularidade: Facilita a reutilização de código.

HCL (HashiCorp Configuration Language): Linguagem própria para definição de infraestrutura.

🔧 4. Azure DevOps
O que é?
Azure DevOps é um conjunto de serviços para planejamento de projetos, desenvolvimento, teste e implantação de aplicativos.

Características:
Pipelines de CI/CD: Automatiza o ciclo de vida de desenvolvimento e implantação.

Repos Git: Controle de versão e colaboração de código.

Boards: Gerenciamento de tarefas e backlog de projetos.

Artifactory: Gerenciamento de pacotes e dependências.

🔧 5. GitHub Actions
O que é?
GitHub Actions permite automatizar fluxos de trabalho de integração e entrega contínua (CI/CD) diretamente no GitHub.

Características:
Automação baseada em GitHub: Integra-se diretamente ao repositório do GitHub.

Customização: Criação de workflows para testes, builds e deploys.

Suporte a múltiplos ambientes e múltiplas nuvens, incluindo o Azure.

🔧 6. Azure CLI (Command-Line Interface)
O que é?
A Azure CLI é uma ferramenta de linha de comando que facilita o gerenciamento e a automação de tarefas do Azure. Ela permite que você implante e gerencie recursos do Azure diretamente do terminal.

Características:
Fácil de usar para quem prefere linha de comando.

Cross-platform: Funciona no Windows, Linux e macOS.

Integração com scripts e automação.

Apoio completo ao gerenciamento de recursos do Azure.

🔧 7. Azure PowerShell
O que é?
Azure PowerShell é um conjunto de cmdlets para gerenciar e automatizar recursos do Azure usando o PowerShell.

Características:
Automação de tarefas do Azure diretamente via PowerShell.

Suporte completo a recursos e operações do Azure.

Compatível com scripts e tarefas de automação em ambientes Windows.

Uso intensivo em ambientes corporativos que já adotam PowerShell como ferramenta principal.

🔧 8. Azure Automation
O que é?
Azure Automation é uma plataforma de automação e gerenciamento que permite implantar, gerenciar e monitorar a infraestrutura e recursos do Azure.

Características:
Runbooks: Scripts que automatizam tarefas repetitivas.

Gerenciamento de patches: Automatiza a instalação de patches em máquinas virtuais.

Azure Automation State Configuration: Configuração e gerenciamento de máquinas com base em políticas.

🔧 9. Azure Resource Mover
O que é?
O Azure Resource Mover é uma ferramenta para mover recursos de um datacenter do Azure para outro dentro da mesma região ou entre regiões diferentes, sem precisar desimplantar e recriar os recursos.

Características:
Mover recursos de forma simples.

Minimizar downtime durante o processo de movimentação.

Suporte a vários tipos de recursos (VMs, redes, etc.).

🔧 10. Azure Site Recovery
O que é?
O Azure Site Recovery permite recuperação de desastres e continuidade de negócios para máquinas virtuais e outros serviços.

Características:
Replicação de dados e máquinas virtuais para uma região de recuperação.

Failover automatizado em caso de falhas graves.

Suporte a ambientes híbridos e multi-nuvem.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
No Azure, os dashboards são ferramentas essenciais para monitorar e gerenciar seus recursos e serviços. Quatro componentes-chave que oferecem insights detalhados e personalizados são o Azure Monitor, o Azure Service Health, o Azure Advisor e os dashboards personalizados.​

1. Azure Monitor:

O Azure Monitor é uma solução abrangente de monitoramento que coleta, analisa e responde a dados de monitoramento de seus ambientes na nuvem e locais. Ele ajuda a maximizar a disponibilidade e o desempenho de seus aplicativos e serviços, fornecendo insights sobre a operação e a integridade de seus recursos. O Monitor coleta dados de métricas, logs e eventos, permitindo que você visualize e analise o desempenho de suas aplicações e infraestrutura. ​

2. Azure Service Health:

O Azure Service Health mantém você informado sobre incidentes de serviço, manutenção planejada e avisos de saúde que podem afetar seus recursos do Azure. Ele oferece alertas personalizados e orientações para ajudá-lo a responder rapidamente a problemas que impactam seus serviços. Com o Service Health, você pode configurar alertas para ser notificado sobre problemas ativos e manutenção futura, garantindo que sua equipe esteja sempre informada sobre o estado dos serviços. ​

3. Azure Advisor:

O Azure Advisor é um serviço que fornece recomendações personalizadas para ajudar a melhorar a confiabilidade, segurança e desempenho de seus recursos do Azure. Ele analisa suas configurações e uso do Azure para oferecer sugestões práticas que podem economizar custos e aprimorar a eficiência operacional. As recomendações cobrem áreas como alta disponibilidade, segurança, desempenho e eficiência de custo.​

4. Dashboards Personalizados:

No Azure, você pode criar dashboards personalizados no portal para exibir visualmente dados relevantes de monitoramento, métricas e alertas. Esses dashboards podem incluir gráficos, métricas e logs que fornecem uma visão consolidada do estado e desempenho de seus recursos. Por exemplo, você pode criar um dashboard que combine métricas de desempenho do Azure Monitor com alertas do Service Health e recomendações do Advisor, oferecendo uma visão holística de seu ambiente. ​

Integrando e utilizando esses componentes, você pode obter uma visão completa e detalhada do estado de seus serviços no Azure, permitindo uma gestão proativa e informada de seus recursos.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------


