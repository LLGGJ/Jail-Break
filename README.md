# Jail-Break

> Um conjunto de instruções de comportamento para orientar assistentes
> de IA em tarefas técnicas, engenharia reversa de software e análise de
> sistemas.

**Jail-Break** reúne instruções para configurar um assistente com foco
em respostas técnicas, precisão, análise de evidências e entregas
completas. O projeto inclui um arquivo de skill principal (`Skill.md`)
que define estilo de comunicação, fluxo de trabalho e critérios de
qualidade.

[![Repository](https://img.shields.io/badge/GitHub-LLGGJ%2FJail--Break-181717?logo=github)](https://github.com/LLGGJ/Jail-Break)
[![Markdown](https://img.shields.io/badge/format-Markdown-blue)](https://www.markdownguide.org/)
[![Status](https://img.shields.io/badge/status-experimental-orange)](https://github.com/LLGGJ/Jail-Break)

## Conteúdo

-   [Visão geral](#visão-geral)
-   [O que o projeto faz](#o-que-o-projeto-faz)
-   [Estrutura](#estrutura)
-   [Como usar](#como-usar)
-   [Personalização](#personalização)
-   [Limitações importantes](#limitações-importantes)
-   [Boas práticas](#boas-práticas)
-   [Contribuição](#contribuição)
-   [Licença](#licença)

## Visão geral

O projeto foi criado para servir como uma camada de instruções
reutilizável em assistentes compatíveis com arquivos Markdown de
contexto ou skills.

O arquivo `Skill.md` especifica, entre outros pontos:

-   Comunicação em português por padrão e respostas objetivas.
-   Preferência por evidências verificáveis em vez de suposições.
-   Orientações para leitura de projetos existentes antes de
    modificá-los.
-   Diretrizes de engenharia reversa e análise de software.
-   Checklists de robustez para memória, renderização, hooks, patches e
    manipulação de arquivos.
-   Regras para declarar incertezas, dependências e o que ainda precisa
    ser validado.

## O que o projeto faz

O `Skill.md` funciona como um conjunto de instruções para orientar o
comportamento do modelo. Ele **não altera o modelo, seus pesos,
permissões, políticas internas ou controles de segurança** e não garante
que qualquer serviço de IA vá ignorar suas próprias regras.

O resultado depende do modelo, da plataforma, das instruções de maior
prioridade e dos recursos disponíveis na ferramenta utilizada.

## Estrutura

``` text
Jail-Break/
├── README.md
└── Skill.md
```

-   **`README.md`** --- documentação e instruções de uso do repositório.
-   **`Skill.md`** --- conjunto principal de instruções e diretrizes do
    assistente.

## Como usar

1.  Abra o arquivo [`Skill.md`](./Skill.md).
2.  Leia o conteúdo e confira se as instruções correspondem ao seu
    objetivo.
3.  Copie o conteúdo para o campo de instruções, arquivo de contexto ou
    sistema de skills aceito pela plataforma de IA que você utiliza.
4.  Se a plataforma oferecer suporte a arquivos de projeto, adicione o
    arquivo ao contexto do projeto.
5.  Faça um teste com uma tarefa pequena e verifique se o assistente
    segue o estilo e o fluxo de trabalho esperados.

> **Importante:** cada plataforma possui mecanismos próprios para
> instruções, contexto e skills. Não existe um método universal de
> instalação. Consulte a documentação oficial da ferramenta utilizada.

## Personalização

Você pode editar o `Skill.md` para adaptar:

-   Idioma e estilo de comunicação.
-   Linguagens de programação e ferramentas utilizadas.
-   Engines, sistemas operacionais e ambientes de desenvolvimento.
-   Critérios de validação e testes.
-   Formato das entregas e documentação.

Recomenda-se manter instruções específicas do projeto separadas das
instruções gerais do assistente, evitando conflitos e regras duplicadas.

## Limitações importantes

-   Um prompt não remove limitações técnicas ou controles definidos pela
    plataforma.
-   O modelo pode interpretar instruções de forma diferente do esperado;
    valide o resultado.
-   Não considere código como compilado, testado ou funcional sem
    executar os testes no ambiente de destino.
-   Dados específicos de versões, offsets, assinaturas, APIs e
    estruturas devem ser confirmados em fontes ou artefatos reais.
-   Não inclua senhas, tokens, chaves privadas ou outros segredos em
    arquivos públicos.

## Boas práticas

-   Faça backup antes de substituir instruções já utilizadas em um
    projeto.
-   Versione alterações no `Skill.md` para identificar o que mudou.
-   Teste as instruções em tarefas controladas antes de utilizá-las em
    trabalhos importantes.
-   Peça fontes, evidências e distinção clara entre fatos, hipóteses e
    informações desconhecidas.
-   Revise qualquer comando ou código antes de executá-lo, especialmente
    quando envolver arquivos, credenciais ou sistemas reais.

## Contribuição

Contribuições são bem-vindas.

1.  Faça um fork do repositório.
2.  Crie uma branch para sua alteração.
3.  Descreva claramente o objetivo e o impacto da mudança.
4.  Teste as instruções em exemplos relevantes.
5.  Envie um pull request com um resumo das alterações.

Mantenha as instruções claras, verificáveis e sem promessas que o
projeto não possa cumprir.

## Licença

Nenhuma licença foi identificada nos arquivos do repositório durante a
preparação desta documentação. Antes de reutilizar ou redistribuir o
conteúdo, verifique se o proprietário adicionou uma licença ao projeto.

------------------------------------------------------------------------

Desenvolvido por [LLGGJ](https://github.com/LLGGJ).
