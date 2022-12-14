Este material é um resumo e entendimento do livro [Atomic Design](https://atomicdesign.bradfrost.com/) de Brad Frost.

# Atomic Design

> É um erro assumir que uma página é uniforme, isolada e algo quantificável, quando na verdade é fluída, interativa e interdependente.

Não se pode dizer que um página inicial é fácil de fazer, e dar manutenção para 30 mil páginas de registros é difícil, pois precisa saber a composição delas. O segredo para ser fácil e com menor manutenção é a modularidade. Henry Ford aplicou a modularidade em sua empresa de automóveis onde "quebrou" o veículo em componente menores e modularizou o processo de montagem. O resultado foram carros mais uniformes, mais confiáveis, seguros e rápidos de fazer.

Da era das máquinas passou para a era dos computadores, e a modularidade foi aplicada nas linguagens de programação, muito antes da Web existir. A importância de se falar sobre isso agora é que há uma grande expansão acontecendo, com vários novos aparelhos, e a melhor forma de se preparar para isso é separar essas responsabilidades.

A cada, mais ou menos, 8 anos as empresas, não muito organizadas, refazem seus websites e os seus usuários precisam reaprender a usar seus sites. As páginas ficam com uma cara nova, mas o problema raiz não é tratado, que é "o novo hoje fica velho amanhã" e depois de 8 anos o site será novamente refeito e o ciclo de aprendizado do usuário se repete.

## Atmosfera de Design

É muito difícil desenhar uma interface para cada aparelho em que aparecerá, seja monitor, celular, tv... Por isso andy Clarke fala da importância da Atmosfera de Design, termo que evoluiu de Identidade Visual, onde oque mais importa não é o arranjo dos elementos, mas oque é visto e sentido em cada página e aparelho.

A designer Samantha Warren desenvolveu um conceito chamado Style Tyles onde o designer não mais gera as páginas a serem desenvolvidas e sim os artefatos, como cor, fonte, elementos visuais... Com isso os stackholders passam a ter mais liberdade e isso remove longas conversas e trabalho dos designers de gerar tela a tela.

Em 2010 Ethan Marcotte cunhou o tempo Web Design Responsivo, com isso os designers passam a criar layouts adaptados para múltiplos aparelhos obrviomente não foi apenas criar páginas que espicham e encolhem, pois cada parte da interface têm seus desafios e oportunidades.

Os frameworks são a base para o desenvolvimento de muitas websites. Os frameworks são conjuntos que orientam o desenvolvimento, porém um layout baseado em um framework específico fará o produto perder suas características, então, ao invés disso, cada site deve ter seu "[Bootstrap](https://getbootstrap.com/docs/5.0/)". Como diz o autor, "não é sobre usar um design system é sobre criar o seu".

## Style Guide

Para organizar um design system é essencial ter um Style Guide para organizar todo material, orientações, componentes, indetidade da marca, convenção de código... Isso tudo quando aplicado faz seu cliente acreditar mais em você, pois o seu site se torna mais coeso ao seguir um guia de estilos. Os stackholders passam a ver o site como um sistema e não apenas um amontoado de páginas onde cada um pensa que seu problema é unico e deve ser resolvido de uma forma diferente. Os desenvolvedores e designers também são educados pelo Style Guide e passam a saber que suas decisões afetam o Desigh Sytem como um todo.


### Identidade da Marca

Em resumo, Identidade da Marca é tudo que a torna única, seja sua logomarca, tipografia, paleta de cores, slogan e outros. Uma marca então deve ser coesa em todos os seus canais para que seu cliente a identifique e confie nela.

Outro termo importante é o Design Language que é semelhante a identidade da marca, porém mais filosófico.

### Bibliotecas de componentes

Assim que houver uma definição dos componentes pode existir essa lib, porém ela não deve ser considerada um "projeto auxiliar", pois na primeira redução de custos ela deixa de existir.

Estratégias de manutenção e governança são essenciais para o projeto não ser abandonado.

## Atomic Design - Metodologia

O Atomic Design foi inspirado na quimica e cada parte é uma fase da construção. A divisão é:

1. átomos
2. moléculas
3. organismos


### Átomos

Os átomos são os blocos base. São formados por elementos menores, mas assim como na matéria, o átomo é a menor parte funcional e para as interfaces é o menor elemento de uma interface. Exemplo botão, input, títulos.

## Moléculas

Na química, as moléculas são a junção de 2 ou mais átomos. Essa combinação traz novas propriedades. 

Em interfaces, **moléculas são simples grupos de elementos UI funcionando juntos como unidade.** A combinação dos átomos traz a eles um propósito. a criação desses componentes simples vão de acordo com o princípio da responsabilidade única, onde cada parte deve ser bem feita e testada, encorajando a reusabilidade e aumentando a consistência das interfaces.

