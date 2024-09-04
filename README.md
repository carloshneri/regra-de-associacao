# regra-de-associacao

As regras de associação é uma forma de relacionar dentro de um conjunto de items padrões de relacionamento em que X implica em Y.(X --> Y). As regras de associação podem ter diversos usos como verificar comportamento de clientes, campanha de marketing, gestão de estoque, definição de catálogo etc.

Algumas medidas podem ser tiradas qunado estamos trabalhando com a regra de associação como o suporte, confiança e lift que nos ajuda a ir criando alguns critérios para a formação das regras como por exemplo a criação de regras que satisfaça a um suporte minimo. Isso é importante já que o numero de regras cresce exponencialmente com o numero de itens da base.


Suporte mede a probabilidade de um determinada regra acontecer dentro do conjunto de dados.

suporte = Sup(X -> Y) = P(X u Y) = σ(X u Y)/n onde n é o numero de transações.
Serve para eliminar as regras menos interessantes.

Confiança verifica a ocorrência da parte consequente da regra.
Conf(X -> Y) = P(X|Y) = σ(X u Y)/σ(X)

Lift O Lift é uma medida que indica a força de associação entre dois itens, levando em conta a frequência de ambos no conjunto de dados. É calculado dividindo a confiança da associação pelo suporte do segundo item.

O Lift é usado para comparar a força da associação entre dois itens com a força esperada. Um valor de Lift maior que 1 indica uma associação positiva, ou seja, a ocorrência do antecedente aumenta a probabilidade do consequente.

Lift(X -> Y) = Conf(X -> Y)/σ(Y) = σ(X u Y)/σ(X) * σ(Y)
