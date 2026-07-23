# Estudos de Cibersegurança

Repositório criado pra documentar, de forma pública, todo o meu processo de aprendizado em Cibersegurança.

A ideia é registrar cada tópico estudado em um documento próprio, com explicações em linguagem simples, exemplos práticos e um resumo do que foi aprendido. Serve tanto como material de consulta futura quanto como portfólio do progresso.

---

## Trilha de estudos

Os estudos seguem o curso de Cibersegurança da Cisco NetAcad, avançando módulo por módulo conforme o curso libera o conteúdo.

```
flowchart LR
    subgraph M1["Módulo 1 — Panorama da Cibersegurança"]
        D01["..."]
    end
    subgraph M2["Módulo 2 — Ataques, Conceitos e Técnicas"]
        D02["..."]
    end
    subgraph M3["Módulo 3 — Proteção de dados e privacidade"]
        D03["..."]
    end
    subgraph M4["Módulo 4 — Proteção da organização"]
        D04["..."]
    end
    subgraph M5["Módulo 5 — O seu futuro estará na segurança cibernética?"]
        D05["..."]
    end

    D01 --> D02 --> D03 --> D04 --> D05

    click D02 "./2.2-metodos-de-infiltracao.md" "Abrir documento"
```

    Loading
> O grafo acima cresce conforme os estudos avançam. Cada nó é um documento novo, e as setas indicam a ordem de progressão.
---

## Índice de documentos

| #  | Tópico                                                                                          | Módulo                          | Status         |
| --- | ------------------------------------------------------------------------------------------------ | -------------------------------- | -------------- |
| 01 | [2.2 Métodos de infiltração](/Introducao/metodos-de-infiltracao.md) | Ataques, Conceitos e Técnicas | ✅ Concluído |

---

## Estrutura do repositório

```
.
├── README.md
├── 2.2-metodos-de-infiltracao.md
└── ...
```

Cada arquivo segue o padrão de nome `X.X-titulo-do-topico.md`, contendo:

- Explicação didática do conteúdo
- Exemplos práticos
- Status do tópico no curso

---

## Objetivo final

Consolidar o aprendizado em uma base sólida de Cibersegurança, com foco em segurança de aplicações web, aproveitando a experiência prévia como desenvolvedor front-end pra unir os dois mundos.

---

## Sobre

Estudos conduzidos e documentados por @ewerson_dev, freelance fullstack developer e criador de conteúdo educativo sobre desenvolvimento web.