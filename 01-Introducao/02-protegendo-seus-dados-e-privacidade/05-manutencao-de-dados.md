# Manutenção de Dados

> Diário de estudos - módulo "Protegendo seus Dados e Privacidade"

Depois de proteger a rede e os dispositivos, o próximo passo é cuidar dos dados em si, os arquivos, fotos, documentos e informações que ficam guardados nesses aparelhos. Esse tópico ensina como manter esses dados seguros, como fazer cópia deles e o que realmente acontece quando você "deleta" alguma coisa.

## O que é criptografia?

**Explicando do zero**
Imagina que você escreve uma carta, mas em vez de escrever com letras normais, você troca cada letra por um número seguindo um código que só você e a pessoa que vai receber conhecem. Se alguém roubar essa carta no caminho, vai ver só um monte de número sem sentido. Só quem tem o código consegue transformar aquilo de volta em texto legível.

Criptografia é exatamente isso, só que aplicada em dados digitais. É o processo de transformar uma informação legível (chamada de texto simples) em uma informação embaralhada e ilegível (chamada de texto cifrado), usando uma fórmula matemática e uma chave. Só quem tem a chave certa consegue desembaralhar e ler o conteúdo original de novo.

**Pra que serve isso na prática**
Mesmo que alguém consiga roubar um arquivo, invadir um HD ou interceptar uma mensagem, se aquele dado estiver criptografado, tudo que a pessoa vai ver é um monte de caractere sem nexo. A criptografia protege a informação mesmo quando ela cai em mãos erradas.

## Como você criptografa seus dados?

**Explicando do zero**
Criptografar dados não é algo só pra empresa grande ou especialista em tecnologia, dá pra aplicar isso no dia a dia com ferramentas relativamente simples.

**As formas mais comuns de fazer isso**

- **Criptografia de disco inteiro** - a maioria dos sistemas operacionais modernos já oferece essa opção nativa (como BitLocker no Windows ou FileVault no Mac). Ela criptografa tudo que tá guardado no dispositivo de uma vez só, então mesmo que alguém tire o disco do computador e tente ler direto, não consegue sem a senha
- **Criptografia de arquivo ou pasta específica** - em vez de criptografar o disco inteiro, dá pra proteger só um arquivo ou uma pasta puntual que contenha informação mais sensível
- **Criptografia de comunicação** - aplicativos de mensagem que usam criptografia de ponta a ponta (como o WhatsApp) garantem que só quem envia e quem recebe consegue ler a mensagem, nem o próprio aplicativo no meio do caminho tem acesso ao conteúdo
- **HTTPS em sites** - aquele cadeado que aparece do lado do endereço no navegador indica que a comunicação entre você e aquele site tá criptografada, protegendo dados como senha e número de cartão enquanto trafegam pela internet

## Faça backup de seus dados

**Explicando do zero**
Backup é simplesmente ter uma cópia extra dos seus dados guardada em outro lugar, separado do original. Pensa assim, se você só tem uma cópia de um documento importante e a única cópia se perde (o HD queima, o celular cai na água, um ransomware criptografa tudo), não sobra nada. Com uma cópia guardada em outro lugar, você sempre tem como recuperar.

**Onde guardar um backup**

- **HD externo ou pendrive** - cópia física, guardada fora do dispositivo principal
- **Nuvem** - serviços como Google Drive, iCloud ou Dropbox guardam a cópia em servidores remotos, acessíveis de qualquer lugar com internet
- **NAS (armazenamento em rede)** - um equipamento próprio, dedicado a guardar backups na sua própria rede

**Uma boa prática conhecida no mundo da segurança, a regra 3-2-1**
Ter pelo menos 3 cópias dos dados importantes, guardadas em 2 tipos diferentes de mídia (tipo HD externo e nuvem), sendo que pelo menos 1 dessas cópias fica fora do local físico principal (por exemplo, na nuvem, longe de casa). Isso protege até contra situação extrema, tipo um incêndio ou roubo que destrua todos os equipamentos que estão no mesmo lugar.

## Eles realmente desapareceram?

**Explicando do zero**
Aqui vem uma informação que costuma surpreender bastante gente, quando você deleta um arquivo e até esvazia a lixeira, ele não desaparece de verdade do disco na hora.

**O que realmente acontece por trás dos panos**
Quando um arquivo é "deletado" da forma comum, o sistema operacional só apaga a referência daquele arquivo no índice dele, tipo arrancar a etiqueta de uma caixa guardada num depósito gigante. O conteúdo da caixa (os dados em si) continua lá, jogado no meio do depósito, só que agora sem etiqueta nenhuma indicando onde ela tá nem o que tem dentro.

O espaço que aquele arquivo ocupava é marcado como "disponível" pra ser usado por um dado novo no futuro, mas até que algum arquivo novo seja realmente escrito por cima daquele espaço específico, o conteúdo antigo continua fisicamente ali, intacto. É por isso que existem ferramentas de recuperação de dados capazes de "trazer de volta" arquivos deletados, às vezes até depois de meses.

## Como você exclui os dados permanentemente?

**Explicando do zero**
Já que deletar do jeito comum não apaga os dados de verdade, existem métodos mais específicos pra garantir que uma informação sensível suma de vez, sem chance de recuperação.

**As formas de fazer isso**

- **Sobrescrita de dados (data wiping)** - um programa específico escreve por cima do espaço onde o arquivo estava, várias vezes, com dados aleatórios (tipo sequências de zeros e uns sem sentido). Isso garante que o conteúdo original fique impossível de recuperar, já que ele foi fisicamente substituído no disco
- **Destruição física** - pra quem quer ter certeza absoluta, principalmente em ambiente corporativo, existe a opção de destruir fisicamente o dispositivo de armazenamento, tipo triturar um HD ou pendrive até virar pedaço. Sem o disco existir mais, não tem como recuperar nada dele
- **Criptografia seguida de descarte da chave** - se o disco inteiro já tava criptografado desde o começo, uma alternativa é simplesmente jogar fora a chave de criptografia. Sem a chave, mesmo que alguém consiga ler os dados fisicamente do disco, tudo que vai aparecer é o conteúdo embaralhado e ilegível

---

## Glossário

- **Criptografia** - processo de transformar uma informação legível em uma informação embaralhada, usando uma chave, pra proteger o conteúdo de quem não deveria ter acesso
- **Texto simples** - a informação original, legível, antes de ser criptografada
- **Texto cifrado** - a informação já embaralhada, depois de passar pela criptografia
- **Chave de criptografia** - o código usado tanto pra embaralhar quanto pra desembaralhar os dados
- **Criptografia de ponta a ponta** - tipo de criptografia em que só o remetente e o destinatário conseguem ler o conteúdo, nem o serviço usado no meio do caminho tem acesso
- **HTTPS** - versão segura e criptografada do protocolo usado pra acessar sites na internet, indicada pelo símbolo de cadeado no navegador
- **Backup** - cópia extra de um dado, guardada separada do original, usada pra recuperação em caso de perda
- **Regra 3-2-1** - boa prática de backup, 3 cópias dos dados, em 2 tipos diferentes de mídia, sendo 1 delas fora do local físico principal
- **NAS** - equipamento de armazenamento conectado à rede local, usado como uma espécie de servidor próprio de backup
- **Sobrescrita de dados (data wiping)** - técnica de escrever dados aleatórios várias vezes por cima de um espaço de disco, pra tornar o conteúdo antigo impossível de recuperar
- **Recuperação de dados** - processo, feito com ferramentas específicas, de tentar resgatar arquivos que foram deletados mas ainda não foram sobrescritos no disco
