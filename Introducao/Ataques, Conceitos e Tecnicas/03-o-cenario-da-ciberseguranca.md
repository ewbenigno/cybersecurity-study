# O Cenário da Cibersegurança

> Diário de estudos - módulo "Ataques, Conceitos e Técnicas"

Esse tópico fala sobre criptomoeda, que por si só não é uma ameaça, mas virou alvo de um tipo específico de ataque chamado cryptojacking. Pra entender o ataque, primeiro precisa entender como a criptomoeda funciona por trás dos panos.

## Criptomoeda

**O que é**
Criptomoeda é dinheiro digital, ou seja, não existe em forma física como uma nota ou moeda de metal. Ela usa técnicas fortes de criptografia (embaralhamento de dados) pra proteger as transações feitas online. Diferente do dinheiro tradicional, não existe um banco central controlando ela, o próprio sistema é descentralizado.

Isso já virou coisa séria no mercado, tanto que bancos, governos e até empresas grandes como Microsoft e AT&T já demonstraram interesse e estão de olho nesse mundo das criptomoedas.

**Onde o dinheiro fica guardado**
Quem tem criptomoeda guarda ela em "carteiras" digitais, que também são protegidas por criptografia. Quando duas pessoas fazem uma transação, ou seja, uma manda dinheiro pra outra, os detalhes dessa transação são registrados num sistema de contabilidade descentralizado chamado blockchain.

Duas características importantes desse sistema:

- **Anonimato parcial** - a transação não expõe diretamente a identidade das pessoas envolvidas, só fica registrado o que foi feito, não necessariamente quem fez
- **Sem intermediário** - o sistema é autogerenciado, quer dizer que não existe um banco central nem uma entidade do governo controlando ou aprovando cada transação, como acontece numa transferência bancária comum

**Como uma transação é confirmada, o processo de mineração**
Pra uma transação de criptomoeda ser validada e entrar de fato no sistema, ela passa por um processo técnico chamado mineração. Funciona mais ou menos assim, em passos:

1. A cada dez minutos, mais ou menos, computadores especiais coletam dados sobre as transações mais recentes que aconteceram
2. Esses dados são transformados em quebra-cabeças matemáticos bem complexos, o que ajuda a manter a confidencialidade do sistema
3. Um grupo de computadores conhecidos como "mineradores" trabalha resolvendo esses quebra-cabeças matemáticos, usando bastante poder de processamento pra isso. É esse trabalho que confirma e autentica as transações
4. Depois que a transação é verificada, o "razão" (o registro de todas as transações, também chamado de ledger) é atualizado e copiado pra todo mundo que faz parte da rede blockchain no mundo inteiro, o que finaliza a transação

O nome "mineração" existe porque, assim como minerar ouro exige esforço pra encontrar algo valioso, minerar criptomoeda exige poder computacional pra resolver aqueles quebra-cabeças e "extrair" a recompensa em moeda digital.

## Cryptojacking

**O que é**
Cryptojacking é um tipo de ameaça relativamente nova que se esconde dentro do computador, celular, tablet, notebook ou até servidor de alguém, sem que essa pessoa saiba. O invasor usa o poder de processamento daquela máquina infectada pra minerar criptomoeda, só que sem pedir consentimento nenhum do dono do dispositivo.

**Como isso afeta a vítima**
Lembra do processo de mineração que vimos no tópico anterior? Ele exige bastante poder de processamento pra resolver aqueles quebra-cabeças matemáticos. No cryptojacking, em vez do atacante usar o próprio computador dele pra minerar, ele "sequestra" a capacidade de processamento de outras máquinas infectadas, fazendo elas trabalharem pra ele de graça, enquanto a vítima só percebe o computador mais lento ou a bateria acabando mais rápido, sem entender o motivo.

**Por que é difícil de perceber**
O detalhe mais preocupante desse ataque é que ele é bem discreto. Muitas vítimas de cryptojacking nem sabiam que tinham sido invadidas até que já fosse tarde demais, já que o malware fica rodando escondido em segundo plano, sem travar o sistema de forma óbvia nem chamar muita atenção logo de cara.
