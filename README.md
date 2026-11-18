# AURELIO Prompt Builder

Plugin que avalia, melhora e constrói prompts para qualquer modelo de linguagem usando o **framework AURELIO**, método criado pelo Prof. Aurélio L. S. Murta (Universidade Federal Fluminense).

*English summary: a prompt engineering plugin that scores, rewrites and builds prompts using the seven-dimension AURELIO framework. Instructions are written in Brazilian Portuguese; the skill answers in the user's language.*

## O framework

| Letra | Dimensão | Pergunta que responde |
|---|---|---|
| A | Alvo | Que papel o modelo assume e para quem é a resposta? |
| U | Utilidade | Para que serve a resposta e em que contexto será usada? |
| R | Regras | Quais critérios e restrições devem ser seguidos? |
| E | Estrutura | Em que formato a resposta deve vir? |
| L | Linguagem | Qual o idioma, o tom e o nível de detalhe? |
| I | Iteração | Como o prompt será refinado até ficar adequado? |
| O | Objetividade | O comando está claro e sem ambiguidades? |

## O que o plugin faz

- **Você envia um prompt pronto:** recebe uma nota de 0 a 10 para cada letra, a nota geral e, se a média for inferior a 8,5 ou alguma letra ficar abaixo de 7, uma versão reescrita.
- **Você envia ideias soltas:** recebe um prompt construído do zero, com no máximo três perguntas de esclarecimento quando faltar informação essencial.

A resposta vem sempre em duas partes: a análise e o prompt final, em bloco de código, pronto para copiar e colar. Dados que você não informou aparecem como `[CAMPOS ENTRE COLCHETES]`, nunca inventados.

## Como instalar no Claude

**No Claude (web ou desktop):** abra Customize > Plugins > Add > Add marketplace e informe `aureliomurta75/aurelio-prompt-builder`. O plugin aparece na lista para ser adicionado.

**No Claude Code:**

```
/plugin install aurelio-prompt-builder --marketplace aureliomurta75/aurelio-prompt-builder
```

## Como usar no Gemini

Abra este link com a sua conta Google e adicione a habilidade:

https://gemini.google.com/customize/skills/d/1RwDzpjpqEGkpwrspJBooDwW-2VVlIp0V?usp=sharing

Alternativa: baixe o arquivo [`SKILL.md`](skills/4ur3l10-prompt-builder/SKILL.md) e, em gemini.google.com, vá em Personalizar > Habilidades > Criar > Enviar.

## Como usar no ChatGPT e em outras IAs

- **ChatGPT com o recurso Skills:** baixe o arquivo [`SKILL.md`](skills/4ur3l10-prompt-builder/SKILL.md) e envie em Plugins > Skills > Create > Upload from your computer. O recurso depende do plano da conta.
- **Qualquer IA, inclusive planos gratuitos:** abra o arquivo [`SKILL.md`](skills/4ur3l10-prompt-builder/SKILL.md), copie todo o conteúdo e cole no início da conversa. Em seguida, envie o prompt que deseja avaliar ou as ideias para construir um novo.

## Como usar

Depois de instalar, basta pedir em linguagem natural:

- "Avalie este prompt: ..."
- "Melhore este prompt com o AURELIO: ..."
- "Crie um prompt para ..."

Ou chame a skill diretamente pelo menu de barra: `/aurelio-prompt-builder:4ur3l10-prompt-builder`.

## Conteúdo

O plugin contém uma única skill, `4ur3l10-prompt-builder`, composta apenas por instruções em texto.

## Privacidade e segurança

O plugin não executa código, não instala pacotes, não usa conectores, não acessa a rede, não lê arquivos e não envia dados a nenhum serviço externo.

## Autor

Prof. Aurélio L. S. Murta, Professor Titular do Departamento de Administração da Universidade Federal Fluminense (UFF).
Currículo Lattes: http://lattes.cnpq.br/7344029160665638

## Licença

MIT. Uso, cópia e adaptação são livres, desde que mantido o aviso de autoria.
