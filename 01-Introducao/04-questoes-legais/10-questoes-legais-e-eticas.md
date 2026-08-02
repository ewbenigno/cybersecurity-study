# Questões Legais e Éticas

> Diário de estudos - módulo "O seu futuro estará na segurança cibernética?"

Começa aqui o último módulo do curso. Antes de falar sobre carreira, esse tópico trata de um lado que muita gente esquece quando pensa em segurança cibernética, os limites legais e éticos de tudo que foi estudado até agora. Saber invadir um sistema é uma coisa, ter permissão pra fazer isso é outra completamente diferente.

## Questões jurídicas em segurança cibernética

**Explicando do zero**
Praticamente tudo que foi visto no curso até aqui, desde varredura de porta até exploração de vulnerabilidade, pode ser crime dependendo de um único detalhe, se você tinha autorização pra fazer aquilo ou não. A mesma ação técnica pode ser um trabalho de pentest legítimo e bem pago, ou um crime sério, dependendo só desse detalhe.

**Por que isso importa tanto**
Diferente de outras áreas da tecnologia, em segurança cibernética o profissional lida o tempo todo com ferramentas e técnicas que também são usadas por criminosos. A lei, em geral, não olha pra ferramenta usada, olha pra autorização. Testar a segurança de um sistema que não é seu, sem permissão explícita por escrito do dono, é crime na maioria dos países, mesmo que a intenção fosse só "dar um alerta" ou "ajudar".

**O que costuma caracterizar a legalidade de uma ação**

- Ter autorização por escrito antes de testar qualquer sistema que não seja seu
- Respeitar exatamente o escopo definido nessa autorização, ou seja, só testar o que foi combinado, nada além disso
- Reportar vulnerabilidades encontradas pelo canal correto, em vez de explorar ou divulgar publicamente sem aviso prévio
- Estar ciente de que leis variam de país pra país, o que é permitido num lugar pode ser crime em outro

## Questões éticas em segurança cibernética

**Explicando do zero**
Além da lei, existe uma camada de ética que vai além do que é ou não permitido no papel. Ética aqui é sobre fazer a escolha certa mesmo quando ninguém estaria olhando, ou mesmo quando tecnicamente algo não seria ilegal, mas ainda assim seria errado fazer.

**Dilemas éticos comuns na área**

- Encontrar uma vulnerabilidade grave num sistema, mas a empresa dona demora muito ou se recusa a corrigir, o profissional deve divulgar publicamente pra forçar a correção, mesmo sabendo que isso expõe usuários até a correção sair?
- Ter acesso a dados sensíveis durante um teste autorizado, mas usar aquele acesso só pro que foi combinado, resistindo à curiosidade de "dar uma olhada" em informação que não tem relação com o trabalho
- Descobrir por acaso uma falha grave num sistema que você nunca foi autorizado a testar, o que fazer com essa informação

**O princípio central**
A maioria dos códigos de ética da área se resume a uma ideia, usar o conhecimento técnico pra proteger, não pra causar dano, e sempre respeitar a privacidade e os direitos das pessoas envolvidas, mesmo quando teria como fazer diferente sem ser pego.

## Questões de ética corporativas

**Explicando do zero**
Enquanto o tópico anterior falou de ética num nível mais individual, esse aqui trata de como as próprias empresas lidam com questões éticas relacionadas a segurança e dado dos seus usuários.

**Pontos comuns nesse tema**

- **Transparência com vazamento de dados** - quando uma empresa sofre um incidente de segurança, existe uma responsabilidade ética (e muitas vezes legal, como já vimos com a LGPD) de avisar os usuários afetados, em vez de esconder o problema pra evitar dano à imagem
- **Uso responsável de dado coletado** - só porque uma empresa tecnicamente pode coletar um tipo de dado, não significa que deveria, principalmente se aquele dado vai além do necessário pro serviço funcionar
- **Segurança como prioridade real, não só discurso** - existe uma diferença entre uma empresa que investe de verdade em segurança e uma que só usa o termo em campanha de marketing, sem aplicar prática nenhuma por trás
- **Tratamento justo de quem reporta vulnerabilidade** - empresas que recebem um aviso de vulnerabilidade de um pesquisador de segurança de boa fé têm a responsabilidade ética de tratar aquilo com seriedade, em vez de ameaçar processo contra quem só quis ajudar

---

## Glossário

- **Pentest (teste de penetração)** - simulação autorizada de um ataque real, feita por um profissional contratado, pra encontrar vulnerabilidades antes de um invasor real
- **Escopo** - limite exato do que foi autorizado a ser testado durante um trabalho de segurança, definido previamente entre o profissional e o contratante
- **Divulgação de vulnerabilidade** - processo de reportar uma falha de segurança encontrada, seja de forma privada direto pra empresa responsável, seja publicamente após um prazo combinado
- **Ética profissional** - conjunto de princípios que guiam a conduta correta de um profissional, mesmo além do que é exigido por lei
- **LGPD** - Lei Geral de Proteção de Dados, legislação brasileira que regula como empresas devem coletar, usar e proteger dados pessoais
- **Pesquisador de segurança de boa fé** - pessoa que encontra e reporta vulnerabilidades com a intenção de ajudar a corrigir o problema, não de causar dano ou obter vantagem indevida
