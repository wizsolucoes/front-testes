# Reserva ingressos para pré estreia

Este teste tem por objetivo medir o nível técnico nas seguintes áreas:

+ Organização do projeto
+ Utilização coesa das estruturas Html
+ Uso de CSS/SCSS
+ Uso de Typescript
+ Clareza e organização de código
+ Nível de conhecimento em **Angular**
+ Consumo de WebApi's e tratamento de chamadas assíncronas
+ Conhecimento em testes (não obrigatório, mas será um diferencial)

## Tecnologias a serem utilizadas

+ A versão mais recente de Angular
+ Scss ou css

## Desafio

O desenvolvedor deverá criar um formulário de reserva de ingressos para os filmes que estão para serem lançados. Respeitando os seguintes critérios:

### Layout

Utilize o links a seguir para montar a estrutura da sua aplicação.
<br><br>
[Tela sem acompanhante](https://app.avocode.com/view/1a45b72eba2a46a28cf9c20a13a35d7a) 
<br>
[Tela com acompanhante](https://app.avocode.com/view/86dd682733d041afbc696cbb9bb0ec62) 

> Obs:<br>
> + O campo de cidade pode ser textual.<br>
> + A área de valores não precisar ser dinâmica, mas deve ser incluída na implementação do layout.

### APIs obrigatórias:

#### The Movie Database API

Para preencher o campo de filmes será obrigatório o uso da api [https://www.themoviedb.org/](https://www.themoviedb.org/).

+ Utilize o endpoint de upcoming: [https://developers.themoviedb.org/3/movies/get-upcoming](https://developers.themoviedb.org/3/movies/get-upcoming)
+ Você precisará se cadastrar para conseguir uma chave de acesso.
+ Somente será necessário exibir a página 1 dos resultados na lista.

##### Sobre a chave de acesso
Na sua implementação a chave de acesso deve ficar em um arqvuivo chamado `moviedb-config.ts`, **mas este arquivo não deve ser versionado no git**. Para sua entrega crie um arquivo chamado `moviedb-config-sample.ts` que deve ser versionado com o mesmo formato mas **sem a chave de acesso real**.

Exemplo:
```ts
// moviedb-config.ts NÂO DEVE ser versionado
export const movieDbConfig = {
  api_key: "ec5e799n384n48e8dnen48r8585rnff8",
};
```

```ts
// moviedb-config-sample.ts DEVE ser versionado
export const movieDbConfig = {
  api_key: "INSIRA-SUA-CHAVE-AQUI",
};
```

O clonar seu repositório vamos renomear o arquivo de `moviedb-config-sample.ts` para `moviedb-config.ts` para rodar a aplciação.

### API de consulta de CEP

Após digitar o cep os demais campos deverão ser preenchidos com base no retorno de uma api de consulta de endereço por **cep**:

+ Recomendamos a [ViaCEP](https://viacep.com.br/), mas o desenvolvedor poderá utilizar outra de sua preferência.

**Lembre-se que ela deve funcionar abertamente, sem restrições de rede ou hospedagem.**


### Componentização:

Seu projeto deve conter ao menos um componente a ser utilizado no formulário como uma tag, exemplo: 
```html
<address-form></address-form>
```

### Regras:

+ Todos os campos são obrigatórios
+ Somente um acompanhante é permitido e os campos somente aparecem quando o checkbox **Adicionar acompanhante** estiver marcado.
+ Caso o checkbox **Adicionar acompanhante** esteja marcado, os campos do acompanhante também serão obrigatórios.
+ O botão Enviar somente estará ativo quando todos os campos estiverem válidos.
+ Ao clicar no botão enviar um JSON deverá ser enviado a seguinte url: *http://localhost/reserva*, a chamada deverá ser um **post** e em seu cabeçalho deverá haver um campo **Authorization** com o seguinte hash: *#ASDFGW#ERWQERTRYT#%$%$@#$%==*.

> A chamada `post` irá gerar erro, não há problemas quanto a isso, o que será julgado será a chamada gerada e o código desenvolvido.

### Diferenciais:

+ [Seguir a estrutura de aplicação recomendada pela equipe Angular](https://angular.io/guide/styleguide#application-structure-and-ngmodules)
+ [Lazy-loading de módulos de feature](https://angular.io/guide/lazy-loading-ngmodules)
+ Máscaras nos campos que permitem esse uso
+ Implementar responsividade
+ Animações
+ Testes unitários
+ README.md sugerir melhorias de usabilidade e acessibilidade caso as encontre

## Procedimento para a execução do projeto:

1. Criar um repositório Git aberto.
2. Criar um README.md com os procedimentos para a execução, teste e publicação do seu projeto.
3. Ao finalizar, enviar um e-mail com o link do seu projeto.
