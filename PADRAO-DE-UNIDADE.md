# Como escrever uma unidade

Guia de produção de conteúdo do BFA, na ordem em que você escreve.

O protocolo abaixo foi fechado na prática, escrevendo a **Unidade 1 de
Matemática** (`docs/matematica-aplicada-a-financas/modulo-1-algebra-do-zero/aula-01-numeros-e-operacoes.md`).
Sempre que ficar em dúvida sobre como algo deve ficar, abre ela e olha —
ela é o modelo, não este arquivo.

Para calibrar: a Unidade 1 fechou em **390 linhas** de Markdown. Se a sua
estiver com 120, provavelmente falta a parte de exercícios. Se estiver com 800,
provavelmente virou duas unidades.

Este arquivo fica na raiz do repositório de propósito: o site publica só a pasta
`docs/`, então isto não aparece para o aluno.

---

## O princípio, em uma frase

**Ver → Fazer junto → Fazer sozinho → Aplicar.**

Cada etapa tira um pouco do apoio. A ideia é o aluno nunca travar, mas também
nunca ficar sem esforço. Quem só lê teoria não aprende; quem é jogado direto na
lista desiste.

Não é invenção nossa: vem do *worked example effect* (Sweller) e da *retrieval
practice* (Roediger e Karpicke).

---

# A ordem de escrita

## Fase 0 — antes de escrever uma linha

1. **Abra a unidade anterior e leia o último parágrafo dela.** Toda unidade
   termina com uma ponte para a próxima. Essa ponte é a promessa que você tem
   que cumprir.
2. **Escreva, para você mesmo, a única ideia que essa unidade ensina.** Uma
   frase. Se não couber em uma frase, a unidade está grande demais e vale
   dividir.
3. **Pense na situação de dinheiro que torna essa ideia inevitável.** Não é
   ilustração no fim — é o ponto de partida da fase seguinte.

## Fase 1 — o gancho

Primeira coisa da página, numa caixa `!!! tip "Comece aqui"`.

Uma pergunta concreta sobre dinheiro. **Nunca** "hoje vamos aprender funções
exponenciais".

Na Unidade 1 o gancho é o **"12x de R$ 89,90 sem juros"**: todo mundo já viu
essa frase, quase ninguém sabe o que ela significa. É esse o alvo — algo que o
aluno reconhece e não entende.

```markdown
!!! tip "Comece aqui"
    Você já viu "12x de R$ 89,90 sem juros" e ficou na dúvida se era
    barato ou caro. No fim desta unidade você responde isso em dez segundos.
```

## Fase 2 — a ideia em uma frase

Título `## A ideia em uma frase`. Dois ou três períodos, **zero símbolo
matemático**. É a intuição, para o aluno saber onde está entrando.

## Fase 3 — `## 1. Entender`

A parte mais importante, e onde quase todo material erra.

**Regra que não se negocia: o significado vem antes da tabela.** Nosso público
já viu a maioria dos assuntos na escola — o que falta não é a definição, é para
que serve. Se você começar pela tabela resumida, ele reconhece, acha que já sabe
e não aprende nada.

Um subtítulo `###` por conceito. Em cada um:

- **a pergunta que aquele conceito responde** (é isso que fica na cabeça);
- **um exemplo de dinheiro do dia a dia**, pequeno;
- quando o conceito tiver mais de um uso, separe os usos.

Na Unidade 1 isso ficou assim:

| Conceito | A pergunta dele | Usos separados |
|---|---|---|
| Soma | "Quanto dá no total?" | 1 |
| Subtração | "O que sobra? Qual a diferença?" | **2** — tirar e comparar |
| Multiplicação | "E se isso repetir?" | 1 |
| Divisão | "Quanto isso representa do total?" | **3** — repartir, medir, criar taxa |

Repare na divisão: são três usos, e o terceiro ("criar taxa") é o que abre
porcentagem, juros e rentabilidade nas unidades seguintes. Separar os usos é o
que faz o aluno reconhecer a operação depois, num problema que não avisa qual
operação usar.

**Depois** dos conceitos explicados, e só depois, vêm:

1. **um visual** — você escreve a especificação, o Guima produz (ver a seção
   "O que pedir para o Guima");
2. a tabela `### Conceitos essenciais`, com significado em linguagem simples;
3. uma tabela de "qual ferramenta usar" — na Unidade 1 ela se chama
   `### A pergunta que resolve metade dos problemas`, e liga situação a
   operação:

```markdown
| Se você quer saber… | A operação é |
|---|---|
| o total de várias coisas | soma |
| o que sobra depois de gastar | subtração |
| a diferença entre dois valores | subtração |
| o efeito de algo que se repete | multiplicação |
```

Essa tabela é a que o aluno consulta na hora da prova. Vale caprichar.

## Fase 4 — `## 2. Ver e fazer junto`

**Um exemplo resolvido, numerado passo a passo.** E o essencial: cada passo
**diz qual operação usou e por quê**, não só a conta.

Na Unidade 1 são 6 passos, e o formato de cada um é este:

```markdown
**Passo 1 — quanto ela ganha com o geladinho?** (multiplicação — preço × quantidade)
```

O que está entre parênteses é o que ensina. Sem isso, o aluno copia a conta e
não aprende a escolher a operação.

O exemplo tem uma pessoa com nome e uma situação inteira, que atravessa todos os
passos — na Unidade 1 é a **Ana**, mesada de R$ 200, vendendo geladinho a R$ 2,
juntando para uma meta de R$ 900. No fim, mexemos numa variável ("e se ela
cortar o lanche pela metade?") para o aluno ver o efeito.

Termine com **`### Agora você`**: dois exercícios com **o primeiro passo já
dado** e a resposta escondida num bloco recolhível.

```markdown
### Agora você

**(a)** O Pedro gasta R$ 12 por dia no transporte, 22 dias por mês.
Primeiro passo: isso se repete, então é multiplicação — `12 × 22`.
Quanto ele gasta no mês?

??? note "Ver resposta de (a)"
    `12 × 22 = 264`. Ele gasta **R$ 264** por mês só de transporte.
```

O primeiro passo dado é o degrau. É o que separa "fazer junto" de "fazer
sozinho".

## Fase 5 — `## 3. Praticar sozinho`

**6 a 8 problemas**, em dificuldade crescente, nesta ordem:

1. dois ou três de técnica pura (só a conta);
2. o miolo em contexto de dinheiro — **pelo menos 2 obrigatoriamente**;
3. um desafio no fim.

Depois de todos, **um único bloco recolhível** com o gabarito — e gabarito
significa **resolução explicada**, não resultado.

```markdown
??? note "Gabarito com resolução"
    **1.** `45 + 130 = 175`.

    **2.** Aqui é comparação, não "tirar": `180 − 145 = 35`, então o
    segundo mês foi R$ 35 mais caro.
```

Se o gabarito só tiver o número, o aluno que errou continua sem saber por quê —
e é exatamente ele que precisava do gabarito.

## Fase 6 — `## 4. Levar pra vida`

Três coisas, nesta ordem:

**1. `### Onde isso aparece no seu dinheiro`** — dois ou três lugares reais.
Fatura de cartão, boleto, extrato, anúncio de parcela.

**2. A colinha na página**, em caixa `!!! abstract "Resumo de bolso"`, com
fórmulas, a taxa-chave e os erros comuns. Ela fica **na página** — não depende
de baixar nada. Encerre com a nota padrão do PDF:

```markdown
!!! tip "Versão para imprimir"
    Uma versão em PDF desta colinha, feita em LaTeX, será disponibilizada
    para download em breve.
```

**3. `### Próxima unidade`** — a ponte. Uma pergunta que a unidade seguinte
responde. É o que a Fase 0 da próxima unidade vai ler.

## Fase 7 — revisão antes de dar por pronta

- [ ] O gancho é uma situação de dinheiro reconhecível, não um anúncio de tema
- [ ] Cada conceito tem o significado explicado **antes** de aparecer em tabela
- [ ] Conceitos com mais de um uso estão com os usos separados
- [ ] Tem a especificação escrita de pelo menos um visual
- [ ] Cada passo do exemplo resolvido diz qual operação usou e por quê
- [ ] O "Agora você" tem o primeiro passo dado
- [ ] Entre 6 e 8 problemas, com pelo menos 2 em contexto de dinheiro
- [ ] O gabarito explica a resolução
- [ ] A colinha está na página
- [ ] Tem ponte para a próxima unidade
- [ ] **Acentuação revisada** (ç, ã, acentos) — o público é estudante
      brasileiro e erro de grafia destrói credibilidade antes do conteúdo
- [ ] Diz "unidade", nunca "aula"

---

# O que pedir para o Guima

Estas três coisas **não são para você fazer**. São dele, e ele já combinou isso.
O que você precisa é saber **como pedir**, porque um pedido malfeito volta.

## 1. Gráficos e imagens

Você **não desenha nada**. Você escreve a **especificação** do visual, numa
caixa dentro da unidade, e o Guima produz a arte depois.

A especificação precisa de quatro coisas — a quarta é a que costuma faltar:

```markdown
!!! note "📊 Gráfico 1 — o mapa das quatro operações"
    **Formato:** quatro quadrados em grade 2×2, um por operação.

    **Conteúdo de cada quadrado:** o sinal grande (+ − × ÷), o nome da
    operação, a pergunta que ela responde, e um exemplo numérico curto.

    **Cores:** uma cor por operação, para o aluno reconhecer depois.

    **O que o aluno deve enxergar:** que cada operação existe para
    responder uma pergunta diferente — não são quatro contas, são quatro
    perguntas.
```

**O que o aluno deve enxergar** é o item mais importante. Sem ele, sai um
desenho bonito que não ensina. Com ele, o Guima sabe o que precisa ficar em
destaque e o que pode ser discreto.

Escreva a especificação **no lugar exato** onde o gráfico vai entrar no texto.
Assim ele sabe o contexto.

## 2. O PDF da colinha em LaTeX

A colinha você escreve — é conteúdo. O **PDF** é o Guima que faz, em LaTeX,
depois.

Sua parte: escrever a caixa `!!! abstract "Resumo de bolso"` completa e deixar a
nota padrão do "Versão para imprimir". Não precisa fazer nada além disso, e não
precisa aprender LaTeX.

## 3. Publicar e qualquer coisa de site

Deploy, endereço, cor, botão, layout: nada disso é seu. Se aparecer algo
estranho na tela — texto cortado, fórmula quebrada, tabela torta — **avise em
vez de tentar consertar**. Já aconteceu de um defeito de renderização parecer
erro de conteúdo.

## 4. Dúvida de recorte

Se você não souber se um assunto é desta unidade ou da próxima, pergunte antes
de escrever. É mais barato que reescrever.

---

# O que vale você aprender a fazer

Coisas pequenas que te deixam trabalhar sem depender de ninguém.

## 1. Os cinco blocos de Markdown que você vai usar

São só estes. Repare que a indentação de 4 espaços dentro das caixas é
obrigatória.

**Caixa de destaque** (gancho, avisos):

```markdown
!!! tip "Comece aqui"
    Texto da caixa, com quatro espaços de indentação.
```

Tipos disponíveis: `tip`, `note`, `warning`, `important`, `abstract`.

**Bloco recolhível** (respostas e gabaritos) — igual, mas com `???`:

```markdown
??? note "Ver resposta"
    A resposta fica escondida até o aluno clicar.
```

**Tabela:**

```markdown
| Coluna | Outra coluna |
|---|---|
| valor | valor |
```

**Negrito e código:** `**negrito**` e `` `12 × 22` `` para contas e números.

**Título:** `##` para as seções grandes, `###` para as de dentro.

## 2. Editar direto pelo site

Não precisa de terminal, nem instalar nada, nem token.

1. Abre a unidade em **brasil-financas-atlas.github.io/bfa**
2. Clica no **lápis ✏️** no topo da página
3. Abre o editor do GitHub naquele arquivo
4. Edita, e tem aba **Preview** para conferir antes
5. Rola até o fim, **Commit changes**, escreve uma frase do que mudou, confirma

Em cerca de um minuto está no ar. Só precisa de conta no GitHub e estar na
organização — o Guima te adiciona.

## 3. Ler o Preview antes de salvar

A aba *Preview* do editor do GitHub mostra quase igual ao site. Ela pega a
maioria dos erros de formatação — principalmente caixa sem indentação, que é o
erro mais comum e faz a caixa virar texto solto.

---

# Decisões já fechadas (não reabrir sem conversar)

- **Sem PBL em Matemática.** O caso de Problem Based Learning fica em Finanças.
  Matemática é procedimento: precisa de treino, então a lista de problemas é a
  prática principal. Finanças é julgamento: precisa de discussão, então leva
  caso, PBL e links do mundo real, com menos conta.
- **A colinha vive na página.** O PDF é complemento, nunca requisito.
- **Gráfico é especificação escrita**, produzido depois pelo Guima.
- **Diga "unidade", nunca "aula".** Os nomes de arquivo continuam
  `aula-NN-*.md` de propósito, para não quebrar a importação da plataforma.
  Não renomeie arquivo.

---

# Onde estamos

| Trilha | Estado |
|---|---|
| Matemática, Módulo 1 (Álgebra do Zero) | **Unidade 1 pronta no formato novo.** Unidades 2 a 7 são a prioridade |
| Matemática, Módulos 3 e 4 | 17 unidades escritas em **formato antigo** — têm PBL, e não têm gancho, "Agora você", visual nem colinha. Retrofit pendente, depois do Módulo 1 |
| Finanças, Módulos 1 a 3 | 26 unidades escritas. Estrutura própria de Finanças ainda a definir |
| Preparação BRHSIC | vazio |

**A prioridade combinada é terminar o Módulo 1 de Matemática primeiro**, no
formato novo, para existir um módulo inteiro coerente antes de mexer no resto.

Comece pela **Unidade 2 — Frações e decimais**. A ponte da Unidade 1 já promete
ela.
