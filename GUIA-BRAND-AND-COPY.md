# Guia: Marca e Copy antes de codar

> Este guia é lido dentro do Claude Code — ou em qualquer leitor Markdown.
> Cada módulo leva entre 20 e 60 minutos. Você pode parar e continuar de onde parou.

---

## Por que este guia existe

A maioria das pessoas trata marca e copy como a última etapa. Algo para "deixar bonito" depois que o produto funciona.

Isso é de trás pra frente.

As palavras que você usa, as cores que escolhe e o tom que fala não são enfeite — são parte do produto. São a primeira coisa que alguém julga, no meio segundo antes de ler qualquer frase, e o que decide se a pessoa entende o que você fez, sente que é pra ela, e fica.

Este guia cobre a camada entre "eu sei o que estou construindo" e "estou pronto pra escrever código". É o que faz o seu produto *parecer alguma coisa*, não só *fazer alguma coisa*.

Vem depois do [product-discovery](https://github.com/ohanatais/product-discovery) (você já sabe pra quem é e o que te diferencia) e antes do [build-with-claude](https://github.com/ohanatais/build-with-claude) (a hora de construir).

---

## O que você vai aprender

Três módulos. A ordem importa: eles se constroem um sobre o outro.

| Módulo | Pergunta central | Skill |
|---|---|---|
| [1. Identidade de marca](#módulo-1-identidade-de-marca) | Quem é este produto, e como ele se parece? | `/brand-identity` |
| [2. Tom de voz](#módulo-2-tom-de-voz) | Como este produto fala — e como soa sempre como ele mesmo? | `/tone-of-voice` |
| [3. Copy de produto](#módulo-3-copy-de-produto) | Que palavras fazem a pessoa certa sentir que isso foi feito pra ela? | `/product-copy` |

A identidade define o recipiente visual. O tom de voz define a personalidade verbal. A copy é onde os dois ganham vida nos momentos que importam. Construa nessa ordem: copy escrita sem um tom definido soa como todo mundo, e um tom definido sem identidade não tem onde se ancorar.

Você não precisa usar as skills para seguir o guia. Mas elas fazem o trabalho junto com você — dentro do Claude Code, no idioma que você falar, e derivando tudo da *sua* realidade, não de um estilo pronto.

---

## Como usar este guia

**Se você está começando do zero:** siga os módulos em ordem. Cada um tem uma leitura (~10 min) e uma prática (~20–40 min com a skill).

**Se você já está no meio:** pule pro módulo onde está. Mas se a copy parece genérica downstream, a causa quase sempre está numa etapa que você pulou upstream — geralmente uma identidade ou um tom mal definidos.

**Se você quer só as skills:** cada módulo tem instruções de instalação e uso. Você não precisa ler o guia inteiro.

Uma coisa antes de começar: estas skills são **universais por design**. Os frameworks são fixos, mas o resultado não. A mesma skill produz uma marca calorosa e manuscrita pra um produto e uma marca dura e técnica pra outro — porque cada uma deriva da *sua* personalidade, categoria e cultura. Nada aqui te empurra pra um estilo "certo".

---

## Módulo 1: Identidade de marca

### O que é e por que importa

Identidade de marca não é decoração que você adiciona no fim. É a primeira decisão que o seu usuário toma sobre confiar em você — tomada antes de ler uma palavra.

Você não precisa de agência nem de designer. Precisa de clareza sobre o que o produto representa, e de um sistema visual consistente que comunique isso quando você não está na sala pra explicar.

A regra que governa tudo: **derive, nunca recorra ao default.** Toda escolha visual tem que vir de algo que a marca representa. No momento em que a justificativa vira "isso fica bonito" ou "é o que os produtos modernos fazem", a escolha falhou.

### Os cinco componentes, sempre em ordem

A identidade se constrói numa sequência fixa, onde cada peça depende da anterior:

```
1. Personalidade   →  Quem é a marca, como se fosse uma pessoa? (arquétipo + traços + o "único")
2. Cor             →  Uma paleta que expressa essa personalidade de propósito, não por gosto
3. Tipografia      →  A tipografia como voz da marca, antes de qualquer palavra ser lida
4. Logo            →  A marca mais simples que sobrevive a 16px e em uma cor só
5. Documentação    →  O doc de marca + tokens que tornam tudo reproduzível sem você
```

Por que a ordem é inegociável: cor só é "certa" em relação a uma personalidade. Roxo não é premium nem brincalhão no abstrato — depende do que a marca tenta ser. Um logo sem nada acima dele é só uma forma que você por acaso gostou.

### Personalidade: arquétipo + adjetivos que restringem

Duas lentes com base em pesquisa, usadas juntas:

- **Arquétipo** (os 12 de Mark & Pearson, a partir de Jung) — o impulso humano dominante que a marca toca. Escolha **um** primário.
- **Três adjetivos** ancorados nas cinco dimensões de personalidade de marca da Jennifer Aaker (Sinceridade, Entusiasmo, Competência, Sofisticação, Robustez). O teste: cada adjetivo precisa **excluir** alguma coisa. "Moderno, limpo, confiável" descreve qualquer produto e não restringe nada. "Espirituoso, caloroso, um pouco irreverente" elimina o frio e o corporativo — agora cor e tipografia têm um trabalho.

E a **linha de unicidade** (Neumeier): "o único [categoria] que [benefício]." Se você não consegue escrever com a palavra "único", a marca não tem uma borda pra dramatizar.

### Cor: real, mas não universal

Cor carrega personalidade, mas o significado dela é contextual, não fixo. A pesquisa (Labrecque & Milne) mostra que tons mapeiam pra traços de personalidade *em média* — mas o efeito é moderado por contexto, categoria e cultura. Vermelho é sorte na China e perigo em outro lugar. Não existe dicionário universal de cores; desconfie de qualquer fonte que te entregar um.

### O que fazer agora

```bash
# Copiar para o seu projeto
cp -r path/to/brand-and-copy/brand-identity .claude/skills/

# No Claude Code:
/brand-identity
```

A skill tem três modos: **guided** (do zero, explicando cada componente), **brief** (já tem posicionamento, quer o brief + tokens direto), e **audit** (já tem uma identidade, quer uma crítica honesta de coerência, clichês e acessibilidade).

**O que você vai ter no final:** uma declaração de personalidade (arquétipo + três adjetivos + a linha de unicidade), um sistema de cor nomeado por papel, um sistema tipográfico com a sua assinatura, uma direção de logo, e um doc de marca + tokens — o entregável que torna a marca reproduzível sem você.

---

## Módulo 2: Tom de voz

### O que é e por que importa

Tom de voz não é sobre ser engraçado ou formal. É sobre ser **consistente** — e, por isso, reconhecível.

Um produto que soa espirituoso na landing page, robótico no onboarding e pedindo desculpas nas mensagens de erro parece inacabado, mesmo com o código impecável. O que as pessoas sentem é a consistência: se a página, o onboarding, os botões e os erros soam como uma mesma pessoa. Inconsistência lê como desleixo. Uma voz consistente — mesmo simples — lê como um produto que se entende.

### Voz vs. tom: a distinção que sustenta tudo

- **Voz é constante.** É a personalidade do produto em palavras. Não muda entre uma comemoração e um erro. Voz responde: *quem está falando?*
- **Tom é variável.** É como a voz se ajusta ao momento — comemorativo numa vitória, calmo e direto num erro. Tom responde: *o que este momento precisa?*

Uma pessoa tem uma voz e muitos tons: você continua você num velório e numa festa, mas não fala igual. Um produto é a mesma coisa. Defina a voz uma vez; mapeie os tons aos contextos.

### As quatro dimensões (NN/g)

A pesquisa do Nielsen Norman Group dá ao tom algo que "seja amigável" não tem: como medir. Qualquer texto se posiciona em quatro escalas:

1. **Engraçado ↔ Sério**
2. **Formal ↔ Casual**
3. **Respeitoso ↔ Irreverente**
4. **Entusiasmado ↔ Direto ao ponto**

Isso torna a voz repetível ("casual, sério, respeitoso, direto" é um ajuste que outra pessoa consegue acertar) e tem efeito medido na percepção de amigabilidade, confiança e desejabilidade.

### "Diga de três jeitos"

A forma mais confiável de tornar uma voz *ensinável*. Para uma mensagem real do produto, escreva três versões: **na voz** (exatamente certa), **fora da voz** (uma versão plausível que quebra — dura demais, brincalhona demais, genérica demais), e **no limite** (quase certa, mas sutilmente errada). O contraste é o que deixa a voz legível pra qualquer outra pessoa, incluindo o Claude.

### O que fazer agora

```bash
cp -r path/to/brand-and-copy/tone-of-voice .claude/skills/

# No Claude Code:
/tone-of-voice
```

A skill tem três modos: **guided** (define voz e tom do zero), **chart** (já tem a personalidade, quer o guia de voz formal produzido), e **audit** (tem copy, quer checar se soa como um produto só).

Uma coisa que a skill carrega: o **léxico e a lista de proibidos são sempre seus**. Não existe lista universal de "palavras ruins" — só palavras que quebram *esta* voz. Um produto proíbe ponto de exclamação; outro vive deles.

**O que você vai ter no final:** uma definição de voz (três adjetivos + posição nas quatro dimensões), um mapa de tom por contexto, um léxico (palavras que usa e que quebram a voz), padrões de microcopy (erro, estado vazio, onboarding), exemplos de "diga de três jeitos", e um doc de voz — com um guardrail opcional pra manter consistência quando muitas mãos (ou IA) escrevem.

---

## Módulo 3: Copy de produto

### O que é e por que importa

Copy não é sobre soar inteligente. É sobre fazer a pessoa certa, no momento certo, sentir que este produto foi feito pra ela.

Copy genérica é invisível — o olho escorrega. Copy específica converte, porque soa como quem sabe algo verdadeiro sobre *aquela* pessoa. A diferença quase nunca é talento; é método: saber quem está lendo, quanto já sabe, o que realmente quer, e dizer nas palavras que ela reconhece.

### Os cinco estágios de consciência (Schwartz)

A lente mais útil da copywriting, do *Breakthrough Advertising* (Eugene Schwartz, 1966). Antes de escrever uma palavra, posicione o leitor:

1. **Inconsciente** — nem sabe que tem o problema. O trabalho: nomear o problema.
2. **Consciente do problema** — sente o problema, não sabe que há solução. O trabalho: mostrar que você entende o problema com precisão.
3. **Consciente da solução** — sabe que soluções existem, está comparando. O trabalho: a sua diferenciação (o "único" do posicionamento).
4. **Consciente do produto** — conhece o seu produto, ainda não se convenceu. O trabalho: prova, especificidade, objeções respondidas.
5. **Mais consciente** — pronto, precisa de um empurrão. O trabalho: uma oferta clara e um próximo passo fácil.

A regra que evita a maioria dos erros: combine a copy com onde o leitor *realmente está* — quase sempre um ou dois estágios antes do que o fundador assume. O fundador é "mais consciente" sobre o próprio produto; o visitante raramente é.

### A escada do "e daí?"

Uma feature é o que o produto tem. Um benefício é o que ele faz. *Significado* é o que isso muda na vida do leitor — e significado é o que converte. Desça cada afirmação importante perguntando "e daí?" até bater em algo que a pessoa realmente sente:

- Feature: "exporta pra PDF"
- E daí? → "compartilha seu trabalho sem mandar o arquivo"
- E daí? → "você parece profissional pro cliente em dois cliques, sem instalar nada"

Pergunte "e daí?" pelo menos duas vezes em cada benefício.

### Minere, não invente

A melhor copy é montada, não autorada. As palavras que convertem geralmente já existem — em reviews, tickets de suporte, conversas de venda, threads de fórum. "Message mining" é colher as frases que pessoas reais usam pra descrever o problema e o alívio, e colocar essas frases na copy. Quando você tem qualquer linguagem real de cliente, use antes de inventar.

### O que fazer agora

```bash
cp -r path/to/brand-and-copy/product-copy .claude/skills/

# No Claude Code:
/product-copy
```

A skill tem três modos: **guided** (escreve um ativo do zero, explicando os movimentos), **asset** (sabe a mensagem e a voz, quer a copy produzida), e **audit** (tem copy que não converte, quer um diagnóstico).

Ela **herda** o que você já fez: o posicionamento (a mensagem) e a voz (o `/tone-of-voice`). Copy é a última camada — mais forte quando se apoia nas anteriores.

**O que você vai ter no final:** a chamada de leitor + estágio de consciência, a proposta de valor numa frase, a copy escrita na voz do produto com cada parte rotulada, o raciocínio por trás das linhas-chave, as objeções respondidas, um teste de clareza (o teste dos 5 segundos), e 2–3 variações de headline/CTA pra testar.

---

## Próximos passos

Com identidade, voz e copy definidas, o produto tem cara, fala como ele mesmo, e diz a coisa certa pra pessoa certa.

O que vem depois deste repositório:

- **[build-with-claude](https://github.com/ohanatais/build-with-claude)** — Claude Code para não-técnicos: cada decisão técnica explicada e setup de ferramentas passo a passo
- **[go-to-market](https://github.com/ohanatais/go-to-market)** — estratégia de lançamento, canais, primeiros usuários

E, se você ainda não passou por ele:

- **[product-discovery](https://github.com/ohanatais/product-discovery)** — pesquisa de mercado, validação, personas, posicionamento, PRD (a camada que vem antes desta)

---

*Feito por [Ohana Taís](https://github.com/ohanatais) — Senior PM, construindo em público.*
*Parte do ecossistema [build-from-zero](https://github.com/ohanatais/build-from-zero).*
