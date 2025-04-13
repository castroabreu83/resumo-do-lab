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


