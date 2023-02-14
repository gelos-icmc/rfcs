# Processo de RFCs no GELOS

## Resumo

Esse é um protótipo de método para tomada de decisões maiores dentro do grupo.
Estilo [RFCs](https://pt.wikipedia.org/wiki/Request_for_Comments).

A proposta envolve usar o modelo de RFCs (request for comments) para prototipar
decisões e soluções, prover feedback em cima deles, e, eventualmente, ter eles
mergeados nesse repositório representando o *status quo* (estado das coisas) do
grupo.

Essa idéia (usar RFCs no GELOS) está escrita num formato de RFC, para ilustrar
como um RFC funcionaria. Novos RFCs podem ser criados futuramente para refinar
esse processo.

## Problemática

Como toda organização, o GELOS é um grupo com tendência a [bike
shedding](https://en.wikipedia.org/wiki/Law_of_triviality), ou seja, evitar
discussões complexas se agarrando em pedaços triviais (ex: como fazer, a
ideologia por trás da idéia, etc) do problema.

Em 2022, isso foi um empecilho. As principais questões foram: elaboração de um
código de conduta/regimento; formato de reuniões e projetos. Esses "meta
problemas" organizacionais são complexos, e tomar decisões em cima deles é um
processo lento e desgastante. Um protótipo inicial acelera a solução, e é um
ponto de partida para uma solução ideal.

O formato de RFCs ajuda a vencer a inércia. Com RFCs, alguém com algumas horas
livres pode escrever uma proposta inicial, pedir comentários assíncronos, levar
o assunto para reunião, e, eventualmente, será decidido acatar ou não.

Foi comprovado, dado o uso desse formato em milhares de projetos, que ter uma
solução inicial e refiná-la é muito mais eficiente que tentar criar uma solução
"perfeita" desde o início.

Os RFCs surgiram no projeto ARPANET, e são usado na IETF, IAB, comunidades de
software livre, e globalmente para fazer designs detalhados e acionáveis.

## Design

Proponho que esse repositório (hoje no GitHub, mas no futuro pode ser um Gitea
ou GitLab hospedado por nós) seja uma representação do *status quo* do GELOS.
Os RFCs aqui contidos (e aprovados) mostram quais são as decisões (estilo
constituição) que tomamos, quando as tomamos, e como as tomamos.

RFCs podem ser revogados (ou expandidos) por outros RFCs. Sendo, assim, um
histórico de mudanças importantes.

### Repositório

Teremos uma pasta `rfcs` que conterá os RFCs mergeados e aprovados do GELOS.
Esse é o nosso RFC 1.

O branch `main` representa a política vigente; propostas para RFCs devem ser
escritas em novas branches (forks ou não), e, quando prontas para comentários,
deve ser criado um *pull request* pedindo a inclusão daquele RFC na nossa
branch `main`.

### Processo

A idéia é minimizar burocracia e acelerar mudanças (positivas) no grupo, bem
como ter um histórico de decisões. Dito isso, precisamos de algumas regras para
que a coisa seja justa, não trave, e represente consenso no grupo.

0. Tenha uma idéia!
1. Escreva o RFC. Coloque detalhes, argumentos convincentes, busque entender os
   impactos e pontos negativos da idéia. Crie um protótipo, caso faça sentido.
2. Crie um pull request. O PR receberá feedback do grupo, e você deve estar
   preparado para revisar e incorporar mudanças.
3. Encontre um co-autor. É obrigatório que haja pelo menos um membro apoiando e
   participando da idéia, para ajudar a refiná-la.
4. A idéia deve ser divulgada nos canais do grupo. Os membros darão feedback
   diretamente no PR, e também é possível levar o assunto para reuniões (que
   devem ter suas atas publicadas).
5. Quando houver feedback suficiente, deve haver um consenso geral ao redor da
   idéia. A diretoria também deve avaliar o RFC e tomar uma decisão conjunta, e
   escrevê-la como comentário no PR. O RFC entrará na fase final, que durará 10
   dias corridos.
6. Caso surjam novas questões relevantes ou o consenso do grupo seja diferente
   do consenso da diretoria, a fase final deve ser cancelada e o RFC voltará
   para a fase de feedback. 
7. Depois de 10 dias na fase final, o PR será mergeado ou fechado, com base no
   consenso do grupo e diretoria. RFCs rejeitados podem ser refinados e abertos
   como novos RFCs.
    - Em assuntos muito polêmicos, isto é, caso o RFC passe mais de um mês
        (contando a partir do primeiro feedback) sem um consenso, a diretoria
        deve votar entre aceitar ou rejeitar, sem mais mudanças ao texto.


## Alternativas

Existem alternativa mais fracas, mas que contam com o problema de "travar"
atividades e ser pouco transparentes:
- Tomar decisões fechadas.
- Tomar decisões abertas de maneira informal.

- Podemos fazer uma versão mais estrita. Uma forma é ter um grupo de trabalho
    (nomeado pelo grupo e aprovado pela diretoria) para cada RFC específico.
    Esse método é mais complexo, porém mais transparente e democrático.
    Pessoalmente acredito que faz sentido quando o grupo estiver maior.

## Questões

1. A diretoria está OK com um processo "legislativo" mais aberto?
2. O equilíbrio entre agilidade e organização está bom?
