# Métodos de infiltração

> Diário de estudos - módulo "Ataques, Conceitos e Técnicas"

Imagina que um sistema, uma rede ou um dispositivo é tipo uma casa. Infiltração é qualquer jeito que alguém usa pra entrar nessa casa sem ter a chave, sem ter permissão. Às vezes esse "alguém" engana o morador pra ele mesmo abrir a porta. Às vezes ele encontra uma janela mal fechada. Às vezes ele nem tenta entrar, só fica jogando pedra na porta até ela quebrar. Cada tópico abaixo é um jeito diferente de fazer isso.

## Engenharia social

**O que é**
Engenharia social é enganar uma pessoa pra ela mesma entregar algo que não devia, tipo uma senha, um acesso ou uma informação sigilosa.

**Como funciona**
O alvo aqui não é o computador, é o ser humano. O atacante não precisa saber programar nada bonito, ele só precisa ser convincente. Ele cria uma desculpa, uma urgência ou finge ser alguém de confiança, e a vítima ajuda sem perceber que caiu num golpe.

**Formas comuns**

- **Pretexting** - o atacante inventa um personagem ou uma desculpa falsa. Exemplo, liga se passando por "suporte técnico" e pede pra você "confirmar" sua senha
- **Phishing** - um email ou mensagem que parece vir de um banco ou empresa conhecida, pedindo pra clicar num link e digitar seus dados. É o tipo mais comum hoje em dia
- **Something for something (quid pro quo)** - o golpista oferece uma ajuda em troca de algo. Exemplo, "eu resolvo seu problema no PC de graça", e no meio do processo pede acesso remoto
- **Baiting** - deixa uma "isca" física em algum lugar público, tipo um pendrive infectado. A curiosidade faz a pessoa pegar e conectar no computador dela, e o malware entra sozinho

**Por que é perigoso**
Nenhum antivírus ou firewall protege contra isso, porque o problema não é técnico, é humano. A única defesa real é desconfiar de pedidos estranhos, mesmo que pareçam urgentes ou venham de alguém que parece confiável.

## Negação de Serviço (DoS)

**O que é**
DoS vem de "Denial of Service". É um ataque que não rouba nada, ele só quer deixar um site, sistema ou serviço fora do ar, ou tão lento que fica inútil.

**Como funciona**
Existem duas formas principais:

- **Sobrecarga de tráfego** - o atacante manda uma quantidade enorme de requisições pro servidor, muito mais do que ele consegue processar. É tipo lotar a porta de uma loja com gente demais, até ninguém mais conseguir entrar
- **Pacotes malformados** - em vez de mandar muita coisa, o atacante manda dados fora do padrão que o sistema espera. O sistema não sabe lidar com aquilo e trava

## DoS Distribuída (DDoS)

**O que é**
É a versão em grupo do DoS. Em vez de um computador atacando sozinho, são vários ao mesmo tempo, geralmente milhares, todos mandando tráfego pro mesmo alvo junto.

**Por que é pior que um DoS comum**
Duas razões. Primeiro, o volume de ataque é muito maior, então até sistemas bem preparados caem. Segundo, como o tráfego vem de endereços diferentes espalhados pelo mundo, fica bem mais difícil bloquear, porque não dá pra simplesmente banir um único IP.

## Botnet

**O que é**
Uma botnet é uma rede de dispositivos infectados que um invasor controla remotamente, sem o dono de cada aparelho saber. Cada dispositivo dessa rede é chamado de "bot" ou "zumbi".

**Como um dispositivo vira parte disso**
O dono clica num link malicioso ou baixa um arquivo infectado sem perceber. Esse malware fica escondido rodando em segundo plano, esperando ordem de um servidor de controle remoto.

**Por que isso é perigoso**
Sozinho, um dispositivo infectado não parece nada demais. Mas quando o atacante controla milhares deles ao mesmo tempo, ele consegue usar essa força toda junta pra fazer ataques DDoS, mandar spam em massa ou minerar criptomoeda escondido, tudo sem o dono da máquina notar.

Praticamente qualquer coisa conectada à internet pode virar bot, computador, celular, roteador, câmera de segurança, até eletrodoméstico smart.

## Ataques On-Path

**O que é**
Esse ataque também é conhecido pelo nome antigo "man-in-the-middle" (homem no meio). A ideia é o invasor se posicionar bem no meio da comunicação entre duas partes, por exemplo entre você e o site do seu banco, sem que nenhum dos dois perceba.

**Como funciona na prática**
Uma vez posicionado ali, o atacante consegue ler tudo que passa por aquela conexão, e às vezes até alterar os dados antes de entregar pro destino final. É bem comum em redes WiFi públicas mal configuradas, tipo aeroporto ou cafeteria, onde o atacante consegue se meter entre o seu dispositivo e o roteador.

## SEO Poisoning

**O que é SEO primeiro**
SEO significa Search Engine Optimization, que são técnicas usadas pra fazer um site aparecer bem posicionado nos resultados do Google.

**O que é o ataque**
SEO Poisoning é usar essas mesmas técnicas de forma maliciosa, pra fazer sites falsos ou infectados subirem no topo da busca.

**Como o golpe acontece**
A vítima procura algo no Google, tipo "baixar programa X", vê um resultado bem no topo (que parece confiável só por estar em primeiro lugar) e clica sem desconfiar. Só que esse site foi manipulado pra aparecer ali, e na verdade é uma armadilha que instala malware ou rouba dados.

## Quebra de senha de acesso à rede WiFi

**O que é**
São as técnicas usadas pra descobrir a senha de uma rede WiFi protegida sem ter autorização.

**As três formas principais**

- **Engenharia social** - de novo essa técnica aparece, e às vezes é o jeito mais simples, simplesmente perguntar a senha pra alguém ou enganar essa pessoa pra conseguir
- **Ataques de força bruta** - um programa vai testando várias combinações de senha, uma atrás da outra, até acertar
- **Farejamento de rede (network sniffing)** - o atacante fica "escutando" o tráfego que passa pela rede WiFi, capturando os dados. Se a rede usa criptografia fraca ou desatualizada, dá pra extrair a senha analisando esse tráfego capturado

## Ataques de senha

**O que é**
São métodos mais gerais pra tentar quebrar ou adivinhar senha de qualquer tipo de conta, não só WiFi.

**Os três tipos principais**

- **Ataque de dicionário** - o programa testa uma lista enorme de palavras comuns, nomes, datas e combinações que as pessoas costumam usar como senha. Funciona bem contra senhas fracas ou óbvias
- **Força bruta** - diferente do dicionário, aqui o programa testa literalmente todas as combinações possíveis de caracteres, letra por letra, até acertar. É mais lento, mas garante achar a senha em algum momento
- **Ataque de tabela arco-íris (rainbow table)** - as senhas geralmente ficam guardadas de forma criptografada, em um formato chamado "hash", não em texto puro. Esse ataque usa tabelas já prontas com hashes calculados antecipadamente, o que acelera muito o processo de descobrir qual senha corresponde a qual hash

## Tempos de Cracking

**O que é**
"Cracking" aqui é o processo de quebrar uma senha por força bruta. "Tempo de cracking" é quanto tempo isso demora.

**Os dois fatores que definem o tempo**

1. **Tamanho da senha** - quanto mais caracteres, mais combinações possíveis existem, e mais tempo o ataque demora
2. **Variedade de caracteres** - se a senha só tem letras minúsculas, o número de combinações é bem menor do que uma senha que mistura maiúsculas, minúsculas, números e símbolos

**Na prática**
Uma senha curta e simples pode ser quebrada em poucos segundos com os computadores de hoje. Já uma senha longa, com bastante variedade, pode levar anos ou até séculos pra ser quebrada por força bruta.

**Detalhe importante**
O tamanho da senha costuma pesar mais do que a complexidade sozinha. Uma senha de 16 caracteres simples geralmente é mais segura do que uma de 8 caracteres complexa.

## Ameaças persistentes avançadas (APT)

**O que é**
APT vem de "Advanced Persistent Threat". É um tipo de ataque bem diferente dos outros porque não é rápido, ele é planejado pra durar.

**Como funciona**
O invasor consegue entrar na rede de um alvo e fica escondido ali dentro, sem ser detectado, por semanas, meses ou até anos. Durante esse tempo todo, o objetivo é coletar informação aos poucos, com calma, sem levantar suspeita nenhuma.

**Por que é diferente de um DoS**
Um DoS quer causar impacto imediato e visível. Uma APT é o oposto disso, ela quer passar despercebida o máximo de tempo possível.

**Quem costuma sofrer esse ataque**
Alvos de alto valor, como empresas grandes, órgãos do governo ou infraestrutura crítica, porque uma APT exige bastante recurso técnico e financeiro pra ser executada. Normalmente por trás dela tem um grupo organizado, não uma pessoa sozinha.
