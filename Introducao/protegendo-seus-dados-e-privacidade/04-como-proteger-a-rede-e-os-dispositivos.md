# 3.1 Como proteger a rede e os dispositivos

> Diário de estudos - módulo "Protegendo seus Dados e Privacidade"

Até aqui os estudos mostraram os ataques, ou seja, o "lado ruim". Agora começa o "lado bom", como se proteger de tudo isso. Esse tópico é bem prático, dá pra aplicar cada dica direto no seu próprio computador, celular e roteador de casa.

## 3.1.1 O que você acha?

Atividade de abertura do tópico, só pra fazer você pensar um pouco antes de entrar no conteúdo. Não tem teoria nova aqui, é tipo um aquecimento antes da aula de verdade começar.

## 3.1.2 Proteger seus dispositivos de computação

**Explicando do zero**
Todo aparelho que se conecta à internet, seja computador, celular ou tablet, precisa de camadas de proteção. Pensa assim, sua casa não tem só uma porta trancada, ela tem porta trancada, alarme, câmera. Com o dispositivo é a mesma lógica, cada proteção cobre um tipo de risco diferente.

**As camadas de proteção, uma por uma**

- **Firewall** - imagina um segurança na entrada de um prédio, verificando quem pode entrar e quem não pode. O firewall faz isso com o tráfego de internet, ele fica entre o seu dispositivo e a rede, bloqueando conexões suspeitas antes delas chegarem até você. A maioria dos sistemas operacionais já vem com um firewall básico ativado
- **Antivírus e antimalware** - são programas que vasculham o dispositivo procurando arquivos maliciosos conhecidos, tipo um vigia que reconhece a cara de bandidos já fichados. Só que pra esse vigia continuar reconhecendo os bandidos novos, ele precisa de atualização constante, porque malware novo aparece toda hora
- **Manter tudo atualizado** - sistema operacional e aplicativos recebem atualizações que corrigem falhas de segurança descobertas depois que o programa já foi lançado (lembra do que vimos sobre vulnerabilidades de software?). Adiar uma atualização é literalmente deixar uma porta conhecida destrancada
- **Backup** - é ter uma cópia dos seus arquivos guardada em outro lugar, tipo um HD externo ou a nuvem. Se o dispositivo for infectado, roubado ou simplesmente quebrar, você não perde tudo de uma vez
- **Criptografia de disco** - embaralha os dados guardados no aparelho de um jeito que só quem tem a senha certa consegue ler. Mesmo que alguém roube o dispositivo fisicamente e tente tirar o disco pra ler os arquivos direto, sem a chave certa os dados ficam ilegíveis

## 3.1.3 Segurança da rede sem fio em casa

**Explicando do zero**
O roteador é a porta de entrada da internet na sua casa. Se ele fica mal protegido, é como deixar o portão de casa aberto, qualquer um de fora pode tentar entrar e usar sua rede, ou pior, espionar o que passa por ela.

**Os cuidados básicos, um por um**

- **Trocar a senha padrão do roteador** - todo roteador sai de fábrica com um usuário e senha padrão pra configuração (tipo "admin" e "admin"). Essas senhas padrão são conhecidas publicamente, então não trocar isso é basicamente deixar a fechadura da porta destravada de propósito
- **Usar criptografia forte (WPA3 ou WPA2)** - isso embaralha o sinal WiFi, dificultando que alguém de fora, sem saber a senha, consiga captar e entender o que tá passando pela rede
- **Trocar o nome da rede (SSID)** - o nome padrão de fábrica costuma revelar o modelo do roteador. Isso ajuda um atacante a pesquisar exatamente quais falhas aquele modelo específico tem
- **Desligar o que não usa** - funções como conexão por botão (WPS) ou acesso remoto ao roteador, se você nunca usa, é melhor deixar desligado. Cada função ativa é mais uma porta possível de entrada

## 3.1.4 Riscos públicos de Wi-Fi

**Explicando do zero**
WiFi público (aeroporto, shopping, cafeteria) é bom porque é gratuito e aberto, mas essa mesma característica é o problema, ele é aberto pra todo mundo, inclusive gente mal-intencionada conectada na mesma rede que você.

**Por que isso é arriscado**
Lembra do ataque On-Path que vimos, aquele em que o invasor se posiciona no meio da sua comunicação? Numa rede pública, isso fica bem mais fácil de acontecer, porque o atacante só precisa estar conectado ali perto, na mesma rede.

Tem também um golpe chamado rede falsa, o atacante cria um ponto de WiFi com nome parecido com o legítimo, tipo "WiFi_Shopping_Gratis", e espera a vítima se conectar sem perceber que na verdade caiu numa rede controlada por ele.

**Como se proteger nessa situação**
Evite acessar coisa sensível, tipo banco ou email importante, enquanto tiver conectado numa rede pública. Se puder, use uma VPN, que cria um "túnel" criptografado pro seu tráfego, dificultando bastante que alguém consiga espiar o que você tá fazendo, mesmo numa rede insegura.

## 3.1.5 Segurança de senha

**Explicando do zero**
A senha é a chave da porta de qualquer conta sua. Não importa quanta segurança um serviço tenha por trás, se a senha for fraca, é como ter um cofre reforçado com a chave debaixo do tapete.

## 3.1.6 Uma Senha Forte

**O que faz uma senha ser forte**
Lá no tópico de tempos de cracking vimos que quebrar uma senha por força bruta depende do tamanho dela e da variedade de caracteres. É basicamente a mesma lógica aqui, quanto mais longa e mais variada, mais tempo um atacante vai levar pra tentar todas as combinações possíveis.

**Checklist de uma senha forte**

- Ter pelo menos 12 caracteres, o ideal é passar disso
- Misturar letra maiúscula, minúscula, número e símbolo
- Não usar coisa óbvia sobre você, tipo data de nascimento, nome de time ou nome de familiar
- Ser diferente em cada conta, nunca repetir a mesma senha em serviços diferentes

## 3.1.7 Usando uma frase secreta

**Explicando do zero**
Frase secreta (passphrase) é uma alternativa à senha comum. Em vez de uma sequência de caracteres aleatórios que ninguém consegue guardar de cabeça, tipo "K9$mPz2!qL", você usa uma frase inteira, juntando várias palavras que não têm relação óbvia entre si.

**Por que isso é bom**
Uma frase é naturalmente mais longa que uma senha comum, e como já vimos, tamanho é um dos fatores que mais aumenta o tempo de quebra por força bruta. Um exemplo do conceito, uma frase tipo "CachorroAzulComeSeteBananas" é mais longa e mais difícil de quebrar do que uma senha curta cheia de símbolos, e ao mesmo tempo é bem mais fácil de lembrar.

## 3.1.8 Diretrizes de Senha

**Explicando do zero**
Depois de entender o que faz uma senha forte, essas são as regras práticas pra aplicar isso no dia a dia com todas as suas contas.

**As regras principais**

- Usar senha ou frase secreta longa, com bastante variedade de caracteres
- Nunca repetir a mesma senha em sites diferentes. Se um site vazar os dados dele, toda conta que usa aquela mesma senha fica em risco também
- Trocar senha de vez em quando, principalmente se desconfiar de algum vazamento
- Usar um gerenciador de senhas, um programa que guarda e ainda gera senhas fortes pra você, assim não precisa decorar dezenas delas
- Ativar a verificação em duas etapas sempre que o serviço oferecer. Isso adiciona uma segunda trava além da senha, tipo um código que chega no seu celular

**As diretrizes oficiais do NIST**
O NIST (National Institute of Standards and Technology, um instituto do governo dos Estados Unidos) publica um documento chamado SP 800-63B, que virou a referência mais usada no mundo todo sobre como definir regras de senha. Mesmo tendo sido escrito pensando em agências do governo americano, empresas de todo tipo de área acabaram adotando essas recomendações como padrão de mercado.

A versão mais recente desse documento, finalizada em 2025, mudou bastante coisa que era considerada "regra de ouro" até pouco tempo atrás. Os pontos principais:

- **Tamanho importa mais que complexidade** - o NIST recomenda pelo menos 8 caracteres como mínimo, mas incentiva usar 15 caracteres ou mais quando possível, e os sistemas devem aceitar senhas de até 64 caracteres. Isso favorece bastante o uso de frases secretas, que vimos lá em cima
- **Chega de regra obrigando misturar tipo de caractere** - o documento recomenda que sistemas não obriguem mais o famoso "sua senha precisa ter maiúscula, número e símbolo". Essa exigência, na prática, faz muita gente criar senhas previsíveis só pra cumprir a regra, tipo trocar o "a" por "@"
- **Chega de trocar senha por trocar** - forçar troca de senha a cada 90 dias, sem motivo nenhum, caiu de recomendação. A pesquisa mostrou que isso só faz as pessoas criarem senhas fracas e parecidas com a anterior. A troca só é recomendada quando existe suspeita real de vazamento
- **Checagem contra senhas já vazadas** - o sistema deve comparar a senha escolhida com uma lista de senhas conhecidas por já terem vazado ou serem muito usadas, e recusar se ela aparecer nessa lista
- **Fim das dicas de senha e perguntas de segurança** - perguntas tipo "nome do seu primeiro animal de estimação" saíram de recomendação, porque geralmente são informações fáceis de descobrir sobre alguém
- **Incentivo forte à autenticação multifator** - o documento reforça que senha sozinha não deveria ser a única camada de proteção numa conta importante

## 3.1.9 Verificação de senha

**Explicando do zero**
Depois de criar uma senha, dá pra checar de fato se ela é forte ou fraca antes de usar de verdade.

**Como isso funciona na prática**
Existem ferramentas e sites feitos justamente pra isso, eles analisam a senha e estimam quanto tempo um ataque de força bruta levaria pra quebrar ela, baseado no tamanho e na variedade de caracteres usados.

Também existem serviços que checam se aquela senha específica já apareceu em algum vazamento de dados conhecido, publicado na internet depois de algum ataque a outro site. Se ela já vazou antes, é um sinal forte de que não deve ser usada de jeito nenhum, mesmo que pareça complexa à primeira vista.
