## Dapper and Dommel Simple Example

Não é nenhuma novidade usar um _ORM _para acessar um banco de dados, mas se na sua empresa e/ou projeto que está trabalhando ainda é usado _ADO.NET_, ou se você precisa de uma implementação bem simples mas poderosa em questão de produtividade e funcionalidade, ou até mesmo dar uma boa organizada/refatorada naquele projeto já obsoleto, aqui vai uma boa dica.

Para quem já usou o **Entity Framework** ou **NHibernate** sabe que _ORMs_ poderosos com grandes funcionalidades e implementações, mas às vezes ficamos podados em usá-los por conta de vários fatores.

Se o banco não está muito bem modelado, ou o cenário está maçante de trabalhar com a camada de persistência, contém aquelas milhões de _procedures_ e _functions_, onde não tem repositório (_**Repository Pattern**_), quiçá uma camada de acesso à dados, às vezes usar um ORM mais parrudo pode não ser a melhor saída, talvez onere mais ainda as consultas com o banco e pode deixar a aplicação mais lenta.

O _Dapper_ também não é novidade, teve sua primeira versão em 2011 disponível para download no _Nuget_ . Para você programador vai uma informação legal. Sabe aquela nossa bíblia chamada _Stackoverflow_? É feito com _Dapper_. Entretanto em contato com alguns programadores o mencionei, e não o conheciam, e os que conheciam, não sabiam que era possível essa implementação com _Linq_ e _Lambda _e por isso resolvi escrever esse artigo, pois sei que existem vários cenários que podemos melhorar. Nos blogs de hoje em dia se postam várias novidades e se esquecem/não se importam com os casos já começados e que precisam de uma revigorada.

Sei que é inevitável, mas não podemos comparar o uso dessa abordagem com o _**Entity Framework**_ ou _**NHibernate**_, seria até desonesto, mas podemos comparar com o _ADO_. O que quero mostrar é um modo bem simples e muito produtivo de se trabalhar com o _micro-orm_ e que pode poupar bastante código. Existem milhões de abordagens melhores do que essa, principalmente na gringa, mas acho válido fazer esse artigo. Espero que gostem!

### Atenção toda essa abordagem funciona até a versão 4.5.1 do .NET após isso não irá funcionar por conta de restrição dos pacotes instalados.

Você que usa _ADO_, gostaria de reduzir seu código na camada de dados e usar _Linq_ e expressões Lambda para fazer consultas no banco?

[Clique aqui](http://filipececcon.com.br/tecnologia/c-usando-dapper-com-fluentmap-linq-e-lambda-para-consultas/) e veja a explicação completa dessa implementação no blog
