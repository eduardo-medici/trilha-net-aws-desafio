# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 24/08/2025
Empresa: Farma Red Cross
Responsável: Eduardo Médici 

## Introdução
Este relatório apresenta o processo de implementação de ferramentas AWS na empresa Farma Red Cross, realizado por Eduardo Médici.  
O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de reduzir custos operacionais e aumentar a eficiência no processo de distribuição de medicamentos para empresas e farmácias parceiras.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos.  
A seguir, serão descritas as etapas do projeto:

### Etapa 1
- **Nome da ferramenta:** Amazon S3 (Simple Storage Service)  
- **Foco da ferramenta:** Armazenamento de dados e documentos em nuvem  
- **Descrição de caso de uso:**
  Com a utilização do Amazon S3 é possível organizar os dados da empresa Farma Red Cross, em buckets separados, de acordo com o tipo (como histórico de vendas, notas fiscais e relatórios). Cada bucket pode ter políticas de acesso diferentes, garantindo que apenas equipes autorizadas consigam ler ou escrever arquivos. Também é possível habilitar o Versioning para manter o histórico de alterações em documentos críticos, como notas fiscais ou relatórios.
  1. **Redução de custos:** elimina a necessidade de servidores locais caros para armazenamento de dados (como histórico de vendas, notas fiscais e relatórios).  
  2. **Principal ganho:** escalabilidade automática e alta durabilidade dos dados, garantindo segurança e disponibilidade sem investimento em infraestrutura física.  

### Etapa 2
- **Nome da ferramenta:** Amazon RDS (Relational Database Service)  
- **Foco da ferramenta:** Gerenciamento de banco de dados relacional em nuvem  
- **Descrição de caso de uso:**
  A a utilização do Amazon RDS serve para gerenciar bancos de dados relacionais na nuvem de forma mais simples, segura e escalável, sem a necessidade de se preocupar com a infraestrutura física. Ele permite que a empresa tenha um banco de dados robusto, escalável e seguro, mas sem precisar investir pesado em servidores físicos, licenças de software ou equipe de TI dedicada. O pagamento é sob demanda, o que significa que você só paga pelo que usa. Por meio dele é possível centralizar dados de estoque, pedidos e logística, garantindo integridade e performance.
  1. **Redução de custos:** diminui despesas com manutenção e licenciamento de banco de dados on-premises, além de reduzir custos de equipe técnica para administração.  
  2. **Principal ganho:** maior performance e disponibilidade dos dados de estoque e logística, essenciais para o papel da empresa como hub de distribuição.  

### Etapa 3
- **Nome da ferramenta:** AWS Auto Scaling + EC2 + ELB
- **Foco da ferramenta:** Dimensionamento automático de servidores de acordo com a demanda  
- **Descrição de caso de uso:**
  A junção do uso de EC2 + Auto Scaling + ELB mantém sistemas web e APIs estáveis, ajustando automaticamente a capacidade computacional conforme a demanda. Isso funciona pelo ajuste automático do número de instâncias, que aumenta quando a demanda sobe (ex: horário de pico de pedidos) e diminui quando a demanda cai, economizando custos. Pode-se realizar a integração com o ELB que redistribui as requisições conforme a necessidade. Exemplo de fluxo: Recebimento de pedidos aumenta às 12h → Auto Scaling cria novas instâncias EC2 → ELB distribui requisições → Após o pico, instâncias desnecessárias são encerradas automaticamente.
  1. **Redução de custos:** permite pagar apenas pelos recursos computacionais utilizados, evitando custos fixos altos em períodos de baixa demanda.  
  2. **Principal ganho:** alta disponibilidade e desempenho estável para aplicações críticas, como sistemas de pedidos e integração com farmácias e distribuidores.  

## Conclusão
A implementação de ferramentas na empresa Farma Red Cross tem como esperado **reduzir custos com infraestrutura física, otimizar processos de armazenamento e banco de dados, além de melhorar a escalabilidade dos sistemas críticos**, o que aumentará a eficiência e a produtividade da empresa.  

Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.  

Assinatura do Responsável pelo Projeto:  
Eduardo Médici 
