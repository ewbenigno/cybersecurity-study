# Dispositivos e Tecnologias de segurança cibernética

> Diário de estudos - módulo "Protegendo a Organização"

Começa aqui o módulo 4, que muda o foco de "proteger você mesmo" pra "proteger uma organização inteira". Esse primeiro tópico apresenta as ferramentas e tecnologias que empresas usam pra defender suas redes, desde equipamentos físicos até sistemas que detectam ataque em tempo real.

## Dispositivos de segurança

**Explicando do zero**
Assim como uma empresa física tem porteiro, câmera e alarme, uma rede de computadores também tem seus próprios "guardas" especializados. Dispositivos de segurança são equipamentos, físicos ou virtuais, dedicados a proteger a rede de uma organização.

**Os tipos mais comuns**

- **Firewall dedicado** - um equipamento próprio, separado, cuja única função é filtrar o tráfego que entra e sai da rede
- **Roteador com recursos de segurança** - além de simplesmente rotear o tráfego, alguns roteadores empresariais já vêm com camadas extras de proteção embutidas
- **Sistema de detecção e prevenção de intrusos (IDS/IPS)** - equipamento dedicado a identificar e, em alguns casos, bloquear atividade suspeita na rede, algo que vamos ver com mais detalhe daqui a pouco
- **VPN dedicada** - equipamento que gerencia conexões seguras e criptografadas entre a rede da empresa e usuários remotos

## Firewalls

**Explicando do zero**
Já vimos o conceito de firewall lá no tópico de proteção de dispositivo pessoal, mas aqui ele aparece em escala empresarial, protegendo uma rede inteira, não só um único computador.

**Como um firewall decide o que bloquear**
Um firewall funciona verificando o tráfego que passa por ele, comparando com um conjunto de regras definidas, e decidindo se aquele tráfego pode passar ou deve ser bloqueado. É tipo uma lista de convidados na porta de um evento, só entra quem tá na lista, ou quem se encaixa nas condições liberadas.

**Tipos de firewall**

- **Firewall de filtragem de pacotes** - o tipo mais básico, examina cada pacote de dado isoladamente, olhando informação como endereço de origem e destino, sem entender o contexto da conversa inteira
- **Firewall de inspeção com estado (stateful)** - mais avançado que o anterior, ele acompanha o estado das conexões ativas, entendendo o contexto completo de uma comunicação, não só pacotes isolados
- **Firewall de próxima geração (NGFW)** - além de filtrar tráfego, consegue inspecionar o conteúdo dos dados de forma mais profunda, identificando aplicativos específicos e ameaças mais sofisticadas escondidas dentro do tráfego permitido

## Varredura de portas

**Explicando do zero**
Pensa numa casa com várias portas e janelas. Varredura de portas (port scanning) é o processo de testar, uma por uma, quais dessas "portas" de um sistema estão abertas, fechadas ou filtradas.

**O que é uma "porta" nesse contexto**
Em redes de computador, uma porta é um número que identifica qual serviço específico tá rodando numa máquina, esperando conexão. Por exemplo, a porta 80 costuma ser usada por sites, a porta 443 por sites com conexão segura (HTTPS). Cada porta aberta é um serviço ativo que pode, em teoria, ser acessado de fora.

**Pra que serve a varredura de portas**
Ela é usada tanto pelo lado da defesa quanto pelo lado do ataque. Profissionais de segurança usam pra descobrir quais portas de um sistema próprio estão abertas sem necessidade, e fechar as que não deveriam estar expostas. Já um atacante usa pra mapear quais portas de um alvo estão abertas, tentando encontrar um serviço vulnerável pra explorar.

## Sistemas de detecção e prevenção de intrusos

**Explicando do zero**
Além do firewall, que decide o que pode ou não entrar na rede baseado em regras, existem sistemas dedicados especificamente a identificar comportamento suspeito que já conseguiu passar, ou que tá tentando passar.

**IDS, Sistema de Detecção de Intrusos**
Um IDS (Intrusion Detection System) monitora o tráfego da rede procurando por sinais de atividade maliciosa, mas o trabalho dele é só de vigilância e alerta, ele não bloqueia nada sozinho. É tipo uma câmera de segurança, ela grava e avisa, mas quem age depois é outra pessoa.

**IPS, Sistema de Prevenção de Intrusos**
Um IPS (Intrusion Prevention System) vai um passo além. Além de detectar a atividade suspeita, ele consegue agir automaticamente pra bloquear aquele tráfego malicioso em tempo real, sem esperar intervenção humana. É como se, além da câmera, tivesse também um segurança que fecha a porta assim que percebe alguém suspeito se aproximando.

## Detecção em tempo real

**Explicando do zero**
Detecção em tempo real é a capacidade de identificar uma ameaça no exato momento em que ela acontece, ou o mais próximo disso possível, em vez de descobrir só depois, analisando registros antigos.

**Por que isso é tão importante**
Quanto mais rápido uma ameaça é identificada, menor a chance dela causar dano grande. Lembra das APTs (ameaças persistentes avançadas) que vimos lá atrás, que ficam escondidas por meses coletando dado aos poucos? Um sistema de detecção em tempo real bem configurado é justamente o que ajuda a identificar esse tipo de comportamento mais cedo, antes que o estrago fique enorme.

**O que costuma alimentar esse tipo de detecção**
Sistemas modernos de detecção em tempo real costumam usar uma combinação de regras pré-definidas (padrões já conhecidos de ataque) com análise de comportamento (identificar quando algo foge do padrão normal daquela rede específica), o que ajuda a pegar até ameaças novas, que ainda não tinham sido catalogadas antes.

## Proteção contra Malware

**Explicando do zero**
Malware é qualquer tipo de software malicioso, seja vírus, worm, trojan, ransomware, entre outros. Proteção contra malware em nível organizacional funciona parecido com o antivírus pessoal que já vimos, só que em escala bem maior, cobrindo todos os dispositivos conectados à rede da empresa de uma vez.

**Camadas comuns de proteção contra malware numa organização**

- Antivírus e antimalware instalados em todos os dispositivos da rede, gerenciados de forma centralizada
- Filtragem de email, bloqueando anexos e links maliciosos antes mesmo deles chegarem na caixa de entrada de um funcionário
- Sandboxing, uma técnica que executa arquivos suspeitos num ambiente isolado e controlado primeiro, pra observar o comportamento deles antes de liberar no sistema real
- Atualização automática e centralizada de definições de vírus e patches de segurança em todos os dispositivos

## Práticas recomendadas de segurança

**Explicando do zero**
Fechando o tópico, esse último ponto reúne recomendações gerais que uma organização deveria seguir, combinando tudo que foi visto até aqui numa estratégia de defesa mais completa.

**As práticas principais**

- Usar múltiplas camadas de defesa ao mesmo tempo (firewall, IDS/IPS, antimalware), em vez de depender de uma única ferramenta, estratégia conhecida como defesa em profundidade
- Manter todos os sistemas e dispositivos sempre atualizados
- Treinar funcionários regularmente sobre engenharia social e boas práticas de segurança, já que, como vimos, o fator humano continua sendo um dos pontos mais explorados
- Monitorar a rede continuamente, não só configurar as ferramentas uma vez e esquecer
- Ter um plano de resposta a incidentes definido, pra saber exatamente o que fazer caso um ataque realmente aconteça

---

## Glossário

- **Firewall** - dispositivo ou programa que filtra o tráfego de rede, bloqueando conexões que não seguem as regras definidas
- **Porta (rede)** - número que identifica um serviço específico esperando conexão numa máquina, como a porta 443 usada por sites com HTTPS
- **Varredura de portas (port scanning)** - processo de testar quais portas de um sistema estão abertas, fechadas ou filtradas
- **IDS (Intrusion Detection System)** - sistema que monitora a rede e alerta sobre atividade suspeita, sem bloquear automaticamente
- **IPS (Intrusion Prevention System)** - sistema que detecta e também bloqueia automaticamente tráfego malicioso em tempo real
- **Detecção em tempo real** - capacidade de identificar uma ameaça no momento em que ela acontece, e não só depois através de análise posterior
- **Malware** - termo genérico para qualquer software malicioso, como vírus, worm, trojan ou ransomware
- **Sandboxing** - técnica de executar um arquivo suspeito num ambiente isolado, pra observar seu comportamento antes de liberar no sistema real
- **Defesa em profundidade** - estratégia de usar várias camadas de proteção diferentes ao mesmo tempo, em vez de depender de uma única ferramenta
- **Plano de resposta a incidentes** - conjunto de ações pré-definidas que uma organização segue quando um ataque ou vazamento realmente acontece
