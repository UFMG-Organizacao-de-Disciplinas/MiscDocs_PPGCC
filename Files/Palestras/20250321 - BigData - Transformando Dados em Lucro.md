# 21/03/2025 - Big Data - Transformando Dados em Lucro

## Manhã

### Gustavo Ioschpe

- "Se você tá copiando, você tem teto. Se você tá criando, você não tem teto"
- "No mundo corporativo, demora décadas para que os avanços da academia sejam aplicados"
- "Vocês estão na área certa, no momento histórico certo"

---

- Descritivo;
- Preditivo
- Prescritivo;

| X       | Descritivo | Preditivo | Prescritivo |
| ------- | ---------: | --------: | ----------: |
| Usa IA? |        Não |       Sim |         Sim |
| ...     |            |           |             |
| ...     |            |           |             |
| ...     |            |           |             |

#### O que fazemos?

#### Temos mais de 17.000 variáveis

- "Quero todas as variáveis de todas as cidades de todos os períodos de tempo do Brasil"
- "Queremos colocar todas as informações pra dentro para encontrarmo as correlações mais malucas que temos"
- "Existem 32 tipos de kubitschek no brasil"
- Acharam uma base de dados com número de bueiros, andares de prédios..."

#### Nossos produtos

- Promopti: otimizar a disponibilização de descontos
- Priceo: um preço ótimo para cada produto; "preço é willness to pay"
- One-click order: "mais popular para indústrias que vendem pra lojas"
- Targatom: Targetting atomizado. Medir o potencial de vendas e lucros

"Quanto mais o cliente compra os produtos recomendados, mais desconto tem"

<https://www.inhire.com.br/carreiras-big-data>

### "Nalon"(?)

Como foi transitar da academia pro mercado?

Graduação e Mestrado na UFJF, e Doutorado com o Wagner Meira.

"Incômodo com muita coisa boa feita e que acabava engavetada"

Temas de pesquisa: ~sistemas de recomendação; aprendizado por reforço; Aprendizado por representação

"Quão importante é ter terminado a graduação, mestrado ou doutorado?"

"Queremos que vocês sejam bons solucionadores de problemas"

### Perguntas

- Pergunta do Meira: desde que você entrou até agora, o que que mudou na tecnologia?
  - Ferramentas melhores para tarefas específicas. Mas fundamentalmente a mudança essencial é bem menor. "No fim, a tecnologia é uma ferramente para resolver um problema que temos".

- Como que a empresa hoje lida com LGPD e propriedade intelectual?
  - Apesar de terem um grão bastante fino, eles não precisam de CPF, ou é com malha geográfica, ou setor censitário.
- O produto de vocês faz integração com [?] ?
  - Sim.
- Como vocês ficam quando o cliente não engaja na solução de vocês?
  - "Não é pela lógica, pela conversa e argumentação. É mostrando que dá dinheiro"
- E se o resultado encontrado não é positivo? E quando o resultado é quando o cliente não quer ouvir?
  - Esse não é produto deles. Eles apenas apontam
  - Recomendação de cerveja em cantinas de escola: não havia no banco de dados informações sobre quais lojas eram cantinas de escola, então eles cruzaram esses dados com o do MEC
- Mecanismos de coleta dos dados
  - às vezes floricultura não é o dado em si, mas sim uma proxy pra renda, então não é esperado uma floricultura numa periferia.
  - Sobre a parte técnica: pra crawlers:
    - Às vezes é só um wget na página.
    - às vezes tem que percorrer e paginar
    - Anúncios de imóveis por todo o Brasil
    - Usar Selenium pra navegar a página
    - AWS, Spark, Data Bricks
    - "Medalhão": processamento gradual dos dados em diversas camadas
- Alguma preocupação na ética do uso desses dados?
  - Tem, e é uma que os alegra: tudo o que fazem e (ganha/ganha). Não infrigem LGPD e são produtos que geram ganho social
  - Já foram chamados para trabalhar com empresas de arma e tabaco, mas recusaram.
- Como o ChatGPT impactou? Como definem se mantém algo ou jogam foram?
  - O GPT ajudou bastante e automatizou bastante o trabalho. Gerou um awareness da galera que é meio da idade da pedra.
  - Em 2019 ele teve uma conversa com a Johnson & Johnson nos EUA. "Algoritmo não é coisa de Website?"
  - "Se você usa o maps e não um mapa, pesquisa no google e não sai procurando, e se tudo isso te dá um ganho no seu dia a dia, por que no seu trabalho você também não faria?"
  - Sobre o descarte:
    - Há um sistema inteligente de descarte de dados. É barato armazenar, é caro processar esse dado.
- Falaram muito sobre mercado e varejo. Mas e indústria?
  - É melhor ser bom no que faz do que fazer várias coisas diferentes. Eles sentem que deve haver uma expansão muito forte pros EUA.
  - É um mercado vastíssimo, sem dúvida.

## Tarde

### Nalon

- Eles já fizeram isso de bolsa antes, e agora estão querendo retomar algo do gênero.
- Desejam aproximar a academia com o mercado.
- Meio "Livro de Elias"
- Programa de Residência:
  - A empresa queria se capacitar e o Departamento tinha essa capacidade com bolsistas, estagiários e professores.
- Atualmente não querem capacitar, mas sim aproximar.
- Off-site Trainee
- Quais seriam os temas? E de que forma se conectam com os desafios do BigData?
  
#### Sistemas de Recomendação: One-Click Order

- O que o produto faz?
  - Define quanto de cada produto o vendedor deve vender aos pontos de venda.
  - Olhar para a recorrência e estimar quanto comprará.
  - Ambev 430 itens diferentes
  - PdV = Ponto de Vendas
  - Existe também encontrar quais outros itens nunca antes comprados que podem passar a ser de interesse do comerciante.
  - Mercado Farma também tem muitos itens.
  - "Poucos SKU's que vendem muito"
    - [JV: O que será SKU? Já ouvi sobre isso antes]
  - Bebida, material de construção, etc.
  - Eles buscam otimizar também o nível de desconto de determinado produto
  - O desconto deve ser "mira laser", fazendo o pinpoint de quais os melhores descontos pros melhores clientes
  - "O desconto é autofinanciado"
    - Também tenta dar o desconto ao cliente para avançar na direção do que deseja comprar e forçar um pouco no máximo que poderia comprar.

##### Perguntas (One-Click Order)

- Desejam disponibilizar a gente o mar de dados para gente, favorecendo um ambiente adubado para podermos explorar nessa parte de pesquisa.
- "A gente tem o compromisso de colocar o que vocês fizerem na rua". "Nosso objetivo é realmente criar produtos pros nossos clientes". "O objetivo principal é criar um produto melhor e botar pra rodar".
- Pergunta JV: E, além do aprimoramento dos sistemas já existentes, vocês têm interesse em desenvolver novos produtos?
  - Resposta: É sempre uma dualidade. Queremos aprimorar os produtos existentes, geralmente guiados pelos desejos e pedidos dos clientes, mas à medida que avançamos também avaliamos novas possibilidades de sistemas
- "Eles não gostariam de limitar", afinal, os alunos, junto com professores podem trazer novas ideias que valeriam a pena testar e que eles antes não pensaram sobre.

- Atualmente eles já têm um produto funcionando automatizadamente. Existem n componentes que ficam variando ao longo do tempo, então ficam sempre reajustando alguns detalhes.

- Pergunta Samuel: Até que ponto vocês conseguem generalizar um determinado sistema aos diversos ambientes
  - Eles generalizam as diversas caixinhas de análises.
  - O que desejam é testar essas várias caixinhas para os diferentes sistemas.
  - É meio um lego. Um pipeline de dados.
  - Desejam não só aprimorar as caixinhas como também criar novas dessas caixinhas.

#### Reinforcement Learning

- É um problema de tomada de decisão sequencial
- No geral, querem gerar mais resultado
- Não tá tudo encodado no modelo de dados
- Mais uma vez, buscam a exploração
- Em certa vez eles fizeram o teste de adicionar 1 a mais no produto com maior taxa de compra a partir de um certo threshold e isso trouxe um grande resultado.

- Multi-armed Band (?) já foi usado
  - Eles rodaram e viram que determinados preços deram menor resultado, então devem se tornar menos recorrentes.
  - Outros que dão resultado passam a ser mais recorrentes.

- Problemas da operacionalidade
  - No BK não chegaram a trocar o preço durante o dia
  - No Drive Thru a troca dos valores muitas vezes ainda é no papelão
  - Erros nas bases de dados
  - "Se juntar os lucros dessas empresas deve dar uns 50% do PIB brasileiro"

#### Segmentação / Aprendizado por representação / Representation Learning

- Existem várias intercessões entre essas caixinhas de diversos produtos.
- Uma das coisas que desejam fazer é segmentar as lojas e produtos com as quais eles trabalham.
  - Indo desde um restaurante bacana até uma portinha que um cara faz o pedido.
- A maioria dos clientes fazem isso de forma muito estática
  - Bar pequeno, bar grande, VIP. 6, 8, 10 segmentos diferentes.
- Eles têm cacetadas de variáveis que podem ser usadas para refinar esses segmentos.
- Uma das coisas que fazem é criar novas bases de dados para refinar as variáveis.

- Eles desejam fugir um pouco dessa curadoria e passar a automarizar essas relações entre variáveis.
  - Word two vec
  - Com esse conceito eles desejam conseguir agregar os PdV's por similaridade entre eles.

##### Perguntas - Representation Learning

- Samuel: Já conseguiram fazer algo sobre isso?
  - Já, mas é uma complexidade tão difícil que não pararam alguém pra ficar analisando isso.
  - Cai na linha das coisas que já fez, é promissor, mas não exploraram tanto.

#### E como operacionaliza isso?

- Provavelmente a melhor forma seria com um Edital, uma seleção, bolsa de pesquisa envolvida.
- Devem fazer esse processo seletivo, o Meira deve definir os professores envolvidos.
- Evitando limitar o espaço de busca.

- Perguntas JV:
  - Valor de bolsa: tabela fapesp bolsa de pesquisa
    - Acúmulo segundo o Meira:
      - Acúmulo semântico: o projeto de pesquisa deve estar relacionado ao objetivo da bolsa
      - Acúmulo prático: tende a ser limitado pela necessidade de distribuição de bolsas. Se você tem bolsas acumuladas, a tendência é que você talvez tenha sua bolsa cortada. (ou algo assim)
  - Tempo: Deve seguir o que a universidade deve seguir como regras.
  - É um estilo mais bolsa de pesquisa do que "trainee de empresa".

- Pergunta Samuel: Existe a possibilidade de conseguir se associar à empresa sem atrelar ao edital

- Pergunta Rapaz: Vocês já têm alguma ideia de datas e vagas?
  - Em torno de 6 pessoas. 2 por linha de pesquisa. Relação entre graduação e pós-graduação.
  - E o tempo depende do edital. Eles não têm um prazo, mas querem fazer acontecer o mais rápido. Certamente tendem a ser mais restritos por causa das burocracias.
- Caso participemos com essa bolsa e depois queiram participar como funcionários, tendemos a ter preferência.
  - Há sim uma restrição protocolar dada pelo edital, mas se quiser podem manter contato.
