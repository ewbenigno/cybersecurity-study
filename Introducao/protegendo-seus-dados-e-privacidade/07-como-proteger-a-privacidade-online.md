# Como proteger a privacidade on-line

> Diário de estudos - módulo "Protegendo seus Dados e Privacidade"

Depois de entender quem fica com os seus dados, esse tópico foca em atitudes práticas pra proteger sua privacidade enquanto você navega, usa redes sociais e troca mensagem por email. São hábitos simples, mas que fazem bastante diferença no dia a dia.

## Autenticação de dois fatores

**Explicando do zero**
Pensa numa conta protegida só por senha como uma porta com uma fechadura só. Se alguém descobrir a chave (a senha), entra direto. A autenticação de dois fatores, conhecida também como 2FA, adiciona uma segunda fechadura nessa porta, geralmente de um tipo bem diferente da primeira.

**Como funciona na prática**
Depois de digitar a senha normal (o primeiro fator, que é "algo que você sabe"), o sistema pede uma segunda confirmação, que costuma ser "algo que você tem", tipo:

- Um código enviado por SMS ou por um aplicativo autenticador no celular
- Uma notificação que aparece no celular pra você aprovar o login
- Uma chave de segurança física, um pequeno dispositivo USB feito só pra isso

**Por que isso é tão importante**
Mesmo que um invasor descubra sua senha através de um vazamento ou phishing, ele ainda precisa ter acesso físico ao seu celular ou dispositivo pra completar o segundo fator. Isso torna bem mais difícil alguém entrar na sua conta só com a senha roubada.

## Autorização Aberta

**Explicando do zero**
Você já deve ter visto aquele botão "Entrar com Google" ou "Entrar com Facebook" em vários sites e aplicativos. Isso é possível graças a um sistema chamado OAuth (Open Authorization, ou Autorização Aberta).

**Como funciona**
Em vez de criar uma senha nova pra cada site, o OAuth permite que você use uma conta já existente (Google, Facebook, Apple, entre outras) pra fazer login em outros serviços. O site novo não recebe sua senha do Google, ele recebe só uma permissão limitada, concedida através da conta principal, pra confirmar quem você é e acessar informações específicas que você autorizar.

**O cuidado que isso exige**
É prático, mas cada permissão concedida através do OAuth vale a pena ser revisada de vez em quando. Com o tempo, é fácil acumular um monte de aplicativos com acesso autorizado à sua conta principal, alguns dos quais você nem lembra mais que existem. Se a conta principal (tipo a do Google) for comprometida, todos os serviços conectados a ela ficam em risco também.

## Compartilhamento social

**Explicando do zero**
Redes sociais são feitas pra compartilhar, mas cada informação publicada é também uma informação que sai do seu controle, podendo ser vista, salva ou usada por outras pessoas de um jeito que você não esperava.

**Riscos comuns do compartilhamento**

- Publicar localização em tempo real, revelando onde você está exatamente naquele momento, ou até quando sua casa fica vazia (tipo postar foto de viagem no exato momento em que ela acontece)
- Compartilhar informação pessoal que parece inofensiva, mas que, junta com outros dados públicos, ajuda alguém a montar um perfil detalhado sobre você (isso é usado até em engenharia social, lembra desse conceito?)
- Esquecer que "amigos de amigos" ou configuração de privacidade mal ajustada pode deixar postagens visíveis pra muito mais gente do que você imagina

**Boas práticas**
Revisar quem pode ver o que você posta, evitar compartilhar localização em tempo real e pensar duas vezes antes de publicar informação que, combinada com outras pistas, poderia ser usada contra você.

## Não seja enganado

**Explicando do zero**
Esse tópico volta pro assunto de engenharia social, só que focado especificamente em golpes que acontecem no ambiente online do dia a dia, tipo email e redes sociais.

**Sinais de alerta pra ficar de olho**

- Mensagens que criam urgência, tipo "sua conta será bloqueada em 24 horas, clique aqui"
- Ofertas boas demais pra ser verdade, tipo prêmios que você nunca participou pra ganhar
- Pedidos pra confirmar dados sensíveis por email ou mensagem, coisa que empresa séria raramente faz desse jeito
- Links que, ao passar o mouse por cima, mostram um endereço bem diferente do que o texto sugere

**O hábito que mais ajuda**
Desconfiar por padrão de qualquer pedido inesperado, mesmo que pareça vir de alguém ou de uma empresa confiável, e confirmar por outro canal (tipo ligando direto pra empresa) antes de agir.

## Privacidade de e-mail e navegador da Web

**Explicando do zero**
Email e navegador são duas das ferramentas mais usadas no dia a dia, e também duas das que mais coletam ou expõem dado sobre você sem que perceba.

**Cuidados com o email**

- Não clicar em links ou baixar anexos de remetentes desconhecidos ou suspeitos
- Usar um endereço de email separado só pra cadastros, mantendo o principal mais protegido
- Ativar autenticação de dois fatores também na conta de email, já que ela costuma ser a porta de entrada pra recuperar acesso a outras contas

**Cuidados com o navegador**

- Navegação anônima (ou privada) evita que o histórico e cookies fiquem salvos naquele dispositivo, mas não te torna invisível pra sites, provedor de internet ou empregador
- Cookies são pequenos arquivos que sites usam pra lembrar informação sobre você, tipo login ou preferências, mas também são usados bastante pra rastrear seu comportamento entre sites diferentes
- Extensões de navegador que bloqueiam rastreadores e anúncios ajudam a reduzir a quantidade de dado coletado enquanto você navega
- Manter o navegador sempre atualizado, pelo mesmo motivo que vimos no tópico de vulnerabilidades de software

---

## Glossário

- **Autenticação de dois fatores (2FA)** - método de login que exige duas confirmações diferentes, geralmente a senha mais um código ou aprovação em outro dispositivo
- **OAuth (Autorização Aberta)** - sistema que permite usar uma conta existente (como Google ou Facebook) pra fazer login em outros serviços, sem criar uma senha nova
- **Engenharia social** - manipulação psicológica usada para enganar alguém e fazer essa pessoa entregar informação ou acesso que não deveria
- **Navegação anônima (ou privada)** - modo do navegador que não salva histórico nem cookies naquele dispositivo, mas não esconde a atividade de sites ou do provedor de internet
- **Cookies** - pequenos arquivos guardados pelo navegador que sites usam pra lembrar informações sobre o usuário, como login, preferências ou comportamento de navegação
- **Rastreador** - código ou ferramenta usada por sites e anunciantes para monitorar o comportamento de um usuário entre páginas ou sites diferentes
- **Phishing** - tipo de golpe de engenharia social feito por email ou mensagem, se passando por uma fonte confiável pra roubar dados
