# Abordagem comportamental à segurança cibernética

> Diário de estudos - módulo "Protegendo a Organização"

O tópico anterior mostrou as ferramentas (firewall, IDS/IPS, antimalware). Esse aqui mostra outro jeito de enxergar segurança, olhando pro comportamento da rede como um todo, testando as próprias defesas de propósito e entendendo como lidar com o risco que sempre vai existir, por mais protegida que uma organização esteja.

## Segurança baseada em comportamento

**Explicando do zero**
Até aqui, boa parte da defesa que vimos funciona comparando o que acontece na rede com uma lista de ameaças já conhecidas, tipo reconhecer a cara de bandidos já fichados. Segurança baseada em comportamento funciona diferente, ela aprende qual é o padrão normal de uma rede específica e passa a desconfiar de qualquer coisa que fuja desse padrão, mesmo que aquela ameaça específica nunca tenha sido vista antes.

**Como isso funciona na prática**
O sistema observa, por um tempo, como a rede se comporta normalmente, coisas como que horário tem mais tráfego, quais dispositivos costumam se comunicar entre si, e qual volume de dado é considerado normal. Depois que esse "normal" é estabelecido, qualquer desvio relevante desse padrão dispara um alerta, mesmo sem existir uma assinatura de ataque conhecida por trás daquele comportamento estranho.

**Por que isso complementa as ferramentas tradicionais**
Ameaças novas, que ainda não foram catalogadas em nenhuma lista de ameaça conhecida, conseguem passar despercebidas por sistemas que só comparam com assinaturas já existentes. A análise de comportamento ajuda a pegar justamente esse tipo de ameaça inédita, porque ela não depende de já conhecer o ataque específico, só precisa perceber que algo tá fora do padrão normal.

## NetFlow

**Explicando do zero**
NetFlow é uma tecnologia, criada originalmente pela Cisco, usada pra coletar informação sobre o tráfego que passa por uma rede. Pensa nele como um resumo detalhado de tudo que trafegou por ali, sem precisar guardar o conteúdo completo de cada pacote de dado.

**O que o NetFlow registra**
Ele guarda metadados da comunicação, como endereço de origem e destino, quais portas foram usadas, quanto tempo durou a conexão e quanto dado foi transferido. Ou seja, ele registra o "quem falou com quem, quando e quanto", sem necessariamente guardar o "o que foi dito" em detalhe.

**Pra que isso serve na segurança**
Esses dados coletados pelo NetFlow alimentam justamente a segurança baseada em comportamento que vimos no tópico anterior. Analisando esse histórico de tráfego, dá pra identificar padrões anormais, tipo um dispositivo que de repente começa a mandar uma quantidade enorme de dado pra um destino desconhecido, o que pode ser sinal de uma máquina comprometida ou parte de uma botnet.

## Teste de penetração

**Explicando do zero**
Teste de penetração (pentest) é quando uma organização contrata alguém especializado pra tentar invadir a própria rede de propósito, simulando o que um atacante real faria, mas de forma autorizada e controlada.

**Por que fazer isso**
A lógica é simples, é melhor descobrir as próprias falhas através de alguém contratado pra isso, do que deixar um atacante de verdade descobrir primeiro. O profissional que faz esse trabalho é chamado de pentester, e ele usa as mesmas técnicas e ferramentas que um invasor malicioso usaria, incluindo varredura de portas, engenharia social e exploração de vulnerabilidades conhecidas.

**Como isso costuma funcionar**
No final do teste, o pentester entrega um relatório detalhado pra organização, listando todas as vulnerabilidades encontradas, o quão sério cada uma é, e recomendações de como corrigir cada problema antes que alguém mal-intencionado explore aquilo de verdade.

## Redução do impacto

**Explicando do zero**
Por mais que uma organização invista em prevenção, é praticamente impossível bloquear cem por cento dos ataques. Redução do impacto é sobre se preparar pra minimizar o estrago quando um incidente realmente acontece, em vez de focar só em tentar impedir que ele aconteça.

**Estratégias comuns de redução de impacto**

- **Segmentação de rede** - dividir a rede em partes isoladas entre si, de forma que, se um invasor comprometer uma parte, ele não consiga automaticamente alcançar todo o resto
- **Princípio do menor privilégio** - dar a cada pessoa e sistema só o acesso mínimo necessário pra fazer o trabalho dela, assim, se uma conta for comprometida, o dano fica limitado ao que aquela conta específica tinha permissão de acessar
- **Plano de resposta a incidentes** - já vimos esse conceito antes, ter um passo a passo definido de antemão de como agir durante um ataque reduz bastante o tempo de reação e, consequentemente, o tamanho do dano
- **Backups regulares** - lembra do tópico de manutenção de dados? Ter cópia de segurança é uma das formas mais diretas de reduzir o impacto de um ataque tipo ransomware, já que dá pra restaurar os dados sem precisar pagar resgate nenhum

## O que é gerenciamento de risco?

**Explicando do zero**
Gerenciamento de risco é o processo de identificar, avaliar e decidir o que fazer com os riscos de segurança que uma organização enfrenta. Como proteção total e perfeita não existe, toda organização precisa decidir, de forma consciente, quais riscos ela vai tratar, e como.

**As formas de lidar com um risco identificado**

- **Evitar o risco** - eliminar completamente a atividade ou sistema que gera aquele risco
- **Reduzir o risco** - aplicar controles de segurança (como os que vimos ao longo do curso) pra diminuir a chance ou o impacto daquele risco acontecer
- **Transferir o risco** - repassar o risco pra outra parte, por exemplo contratando um seguro cibernético que cobre prejuízo em caso de ataque
- **Aceitar o risco** - em alguns casos, o custo de se proteger contra um risco específico é maior do que o próprio prejuízo esperado caso ele aconteça, e a organização decide conscientemente conviver com aquele risco

**Por que isso é importante**
Gerenciamento de risco ajuda uma organização a investir os recursos de segurança dela de forma mais inteligente, focando primeiro nos riscos mais graves e mais prováveis de acontecer, em vez de tentar proteger tudo igualmente, o que na prática seria caro demais e pouco eficiente.

---

## Glossário

- **Segurança baseada em comportamento** - abordagem que aprende o padrão normal de uma rede e alerta sobre qualquer desvio relevante desse padrão
- **Assinatura de ataque** - padrão específico já conhecido, usado por sistemas de segurança tradicionais pra reconhecer uma ameaça já catalogada
- **NetFlow** - tecnologia que coleta metadados sobre o tráfego de uma rede, como origem, destino e volume de dados, sem guardar o conteúdo completo
- **Teste de penetração (pentest)** - simulação autorizada de um ataque real, feita por um profissional contratado, pra encontrar vulnerabilidades antes de um invasor real
- **Pentester** - profissional especializado em realizar testes de penetração
- **Segmentação de rede** - prática de dividir uma rede em partes isoladas, limitando o alcance de um invasor caso uma parte seja comprometida
- **Princípio do menor privilégio** - conceder a cada pessoa ou sistema apenas o acesso mínimo necessário para realizar sua função
- **Gerenciamento de risco** - processo de identificar, avaliar e decidir como tratar os riscos de segurança de uma organização
- **Seguro cibernético** - apólice contratada por uma organização pra cobrir prejuízos financeiros em caso de incidente de segurança