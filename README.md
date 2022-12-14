# Introdução a Java
Esse material contem os conceitos de lógica de programação através da linguagem de programação Java, para iniciantes.

A linguagem de programação Java é uma linguagem orientada a objetos e permite a criação de aplicações desktop, web, mobile.

o link da documentação oficial da linguagem é: https://docs.oracle.com/javase/8/docs/api/ ,  através da documentação você pode explorar mais a linguagem entendendo as bibliotecas que a linguagem oferece.

Nessa documentação vamos entender alguns conceitos iniciais e como estes podem ser explorados para um melhor entendimento da lógica de programação. O objetivo não será criar uma plataforma ou sistema e sim explorar a linguagem focando no entendimento da lógica. Esse ambiente de aprendizagem pode ser muito benéfico, já que vai gerar a confiança necessária para os próximos passos.

##  Primeiro passo, conceitos e sintaxe

A linguagem de programação Java, segue o paradigma de desenvolvimento chamado orientação a objetos, isso faz com que ao invés de escrevermos e tratarmos cada arquivo da aplicação como isolado, em certos momentos precisaremos fazer com que estes troquem informações, executem de forma coletiva as ações necessárias dentro da aplicação. É como em uma empresa onde para um produto ser entregue pronto ao cliente é necessário que a matéria prima passe por várias mãos, onde cada um dos colaboradores fará uma parte importante para o resultado final, e a entrega do produto ao cliente sempre será feita pelo departamento de balcão/ recepção. Sim temos um funcionário que entrega o resultado do produto e apenas ele pode faze-lo.  E parece bobeira essa analogia, não é mesmo? Mas guarde bem essa informação, vamos voltar a esse ponto em alguns momentos desse material.

A linguagem de programação Java, por seguir o paradigma orientado a objetos (OO), utiliza-se de alguns termos que precisamos conhecer e entender, pois se atuarmos no mercado com esta linguagem muito provavelmente vamos ouvir esses termos diariamente.


| Termo                | descrição                                                    |
| -------------------- | ------------------------------------------------------------ |
| **Classes**          | Geralmente os arquivos escritos na linguagem Java são chamados de classes, através das classes podemos definir os dados, ações que o programa vai armazenar, tratar e/ou executar. Sim as classes são estruturas que seguem uma sintaxe e podem conter métodos e/ou atributos, termos esses que vamos conhecer a seguir. Em uma analogia simplista podemos dizer que a classe é a folha onde escrevemos os ingredientes e ações necessárias para se fazer um bolo.<br /> **As classes possuem regras:** <br />*- ela deve ter um nome iniciado com letra maiúscula seguido de letras minúsculas; <br />- se tiver nome composto deve seguir o padrão Camel Case, cada nome iniciado com letra maiúscula ExemploDeNomeAceitavel;<br />- não pode ter acentos em seu nome ou caracteres especiais ou espaços em branco;* |
| **Atributos**        | Um atributo é uma característica passada dentro de uma classe, ela tem a função de ser uma propriedade dentro da classe. Se nossa classe é sobre um cliente e esse cliente possui característica dentro de um sistema, ou seja, um nome, uma data de nascimento, um CPF, e um e-mail, todas essas características que me permitem identificar esse cliente dentro do sistema, são sim atributos. <br />**Os atributos possuem algumas regras em sua escrita:**<br />*- escrita do nome do atributo deve ser em letra minúscula, sem caracteres especiais;<br />- a escrita do nome do atributo deve ser iniciado por letra não inicie o nome de um atributo por números;<br />- não utilize espaços em branco no nome dos atributos* |
| **Métodos**          | São ações realizadas dentro das classes, por exemplo se queremos criar uma estrutura para cadastrar um cliente, isso será um método, se precisamos deletar o cadastro desse cliente, isso também será uma ação feita por um método.<br />**Métodos tem uma regra de escrita:**<br />*- devem ter o seu nome escrito em letras minúsculas, sem acentos e sem caracteres especiais;*<br />- se o nome for composto, pode-se adotar o modelo camelCase, porem iniciando o primeiro nome com letra minúscula e os demais em caixa alta - exemploDeNomeDeMetodo<br />- não utilize espaços em branco no nome dos métodos* |
| **Método principal** | Esse é o método responsável por executar toda a aplicação, esse método deve receber o nome de **main**, os demais métodos podem auxiliar esse método principal, já que para a orientação a objetos temos alguns princípios de organização que são adotados em grande parte dos sistemas e frameworks. Voltando ao exemplo da analogia feita anteriormente, o método main é aquela pessoa responsável por entregar o produto ao cliente final. |
| **Bibliotecas**      | A linguagem Java possui uma ampla biblioteca com recursos prontos para uso, o que facilita o desenvolvimento e agiliza, essas bibliotecas assim como no mundo real são responsáveis por armazenar um acervo de informações, no mundo Java as bibliotecas possuem classes e métodos prontos para uso, que podem realizar ações desde uma simples impressão do dado no console, até mesmo cálculos, conversões de dados entre outras ações. |
| **Pacotes**          | As linguagens orientadas a objeto, precisam levar a organização muito a sério, isso porque teremos a informação caminhando de classe a classe até ser entregue a uma classe que possua o método main(principal), então se não mantermos uma organização mínima, podemos ter graves problemas para achar onde as coisas estão sendo tratadas. Além de colocar nome intuitivos nas classes, podemos então, organizar nosso sistemas dividindo as classes em pacotes ou **package**. São como pastas/diretórios de um computador, onde podemos guardar em cada destino um assunto ou conjunto em comum. <br />Pacotes seguem regras para escrita do seu nome:<br />-  *deve ser em letras minúsculas e sem caracteres especiais. <br />- não utilize espaços em branco no nome dos pacotes* |
| **Objetos**          | Vimos acima que podemos criar classes com atributos, que esses atributos são propriedades que formam as características de alguma coisa, ou alguém. Vimos também o exemplo do cliente que possuí algumas características dentro de um sistema( nome, e-mail, cpf, data de nascimento). Até aqui ok, mas quando criamos um cliente com características, criamos o que chamamos na orientação a objetos de Objeto, então o objeto Cliente leva com ele todos os seus atributos, ou seja, características. Vale lembrar, que o objeto tem os atributos preenchidos ou não mas todos os atributos estão para o objeto. |

Então ligando tudo que vimos até aqui, podemos entender que:

1. As Classes são escritas como arquivos do nosso código, cada classe deve ser salva em um arquivo. Cada uma vai realizar uma parte do produto final, atendendo o paradigma de desenvolvimento orientação a objetos.
2. A classe também pode ter estruturas responsáveis por carregar as características de um objeto, que são os atributos  e/ou métodos que são responsáveis por realizar as ações.
3. O método responsável por entregar o produto final ao cliente final do sistema, é o método main.
4. Podemos fazer uso de bibliotecas em nosso código, para agilizar, facilitar o nosso desenvolvimento e essas bibliotecas armazenam métodos prontos dentro delas.

### IDE Eclipse For Developers

Para esse documento estarei utilizando a ferramenta **Eclipse Ide For Developers**, você pode utilizar outra ferramenta que de suporte a desenvolvimento Java conforme se sentir mais confortável.

Para utilizar essa ferramenta devemos primeiro definir o ambiente de trabalho, **Workspace**, pode ser uma pasta dentro da área de trabalho ou da pasta Documentos. Vou utilizar uma pasta na área de trabalho para simplificar as explicações nesse documento.

Ao iniciar esta Ide, a primeira coisa que precisamos definir é o workspace. Essa é a tela onde vamos definir esse diretório de trabalho, para isso:

1. clique no botão Browse;
2. escolha o diretório 
3. clique no botão Launch.

![eclipse-tela1-workspace](https://user-images.githubusercontent.com/8031302/195968001-9846141a-f403-4c8c-aae6-4018da7705c8.png)