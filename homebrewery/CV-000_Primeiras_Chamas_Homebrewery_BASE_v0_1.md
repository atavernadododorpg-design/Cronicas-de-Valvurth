<style>
/* =========================================================
   CRÔNICAS DE VALVURTH — PRIMEIRAS CHAMAS
   Template-base para Homebrewery V3
   Formato A4, identidade própria e sem dependência do tema PHB
   ========================================================= */

@page {
  size: A4;
  margin: 0;
}

.page {
  width: 210mm;
  height: 297mm;
  padding: 16mm 17mm 15mm 17mm;
  box-sizing: border-box;
  overflow: hidden;

  /* Fundo-base provisório. Substitua por imagem própria se desejar. */
  background:
    linear-gradient(rgba(249,245,236,.97), rgba(249,245,236,.97)),
    url('URL_FUNDO_PAPEL');
  background-size: cover;

  color: #2c2723;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 9.6pt;
  line-height: 1.25;
  column-count: 2;
  column-gap: 11mm;
}

/* Cabeçalhos */
.page h1,
.page h2,
.page h3 {
  font-family: "Aptos Display", "Trebuchet MS", Georgia, serif;
  color: #7a2e1d;
  break-after: avoid;
}

.page h1 {
  font-size: 23pt;
  line-height: 1;
  margin: 0 0 5mm 0;
  border-bottom: 1.2px solid #b78757;
  padding-bottom: 2mm;
}

.page h2 {
  font-size: 14pt;
  line-height: 1.05;
  margin: 4mm 0 1.5mm 0;
}

.page h3 {
  font-size: 11pt;
  margin: 3mm 0 1mm 0;
}

/* Parágrafos e listas */
.page p {
  margin: 0 0 2.4mm 0;
  text-align: justify;
  hyphens: auto;
}

.page ul {
  margin: 1.2mm 0 2.5mm 5mm;
  padding-left: 3mm;
}

.page li {
  margin-bottom: .8mm;
}

/* Links */
.page a {
  color: #7a2e1d;
  text-decoration: none;
}

/* Ênfase narrativa */
.emphasis {
  margin: 4mm 3mm;
  padding: 3mm 4mm;
  border-left: 3px solid #b78757;
  background: rgba(183,135,87,.10);
  font-style: italic;
  font-size: 10.2pt;
}

/* Caixa editorial */
.box {
  margin: 3mm 0;
  padding: 3mm 4mm;
  border: 1px solid rgba(122,46,29,.45);
  background: rgba(255,255,255,.46);
  break-inside: avoid;
}

.box h2, .box h3 {
  margin-top: 0;
}

/* Imagens */
.full-bleed {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: -2;
}

.image-frame {
  width: 100%;
  min-height: 55mm;
  margin: 3mm 0;
  border: 1px solid rgba(122,46,29,.35);
  background: rgba(100,80,65,.08);
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: #806f62;
  font-style: italic;
}

/* Página em uma coluna */
.page:nth-of-type(1),
.page:nth-of-type(6),
.page:nth-of-type(11),
.page:nth-of-type(16) {
  column-count: 1;
}

/* Capa */
.page:nth-of-type(1) {
  padding: 0;
  color: #f7efe2;
  text-shadow: 0 2px 8px rgba(0,0,0,.75);
  background: #17120f;
}

.cover-copy {
  position: absolute;
  inset: 0;
  padding: 18mm 16mm;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  z-index: 2;
}

.cover-copy .series {
  margin-top: 3mm;
  font: 700 12pt "Trebuchet MS", sans-serif;
  letter-spacing: .12em;
}

.cover-copy .line {
  margin-top: 2mm;
  font: 700 10pt "Trebuchet MS", sans-serif;
  letter-spacing: .22em;
}

.cover-copy .setting {
  margin-top: 14mm;
  font: 700 19pt "Trebuchet MS", sans-serif;
  letter-spacing: .08em;
}

.cover-copy .title {
  margin-top: 5mm;
  font: 800 34pt "Trebuchet MS", sans-serif;
  line-height: .95;
  text-transform: uppercase;
}

.cover-copy .subtitle {
  margin-top: 4mm;
  font: italic 13pt Georgia, serif;
}

.cover-copy .author {
  margin-top: auto;
  margin-bottom: 8mm;
  font: 700 11pt "Trebuchet MS", sans-serif;
}

/* Mapa */
.map-page .map {
  width: 100%;
  height: 185mm;
  object-fit: contain;
  margin-top: 5mm;
}

/* Gerador */
.generator-grid {
  columns: 2;
  column-gap: 7mm;
}

.generator {
  break-inside: avoid;
  margin: 0 0 3mm 0;
}

.generator h3 {
  font-size: 9.5pt;
  margin-bottom: 1mm;
}

.generator table {
  width: 100%;
  border-collapse: collapse;
  font-size: 6.9pt;
  line-height: 1.1;
}

.generator th,
.generator td {
  padding: .7mm 1mm;
  border-bottom: .4px solid rgba(90,70,55,.25);
  vertical-align: top;
}

.generator th {
  background: rgba(183,135,87,.18);
  text-align: left;
}

/* Rodapé visual */
.page::after {
  content: "CRÔNICAS DE VALVURTH  •  PRIMEIRAS CHAMAS";
  position: absolute;
  left: 17mm;
  right: 17mm;
  bottom: 6mm;
  text-align: center;
  font: 6.5pt "Trebuchet MS", sans-serif;
  letter-spacing: .08em;
  color: rgba(70,55,45,.55);
}

.page:nth-of-type(1)::after {
  content: "";
}

/* Número de página */
.pageNumber {
  color: rgba(70,55,45,.65);
  font-family: "Trebuchet MS", sans-serif;
  font-size: 7pt;
}

/* Tabelas gerais */
.page table {
  max-width: 100%;
}

/* Impressão */
@media print {
  .page {
    box-shadow: none !important;
  }
}
</style>

<img class="full-bleed" src="URL_ARTE_CAPA" alt="A Salmão em Piracema retorna contra a corrente ao entardecer diante de Candelária Velha">

<div class="cover-copy">
  <div class="series">CRÔNICAS DE VALVURTH</div>
  <div class="line">VÉSPERA</div>
  <div class="setting">CANDELÁRIA VELHA</div>
  <div class="title">Primeiras Chamas</div>
  <div class="subtitle">Guia Introdutório Gratuito de Candelária Velha</div>
  <div class="author">DAN UMBALI</div>
</div>

\page

# Sobre este Guia

Primeiras Chamas é um guia introdutório gratuito para Candelária Velha, um cenário de fantasia medieval urbana pertencente ao universo Crônicas de Valvurth.

Seu objetivo é apresentar a atmosfera, a identidade e as possibilidades de aventura da Cidade das Chamas Baixas, oferecendo material suficiente para inspirar mestres e jogadores a iniciarem suas próprias histórias.

Este guia foi concebido como uma porta de entrada para a coleção. Os demais volumes aprofundam a cidade, seus lugares notáveis, facções, personagens e ferramentas para criação de aventuras.

## Créditos

Criação, texto e direção editorial: Dan Umbali

Projeto: Crônicas de Valvurth

Linha editorial: Véspera

## Agradecimento

Obrigado por dedicar seu tempo para conhecer Candelária Velha.

Espero que estas páginas despertem a mesma curiosidade que motivou sua criação e que, em breve, você também encontre seu lugar entre as pequenas chamas da cidade.

Se este material lhe proporcionar uma boa aventura, considere acompanhar os próximos volumes da coleção.

Boa leitura.

## Direitos Autorais e Distribuição

© 2026 Dan Umbali. Todos os direitos reservados.

Esta obra é uma criação original pertencente ao universo Crônicas de Valvurth.

Este guia é disponibilizado gratuitamente pelo autor. Para garantir acesso à versão mais recente e apoiar o crescimento de Crônicas de Valvurth, compartilhe o link oficial de download, e não o arquivo em si.

## Versão

Primeira edição • Versão 1.0

\page

# Bem-vindo a Candelária Velha

Há cidades que crescem ao redor de castelos.

Outras surgem junto ao mar.

<div class="emphasis">Candelária Velha nasceu em torno daquilo que seus habitantes nunca conseguiram abandonar: o rio.</div>

Durante o dia, mercadores disputam espaço nas ruas estreitas, artesãos preservam tradições centenárias e embarcações percorrem o Rio Cristal Velho carregando mercadorias, promessas e histórias.

Quando a noite chega, porém, Candelária muda.

Os lampiões são acesos um a um. As portas se fecham mais cedo. As conversas tornam-se mais baixas.

E quase ninguém permanece muito tempo olhando para a corrente do rio.

<div class="emphasis">Porque algumas histórias insistem em voltar para casa.</div>

## O que você encontrará neste guia

Primeiras Chamas apresenta os primeiros passos para explorar Candelária Velha. Nestas páginas você conhecerá:

- a atmosfera da Cidade das Chamas Baixas;

- seus principais distritos;

- costumes e tradições;

- a Salmão em Piracema, a mais famosa estalagem fluvial da região;

- alguns dos personagens que moldam a vida cotidiana;

- rumores e ferramentas para começar a jogar imediatamente.

O conteúdo foi desenvolvido para que Candelária Velha funcione tanto como cidade-base quanto integrada facilmente a outros mundos de fantasia medieval.

## Continue explorando

Este é apenas o começo. Os próximos volumes aprofundam lugares notáveis, facções, personagens e mistérios, oferecendo novas ferramentas para campanhas de investigação, exploração urbana e intriga política.

<div class="emphasis">Acenda a primeira chama. O restante de Candelária espera por você.</div>

\page

# A Cidade das Chamas Baixas

À primeira vista, Candelária Velha parece apenas mais uma antiga cidade erguida às margens de um grande rio. Muralhas de pedra cercam seus bairros, pontes unem margens movimentadas e embarcações cruzam diariamente o Rio Cristal Velho levando pessoas, mercadorias e notícias para toda a região de Véspera.

Basta permanecer por alguns dias, porém, para perceber que há algo diferente.

Candelária aprendeu a conviver com o passado sem jamais conseguir esquecê-lo.

Ruínas muito mais antigas permanecem escondidas sob suas ruas. Histórias contraditórias atravessam gerações como lembranças de uma mesma família. Em cada bairro existem costumes preservados há séculos, juramentos repetidos quase sem que seus habitantes saibam a origem e pequenas tradições que parecem manter tudo unido diante da passagem do tempo.

Durante o dia, Candelária é vibrante. Mercados lotados, oficinas, embarcações, ferrarias, tavernas e caravanas transformam suas ruas em um encontro constante de culturas, sotaques e interesses.

À medida que o sol desaparece, porém, o ritmo muda.

Os lampiões tornam-se as verdadeiras estrelas. As ruas ficam mais silenciosas. Janelas se fecham. Poucos permanecem próximos ao rio sem um bom motivo.

<div class="emphasis">Em Candelária Velha, a noite nunca é apenas a ausência do dia. Ela faz parte da identidade do lugar.</div>

## Por que jogar em Candelária Velha?

Candelária funciona especialmente bem como cidade-base para campanhas de fantasia medieval.

Aqui, os personagens podem investigar mistérios antigos, negociar com mercadores, envolver-se em disputas políticas, explorar passagens subterrâneas, proteger rotas comerciais ou descobrir por que tantos habitantes evitam falar sobre determinados lugares depois que os lampiões são acesos.

<div class="emphasis">Cada rua pode esconder uma história. Cada ponte liga mais do que duas margens. E cada chama acesa representa a esperança de que algumas memórias permaneçam exatamente onde deveriam estar.</div>

\page

# A Cidade Viva

Em Candelária Velha, cada amanhecer começa com o som das embarcações deslizando pelo Rio Cristal Velho. Mercadores organizam suas barracas antes mesmo do nascer do sol, padeiros acendem os primeiros fornos e artesãos abrem as portas de oficinas que pertencem às mesmas famílias há gerações.

As ruas raramente permanec silenciosas. O Mercado Cem Vozes transforma diferentes sotaques em um único murmúrio. Ferreiros trabalham lado a lado com escribas, marinheiros negociam com viajantes recém-chegados e crianças atravessam becos que conhecem melhor do que qualquer adulto.

À medida que a tarde termina, o ritmo desacelera. Comerciantes recolhem mercadorias, embarcações procuram um lugar seguro para atracar e os lampiões anunciam que uma nova noite se aproxima.

Não existe toque de recolher. Mas há hábitos que ninguém questiona.

Algumas ruas ficam vazias. Certas portas permanecem fechadas. E poucos aceitam atravessar o rio depois de escurecer.

<div class="emphasis">Nem sempre por superstição.</div>

## Aventuras em cada esquina

Candelária Velha foi construída para servir como um lugar onde personagens podem permanecer durante muitas sessões. Entre uma expedição e outra, os aventureiros sempre encontram algo para fazer:

- investigar um desaparecimento;

- negociar com mercadores;

- aceitar um trabalho na Salmão em Piracema;

- seguir um rumor ouvido em uma taverna;

- mediar conflitos entre grupos influentes;

- explorar antigos túneis esquecidos;

- descobrir segredos preservados pelas famílias mais antigas.

Em Candelária, nem toda aventura começa com um dragão.

<div class="emphasis">Às vezes, basta uma conversa interrompida na mesa ao lado.</div>

\page

<div class="map-page">

# Caminhando por Candelária Velha

Uma boa cidade pode ser explorada de muitas maneiras.

Alguns visitantes procuram riqueza. Outros chegam em busca de respostas. Há quem atravesse seus portões apenas para encontrar um velho amigo ou esquecer um passado distante.

Em Candelária Velha, cada distrito possui personalidade própria, desafios distintos e histórias esperando para serem descobertas.

Use o mapa como ponto de partida para escolher onde sua próxima aventura começará.

<img class="map" src="URL_MAPA_CANDELARIA" alt="Mapa de Candelária Velha">

## Primeira visita?

Na primeira sessão, permita que os personagens caminhem livremente antes de apresentar um grande conflito.

Uma conversa em uma taverna, um mercado movimentado ou uma rua silenciosa ao cair da noite revela mais sobre Candelária do que qualquer descrição.

</div>

\page

# Distritos em um Relance

Cada região de Candelária possui um ritmo próprio. Escolha um distrito, apresente sua primeira impressão e deixe que uma oportunidade de aventura conduza os personagens para dentro da cidade.

## Distrito das Velas Frias

**Primeira impressão:** Templos, arquivos e edifícios administrativos iluminados por velas que raramente se apagam.

**Você vai até lá para...** procurar autoridades, registros antigos, auxílio religioso ou respostas sobre as tradições.

**Oportunidade de aventura:** Durante uma vigília silenciosa, uma vela acende sozinha diante do nome de alguém que ainda está vivo.

## Bairro da Bigorna Velha

**Primeira impressão:** Fornalhas, fuligem e o som incessante de metal trabalhado por famílias de artesãos.

**Você vai até lá para...** comprar ou reparar equipamentos, encontrar trabalhadores especializados ou investigar disputas entre oficinas.

**Oportunidade de aventura:** Uma ferramenta marcada com o símbolo de uma família desaparecida surge em uma forja que jura nunca tê-la recebido.

## Bairro das Três Cordas

**Primeira impressão:** Tavernas, pensões, música de rua e uma multidão que transforma rumores em moeda.

**Você vai até lá para...** encontrar hospedagem, ouvir histórias, contratar ajuda ou desaparecer entre trabalhadores e viajantes.

**Oportunidade de aventura:** Um músico interrompe a apresentação ao reconhecer um dos personagens em uma canção muito mais antiga que ele.

## Bairro do Eco Longo

**Primeira impressão:** Casarões decadentes, jardins secos e ruas largas demais, onde toda voz parece retornar diferente.

**Você vai até lá para...** investigar famílias antigas, casas abandonadas, desaparecimentos ou sons vindos dos subterrâneos.

**Oportunidade de aventura:** Uma voz chama um personagem pelo nome de dentro de uma residência fechada há décadas.

## Mercado Cem Vozes

**Primeira impressão:** Barracas, pregadores, artesãos, estrangeiros e negociações acontecendo em todas as direções.

**Você vai até lá para...** comprar, vender, contratar serviços, reunir informações ou cruzar com praticamente qualquer pessoa.

**Oportunidade de aventura:** Um carregamento desaparece entre o cais e o mercado, embora dezenas de testemunhas afirmem tê-lo visto chegar.

<div class="emphasis">Mas Candelária é muito mais do que ruas e bairros. Alguns lugares a tornam inesquecível.</div>

\page

# A Salmão em Piracema

Muitas cidades possuem um lugar onde histórias começam.

Em Candelária Velha, esse lugar não permanece no mesmo cais por muito tempo.

Durante o dia, a Salmão em Piracema percorre lentamente o Rio Cristal Velho, transportando viajantes, mercadores, artistas, aventureiros e curiosos entre diferentes pontos. À primeira vista, parece apenas uma grande embarcação adaptada para servir comida, oferecer abrigo e receber visitantes.

Mas basta voltar ao entardecer para perceber que ela é diferente.

Enquanto outras embarcações procuram um lugar seguro para atracar, a Salmão inicia sua última viagem. Silenciosamente, retorna à cidade contra a corrente do rio.

Ninguém parece estranhar. Os frequentadores apenas levantam os olhos por um instante antes de continuar suas conversas, como se aquele movimento desafiasse menos as leis da natureza do que a rotina de todos os dias.

Ao longo dos anos, a Salmão em Piracema tornou-se um ponto de encontro para quem procura trabalho, deseja trocar informações ou simplesmente ouvir histórias trazidas pelos viajantes.

Rumores percorrem suas mesas antes de alcançar as ruas. Aventureiros encontram contratantes. Mercadores descobrem oportunidades. Velhos marinheiros recordam acontecimentos que ninguém consegue confirmar.

E, vez ou outra, alguém aparece procurando respostas para perguntas que talvez nunca devessem ter sido feitas.

## Um excelente ponto de partida

Para iniciar uma campanha em Candelária Velha, faça os personagens chegarem pela Salmão em Piracema.

Além de abrigo, comida e informações, a embarcação reúne naturalmente pessoas de diferentes origens e interesses, facilitando a apresentação de aliados, rivais, empregadores e primeiros rumores sem parecer forçado.

Poucos lugares representam tão bem o espírito de Candelária.

<div class="emphasis">Mas, por mais conhecida que seja a Salmão em Piracema, poucas pessoas conhecem realmente a mulher que a conduz.</div>

\page

# Mara “Sete Nós”

Poucas pessoas conhecem Candelária Velha tão bem quanto Mara “Sete Nós”.

Proprietária da Salmão em Piracema, ela passa boa parte dos dias navegando pelo Rio Cristal Velho, ouvindo histórias, observando pessoas e percebendo mudanças muito antes que elas se tornem assunto nas ruas.

Mara raramente faz perguntas diretas. Prefere servir uma refeição quente, ouvir em silêncio e deixar que seus visitantes contem muito mais do que pretendiam.

Esse hábito lhe rendeu uma reputação curiosa. Há quem diga que ela conhece todos os rumores de Candelária. Outros juram que sempre sabe quando alguém está mentindo.

Ela apenas sorri e continua trabalhando.

## Uma anfitriã para aventureiros

A Salmão em Piracema costuma ser o primeiro lugar recomendado a quem chega.

Mara recebe desconhecidos com naturalidade, aproxima pessoas que podem ajudar umas às outras e, quando percebe potencial em um grupo de aventureiros, costuma indicar pequenos trabalhos, contatos ou problemas que precisam de atenção.

Ela nunca parece apressada. Nem surpresa. Como se soubesse que cada pessoa chega exatamente quando deveria.

## Interpretando Mara

Ao utilizá-la em jogo, pense menos em uma estalajadeira e mais em alguém que conhece profundamente sua cidade.

Ela fala pouco, observa muito e raramente oferece respostas completas. Em vez disso, devolve perguntas, sugere caminhos ou apresenta pessoas capazes de ajudar.

Sua função não é resolver problemas. É colocar a aventura em movimento.

## Primeira missão

Quando os personagens perguntarem onde encontrar trabalho, Mara dificilmente responderá com um simples “sim” ou “não”.

Ela servirá mais uma rodada, olhará discretamente para outro canto da embarcação e dirá:

<div class="emphasis">“Talvez vocês devam conversar com aquela pessoa antes que ela desista de esperar.”</div>

É assim que muitas aventuras começam em Candelária Velha.

<div class="emphasis">Mas nem todos os frequentadores da Salmão procuram apenas trabalho. Alguns carregam histórias que jamais deveriam ter chegado à cidade.</div>

\page

# Começando em Candelária Velha

A maneira mais simples de iniciar uma campanha é reunir os personagens como passageiros da Salmão em Piracema.

Alguns podem estar chegando pela primeira vez. Outros retornam após anos de ausência. Talvez tenham sido contratados para o mesmo trabalho; talvez apenas compartilhem a embarcação por acaso.

O importante é que todos tenham um motivo para permanecer em Candelária quando a viagem terminar.

Enquanto a Salmão segue pelo Rio Cristal Velho, os personagens têm tempo para conversar, observar a cidade se aproximando e conhecer alguns de seus futuros companheiros antes que a aventura realmente comece.

Quando atracam, Candelária já está pronta para recebê-los.

## Três maneiras de começar

## O desaparecimento

Um morador procura ajuda para encontrar alguém que desapareceu poucos dias atrás. As pistas levam a diferentes bairros, mas ninguém consegue contar exatamente a mesma versão dos acontecimentos.

## O pacote errado

Durante a viagem, um pequeno embrulho é entregue aos personagens por engano. Antes que consigam devolvê-lo, outras pessoas começam a procurá-lo desesperadamente.

## Um favor para Mara

Antes do desembarque, Mara pede aos aventureiros que entreguem uma carta a um antigo conhecido. O pedido parece simples — até descobrirem que o destinatário desapareceu na noite anterior.

## Dicas para o Mestre

Nas primeiras sessões, apresente Candelária Velha aos poucos. Permita que os jogadores conheçam tavernas, mercados, pontes, moradores e costumes antes de revelar conflitos maiores.

Candelária recompensa grupos curiosos. Quanto mais os personagens conversarem com seus habitantes e explorarem seus bairros, mais naturalmente os mistérios aparecerão.

Não tenha pressa. O cenário funciona melhor quando parece um lugar vivo, onde a aventura nasce das pessoas e das relações construídas ao longo do tempo.

<div class="emphasis">E, quando os personagens acreditarem que já conhecem Candelária, descobrirão que ela guarda muito mais do que ruas, tavernas e velhos rumores.</div>

\page

# Acenda uma Chama

Uma história em Candelária Velha pode começar com um rumor, uma carta esquecida, uma discussão no mercado, um barco que chega tarde demais ou uma única pergunta.

Role uma vez em cada tabela. Em poucos minutos você terá um conflito, personagens envolvidos e um mistério pronto para desenvolver. Cada resultado é apenas o começo; as respostas pertencem ao seu grupo.

<div class="generator-grid">

<div class="generator">

### Passo 1 — Como tudo começa?

| d8 | Resultado |
|---:|:---|
| 1 | Um velho rumor volta a circular pela cidade. |
| 2 | Alguém pede ajuda discretamente aos personagens. |
| 3 | Um objeto é encontrado onde não deveria estar. |
| 4 | Uma pessoa desapareceu durante a noite. |
| 5 | Uma discussão pública termina de forma inesperada. |
| 6 | Uma embarcação chega trazendo más notícias. |
| 7 | Um favor antigo finalmente é cobrado. |
| 8 | Um estranho procura alguém que ninguém admite conhecer. |

</div>

<div class="generator">

### Passo 2 — Quem procura os aventureiros?

| d8 | Resultado |
|---:|:---|
| 1 | Mara “Sete Nós”. |
| 2 | Um comerciante do Mercado Cem Vozes. |
| 3 | Um guarda da cidade. |
| 4 | Um pescador veterano. |
| 5 | Uma artesã conhecida. |
| 6 | Um sacerdote local. |
| 7 | Uma criança curiosa. |
| 8 | Um viajante recém-chegado. |

</div>

<div class="generator">

### Passo 3 — Onde tudo acontece?

| d8 | Resultado |
|---:|:---|
| 1 | Salmão em Piracema. |
| 2 | Mercado Cem Vozes. |
| 3 | Cais do Rio Cristal Velho. |
| 4 | Uma ponte antiga. |
| 5 | Um beco estreito. |
| 6 | Um velho armazém. |
| 7 | Próximo às muralhas. |
| 8 | Em uma rua quase vazia ao anoitecer. |

</div>

<div class="generator">

### Passo 4 — O que realmente está acontecendo?

| d8 | Resultado |
|---:|:---|
| 1 | O desaparecimento foi voluntário. |
| 2 | O verdadeiro alvo nunca foi quem todos imaginam. |
| 3 | Tudo começou muitos anos atrás. |
| 4 | Uma família importante está escondendo algo. |
| 5 | Uma mentira protege alguém inocente. |
| 6 | O objeto procurado nunca existiu. |
| 7 | Há duas versões igualmente verdadeiras da história. |
| 8 | Alguém está manipulando todos os envolvidos. |

</div>

<div class="generator">

### Passo 5 — O que complica a situação?

| d8 | Resultado |
|---:|:---|
| 1 | Os personagens têm apenas uma noite para agir. |
| 2 | Outro grupo investiga o mesmo caso. |
| 3 | Um incêndio muda completamente a situação. |
| 4 | Uma forte tempestade interrompe a cidade. |
| 5 | Um inocente torna-se o principal suspeito. |
| 6 | O principal aliado desaparece. |
| 7 | Uma testemunha decide mentir. |
| 8 | Os personagens passam a ser considerados culpados. |

</div>

<div class="generator">

### Passo 6 — Qual é o verdadeiro dilema?

| d8 | Resultado |
|---:|:---|
| 1 | Salvar uma pessoa ou descobrir toda a verdade. |
| 2 | Cumprir a lei ou fazer justiça. |
| 3 | Proteger um amigo ou concluir a missão. |
| 4 | Revelar um segredo ou preservar uma família. |
| 5 | Aceitar uma recompensa ou fazer o que é certo. |
| 6 | Confiar na única pessoa que parece culpada. |
| 7 | Escolher entre duas vítimas igualmente inocentes. |
| 8 | Resolver o caso ou impedir uma tragédia maior. |

</div>

</div>

## Exemplo

Um objeto é encontrado onde não deveria estar; Mara “Sete Nós” pede ajuda; tudo acontece no Mercado Cem Vozes; uma família importante esconde a verdade; outro grupo investiga o mesmo caso; e os personagens precisam escolher entre cumprir a lei e fazer justiça.

Em poucos minutos, você já possui o esqueleto de uma aventura inédita.

\page

# As Chamas que Mantêm a Cidade Viva

Candelária Velha não é definida apenas por seus lugares ou habitantes.

Ela vive dos conflitos que nunca são completamente resolvidos.

<div class="emphasis">É nesses espaços entre interesses, medos e esperanças que surgem as melhores histórias.</div>

## O rio alimenta Candelária — e também guarda seus segredos

O Rio Cristal Velho é a razão da existência de Candelária. Por ele chegam riquezas, viajantes e notícias. Mas suas águas também carregam histórias esquecidas, objetos perdidos e perguntas que muitos prefeririam nunca responder.

**Em jogo:** desaparecimentos, cargas misteriosas, descobertas inesperadas e rumores que descem o rio antes mesmo de qualquer embarcação.

**Pergunta para o Mestre:** O que chegou hoje pelo rio... e quem gostaria que isso nunca tivesse chegado?

## Tradição ou mudança?

Alguns habitantes acreditam que Candelária prospera porque preserva seus costumes. Outros defendem que precisa mudar para sobreviver. Entre esses extremos, comerciantes, artesãos, famílias antigas e recém-chegados disputam silenciosamente o futuro.

**Em jogo:** reformas, disputas políticas, rivalidades familiares e decisões que dividem a população.

**Pergunta para o Mestre:** O que vale mais: preservar um costume centenário ou resolver um problema de hoje?

## Toda informação tem um preço

Rumores circulam com a mesma velocidade das embarcações. Nem sempre quem sabe mais é quem fala mais. Em Candelária, favores, segredos e informações valem tanto quanto ouro.

**Em jogo:** chantagens, espionagem, documentos desaparecidos e alianças improváveis.

**Pergunta para o Mestre:** Quem realmente se beneficia quando um segredo deixa de ser segredo?

\page

# As Chamas que Mantêm a Cidade Viva

## Há histórias que Candelária prefere esquecer

Ruínas antigas, passagens subterrâneas e acontecimentos pouco comentados fazem parte da memória de Candelária Velha. Nem todos desejam que essas histórias voltem à superfície.

**Em jogo:** investigações, descobertas arqueológicas, antigas promessas e mistérios familiares.

**Pergunta para o Mestre:** O que alguém faria para impedir que o passado fosse descoberto?

## Ninguém vive sozinho

Mercadores, pescadores, guardas, artesãos, sacerdotes e viajantes dependem uns dos outros. Um pequeno conflito entre duas pessoas pode transformar-se rapidamente em um problema para toda a cidade.

**Em jogo:** disputas comerciais, favores, reconciliações, vinganças e alianças inesperadas.

**Pergunta para o Mestre:** Quem realmente será afetado pela decisão dos personagens?

## Toda chama ilumina... e projeta sombras

Candelária Velha recompensa personagens curiosos. Quanto mais eles exploram suas ruas, mais descobrem que cada resposta conduz naturalmente a uma nova pergunta.

É assim que campanhas inteiras nascem:

- uma conversa interrompida;

- um objeto encontrado;

- uma promessa esquecida;

- uma embarcação chegando ao entardecer.

Toda grande história começa com uma pequena chama.

<div class="emphasis">E, quando os personagens finalmente acreditarem conhecer Candelária Velha, perceberão que ela é apenas uma entre muitas histórias de Véspera.</div>

\page

# O Próximo Passo

Candelária Velha foi feita para crescer junto com sua campanha.

Este guia apresentou apenas as primeiras chamas. Agora cabe a você decidir quais delas merecem continuar acesas.

Talvez seus personagens tenham se encantado pelas ruas movimentadas, pelos rumores entre mercadores ou pelas histórias contadas a bordo da Salmão em Piracema.

Talvez você queira conhecer melhor seus habitantes, descobrir o que existe por trás dos antigos segredos ou levar novas aventuras prontas à mesa.

Cada suplemento de Crônicas de Valvurth amplia um aspecto diferente de Candelária Velha, permitindo que o cenário cresça naturalmente conforme sua campanha evolui.

## Continue explorando

## A Cidade das Chamas Baixas

Descubra os bairros, a história, a cultura e a organização de Candelária Velha em profundidade.

## Lugares Notáveis

Explore tavernas, templos, oficinas, mercados e construções marcantes, cada um com histórias próprias e novas oportunidades de aventura.

## Rostos de Candelária

Conheça aliados, rivais e figuras influentes que moldam o cotidiano da Cidade das Chamas Baixas.

## Facções

Descubra as organizações que atuam nos bastidores e os interesses que movem Candelária Velha.

## Gerador de Aventuras

Crie novas histórias em poucos minutos com tabelas, ideias e ferramentas inspiradas no estilo narrativo da cidade.

Ainda existem muitas histórias esperando para ser descobertas.

<div class="emphasis">Qual será a próxima chama que você decidirá acender?</div>

\page

# Agora é a Sua Vez

Se você chegou até aqui, já conhece o suficiente para começar uma campanha em Candelária Velha.

Você sabe como é o cenário. Conheceu um lugar onde aventuras começam. Encontrou uma personagem capaz de reunir qualquer grupo. Descobriu conflitos que mantêm Candelária viva. E até criou sua primeira aventura.

Agora falta apenas uma coisa.

<div class="emphasis">Sentar à mesa.</div>

## Antes da primeira sessão...

Não tente mostrar tudo de uma vez.

Deixe que os personagens descubram Candelária do mesmo modo que seus habitantes a conheceram: caminhando por suas ruas, ouvindo histórias, fazendo perguntas e construindo relações.

Cada campanha encontrará uma cidade diferente. Alguns grupos lembrarão da Salmão em Piracema. Outros jamais esquecerão um rumor ouvido no mercado. Haverá aqueles que passarão meses tentando descobrir um único segredo.

Tudo isso faz parte da experiência.

## Faça de Candelária a sua cidade

Não tenha receio de criar novos moradores, inventar ruas, adicionar tavernas, construir tradições, mudar acontecimentos ou transformar um pequeno rumor em uma campanha inteira.

Candelária Velha não pretende limitar sua imaginação. Ela existe para inspirá-la.

<div class="emphasis">A melhor versão da cidade será sempre aquela construída pela sua mesa.</div>

## Quando sua campanha crescer...

Crônicas de Valvurth continuará esperando por você: novos lugares, novos personagens, novas histórias e novas ferramentas.

Sempre que sentir que chegou a hora de expandir sua campanha, haverá outra chama pronta para ser acesa.

<div class="emphasis">Porque cidades memoráveis não pertencem aos autores. Pertencem às histórias que nelas são vividas.</div>

\page

# A Última Chama

Algumas cidades existem apenas enquanto alguém as observa.

Outras permanecem vivas porque continuam sendo lembradas.

Candelária Velha pertence a um terceiro tipo.

Ela desperta sempre que uma mesa se reúne para contar uma nova história.

Quando os dados começam a rolar. Quando um rumor desperta curiosidade. Quando uma embarcação atraca ao entardecer. Quando um personagem decide fazer apenas mais uma pergunta.

É nesse instante que suas ruas voltam a ganhar vida. Seus mercados tornam a ficar cheios. Os lampiões se acendem. E o Rio Cristal Velho volta a seguir seu curso.

Talvez, daqui a alguns meses, seus jogadores não se lembrem do nome de todas as ruas. Talvez esqueçam parte dos acontecimentos.

Mas dificilmente esquecerão a primeira vez que chegaram à Salmão em Piracema. Ou a conversa que mudou completamente o rumo da campanha. Ou aquele pequeno rumor que parecia insignificante... até transformar-se na maior aventura do grupo.

É assim que cidades permanecem vivas.

<div class="emphasis">Não porque foram escritas. Mas porque continuam sendo vividas.</div>

Obrigado por acender esta primeira chama.

Nos encontraremos novamente em Candelária Velha.

Boa aventura.

Dan Umbali
Criador de Crônicas de Valvurth

<div class="image-frame">INSERIR QR CODE OFICIAL</div>

<div class="emphasis">Algumas cidades terminam quando a última página é lida.
Candelária Velha começa quando o livro é fechado.</div>