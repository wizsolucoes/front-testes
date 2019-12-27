# Reserva ingressos para pré estreia

Este teste tem por objetivo medir o nível técnico nas seguintes áreas:

+ Organização do projeto
+ Utilização coesa das estruturas Html
+ Clareza de código e organização das classes
+ Nível de conhecimento em **Angular 5+**
+ Conhecimento em testes (não obrigatório, mas será diferencial)
+ Consumo de WebApi's e tratamento de chamadas assíncronas

## Tecnologias a serem utilizadas

+ Angular 5 ou superior
+ Scss ou css
+ Testes (opcional)

## Desafio

O desenvolvedor deverá criar um formulário de reserva de ingressos para os filmes que estão para serem lançados. Respeitando os seguintes critérios:

### Layout

Utilize o links a seguir para montar a estrutura da sua aplicação.
<br><br>
[Tela sem acompanhante](https://app.avocode.com/view/1a45b72eba2a46a28cf9c20a13a35d7a) 
<br>
[Tela com acompanhante](https://app.avocode.com/view/86dd682733d041afbc696cbb9bb0ec62) 

> A parte de valores, não precisa funcionar mas deve ser imlementada (HTML, CSS).

***Requisitos mínimos:***

+ Seguir o layout proposto, fazendo melhorias somente quando cabíveis.
+ Utilização coesa da estrutura Html.
+ Organização da estrutura CSS.
+ Crie um combo (select) com as opções de filme.
+ Modifique o campo de cidade e estado para um campo de texto.

***Diferenciais:***

+ Máscaras nos campos que permitem esse uso.
+ Implementar responsividade.
+ Animações.
+ Utilização de mixers, variables e placeholders (quando cabíveis).

### Código:

Via de regra o código estará sendo julgado por: organização, identação e clareza. Mas a arquitetura de pastas e a divisão de classes fica por conta do desenvolvedor.

***Api correios:***

Após digitar o cep os demais campos deverão ser preenchidos com base no retorno de uma api de consulta de endereço por **cep**:

+ Recomendamos esta: [https://correiosapi.apphb.com/](https://correiosapi.apphb.com/), mas o desenvolvedor poderá utilizar outra de sua preferência.

### Estrutura:

A organização de pastas e de código fica a cargo do desenvolvedor.

### Regras:

+ Todos os campos são obrigatórios
+ Somente um acompanhante é permitido e os campos do acompanhante devem estar ocultos quando a opção **Adicionar acompanhante** não estiver marcada.
+ O botão Enviar somente estará ativo quando todos os campos estiverem válidos.
+ Ao clicar no botão enviar um JSON deverá ser enviado a seguinte url: *http://localhost/reserva*, a chamada deverá ser um **post** e em seu cabeçalho deverá haver um campo **Authorization** com o seguinte hash: *#ASDFGW#ERWQERTRYT#%$%$@#$%==*.

> A chamada ao post irá gerar erro, não há problemas quanto a isso, o que será julgado será a chamada gerada e o código desenvolvido.

### Testes:

Testes são bem vindos, mas testes que não tenham relevância não serão considerados.

## Procedimento para a execução do projeto:

1. Criar um repositório Git aberto.
2. Executar commit's pequenos para que seja visível o fluxo do desenvolvimento.
3. Criar um README.md com os procedimentos para a execução, teste e publicação do seu projeto.
4. Ao finalizar, enviar um e-mail com o link do seu projeto.
