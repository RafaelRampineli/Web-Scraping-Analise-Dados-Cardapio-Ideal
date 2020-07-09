# Web-Scraping-Analise-Dados-Cardapio-Ideal

Laboratório 4 desenvolvido ao final do curso Bônus Web Scraping da Formação Cientista de Dados da Data Science Academy (DSA).

## Definição do Problema

Você saberia dizer quais são os ingredientes mais comuns nas refeições? E quais são os ingredientes que aparecem frequentemente juntos? E quais os métodos mais comuns no preparo de refeições? Qual a quantidade de porções usada com maior frequência? Qual a correlação entre os ingredientes para o cardápio ideal?

Responder essas e outras perguntas pode ajudar nutricionistas, escolas, restaurantes, indústrias de alimentos ou mesmo instituições de pesquisa, a fim de garantir que os padrões estejam sendo seguidos e que a saúde da população não esteja sendo comprometida com composições desbalanceadas de ingredientes.

Neste Lab vamos analisar um conjunto de dados pouco comum, mas que vai ajudar você a pensar em diferentes problemas e o mais importante, em diferentes soluções. A Ciência de Dados pode ser aplicada a qualquer área, desde que nossa matéria-prima esteja disponível: dados.

E para responder nossas perguntas, vamos extrair e analisar a composição de receitas. Sim, isso mesmo. Receitas. De risoto, de frango e até de Fettuccine Alfredo!

### O Web Scraping deste Lab é pesado e leva quase 50 minutos! Alguns parâmetros poderão reduzir esse tempo, mas nesse caso reduzirá também o volume de dados.

Para saber mais detalhes sobre alimentos e suas características, acesse:

<a href="https://www.abia.org.br/vsn/">ABIA - Associaçao Brasileira da Indústria de Alimentos</a>

Aqui tem um material de referência adicional que ajuda a explicar os benefícios da Ciência de Dados aplicada à Nutrição:

<a href="https://conferences.oreilly.com/strata/strata-ca-2019/public/schedule/detail/72551">Nutrition Data Science</a>

## Fonte de Dados

Nossa fonte de dados para o Web Scraping, será o portal <a href="https://www.allrecipes.com/">All Recipes</a> que contém receitas deliciosas. Navegue pelo site para compreender como os dados estão organizados. São várias páginas, cada qual com diversas receitas.

Observe que o <a href="https://www.allrecipes.com/">All Recipes</a> possui dois layouts HTML diferentes para suas páginas de receita, um layout regular e um layout que suporta a compra de ingredientes diretamente da página da receita. Esses dois layouts têm as informações que precisamos em locais diferentes, portanto, precisamos diferenciá-los durante a raspagem dos dados. Se o elemento de título que procuramos inicialmente estiver definido como 'Nenhum', precisamos procurar os elementos onde eles estariam no segundo layout (comprador).

Vamos então extrair diversas receitas, limpar os dados e avaliar ingredientes, métodos de preparo e outros dados disponíveis.
