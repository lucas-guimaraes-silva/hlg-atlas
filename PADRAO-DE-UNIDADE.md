# Padrão de unidade

Como escrever uma unidade do BFA. Este arquivo é para quem produz conteúdo
(Guima, Herton e quem entrar depois). Ele fica na raiz do repositório de
propósito: o MkDocs só publica a pasta `docs/`, então isto **não** vira
página do site.

Para mexer em cor, botão e layout, veja [DESIGN.md](DESIGN.md).

---

## O princípio: a escada do andaime

**Ver → Fazer junto → Fazer sozinho → Aplicar.**

Cada degrau tira um pouco do apoio. A ideia é que o aluno nunca trave, mas
também nunca fique sem esforço. Quem só lê teoria não aprende; quem é jogado
direto na lista desiste. A escada resolve os dois.

Isso não é invenção nossa: vem do *worked example effect* (Sweller) e da
*retrieval practice* (Roediger e Karpicke). O raciocínio completo e as
referências estão em `wiki/synthesis/design-didatico-bfa.md`, no cérebro do
Guima.

---

## Ordem fixa das seções — Matemática

A ordem é fixa. O aluno aprende o formato uma vez e depois sabe onde
procurar cada coisa em qualquer unidade.

**Gancho** — caixa `!!! tip "Comece aqui"`. Uma pergunta concreta sobre
dinheiro. Nunca "hoje veremos funções exponenciais". O gancho da Unidade 1 é
o "12x de R$ 89,90 sem juros": todo mundo já viu, quase ninguém sabe o que
significa.

**A ideia em uma frase** — a intuição, sem nenhum símbolo.

### 1. Entender

- O **significado** de cada conceito **antes** da tabela resumida. Esse é o
  erro mais comum: começar pela tabela. O público-alvo já viu a maioria dos
  assuntos na escola — o que falta é entender para que servem.
- Depois, a tabela "Conceitos essenciais".
- Um guia de "qual operação/ferramenta usar" para cada situação.
- Pelo menos **um visual**, com legenda dizendo o que o aluno deve observar.

### 2. Ver e fazer junto

- Exemplo resolvido passo a passo, **comentando o raciocínio**, não só a
  conta. O aluno precisa ver por que aquele passo foi escolhido.
- **"Agora você"**: dois exercícios com o primeiro passo já dado e a
  resposta em `??? note` recolhível.

### 3. Praticar sozinho

- 6 a 8 problemas em dificuldade crescente: técnica → contexto de dinheiro →
  um desafio.
- Pelo menos 2 contextualizados em dinheiro.
- Gabarito recolhível **com resolução explicada**, não só o resultado.

### 4. Levar pra vida

- "Onde isso aparece no seu dinheiro".
- A **colinha** na própria página, em caixa `!!! abstract "Resumo de
  bolso"`: fórmulas, taxa-chave e erros comuns.
- Ponte para a próxima unidade.

---

## Decisões já tomadas (não reabrir sem conversar)

**Sem PBL em Matemática.** O caso de Problem Based Learning fica em
Finanças. Matemática é procedimento: precisa de treino, então a lista de
problemas é a prática principal. Finanças é julgamento: precisa de
discussão, então leva caso, PBL e links do mundo real, com menos conta.

**A colinha vive na página.** No futuro terá também um PDF em LaTeX para
baixar, mas o conteúdo não pode depender do download.

**Gráficos são responsabilidade do Guima**, não do time de front-end. Cada
unidade traz a **especificação escrita** do visual em caixa
`!!! note "📊 Gráfico N"`: formato, conteúdo e o que o aluno deve enxergar.
A arte é produzida depois, a partir dessa especificação.

---

## Terminologia

Diga **unidade**, nunca "aula". A troca já foi feita em todo o conteúdo
visível (383 ocorrências).

Os **nomes de arquivo** continuam `aula-NN-*.md` de propósito, para não
quebrar a importação que o David já fez na plataforma. Serão renomeados
depois, junto com ele. Não renomeie por conta própria.

---

## Checklist antes de dar a unidade por pronta

- [ ] Gancho é uma situação de dinheiro reconhecível, não um anúncio de tema
- [ ] Cada conceito tem o significado explicado antes de aparecer em tabela
- [ ] Tem pelo menos um visual (ou a especificação escrita dele)
- [ ] O exemplo resolvido comenta o raciocínio, não só a conta
- [ ] "Agora você" tem o primeiro passo dado
- [ ] Entre 6 e 8 problemas, com gabarito explicado
- [ ] Colinha na página
- [ ] Ponte para a próxima unidade
- [ ] Acentuação revisada (ç, ã, acentos) — o site é para estudante
      brasileiro e erro de grafia destrói credibilidade
- [ ] Aberto no navegador com `python -m mkdocs serve` antes do commit

---

## Pendência conhecida

As 17 unidades já escritas dos Módulos 3 e 4 de Matemática seguem um formato
antigo: têm seção de PBL e **não** têm gancho, "Agora você", visual nem
colinha. O retrofit está pendente. A prioridade combinada é terminar o
Módulo 1 primeiro.
