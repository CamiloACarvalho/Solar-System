# Boas-vindas ao repositório do projeto Solar System!

Para realizar o projeto, atente a cada passo descrito a seguir e, se tiver qualquer dúvida, nos envie por Slack! #vqv 🚀

Aqui você vai encontrar os detalhes de como estruturar o desenvolvimento de seu projeto com base neste repositório utilizando uma branch específica e um Pull Request para colocar seus códigos.

# Termos e acordos

Ao iniciar este projeto, você concorda com as diretrizes do Código de Conduta e do Manual da Pessoa Estudante da Trybe.

<details>
  <summary><strong>👨‍💻 O que deverá ser desenvolvido</strong></summary><br />

  Neste projeto, você desenvolverá um modelo do Sistema Solar! Ao utilizar essa aplicação, uma pessoa usuária deverá ser capaz de:

    * Visualizar todos os planetas do Sistema Solar renderizados na tela.

    * Visualizar todas as cartas com informações sobre missões espaciais.

</details>

<details>
  <summary><strong>:memo: Habilidades</strong></summary><br />

  Neste projeto, verificaremos se você é capaz de:

  * Utilizar JSX no React.

  * Utilizar corretamente o método `render()` para renderizar seus componentes.

  * Utilizar `import` para trazer componentes em diferentes arquivos.

  * Criar componentes de classe em React.

  * Criar múltiplos componentes a partir de um array.

  * Fazer uso de `props` corretamente.

  * Fazer uso de `PropTypes` para validar as `props de um componente`.
</details>

<details>
  <summary><strong>🗂 Compartilhe seu portfólio!</strong></summary><br />

  Você sabia que o LinkedIn é a principal rede social profissional e compartilhar seu aprendizado nela é muito importante caso deseje construir uma carreira de sucesso? Compartilhe esse projeto em seu LinkedIn, marque o perfil da Trybe (@trybe) e mostre à sua rede toda a sua evolução.

</details>

# Requisitos

:warning: **PULL REQUESTS COM ISSUES DE LINTER NÃO SERÃO AVALIADAS.** :warning:

:warning: **As imagens são meramente ilustrativas para visualizar o fluxo da aplicação, portanto os nomes devem seguir os requisitos, e não as imagens.** :warning:

## 1. Crie um componente chamado `Header`

<details>
  <summary>Crie um componente chamado <code>Header</code> dentro da pasta <code>src/components</code>. Esse componente vai renderizar o título principal da página.</summary>

  - Ele deve conter uma tag `header` e, dentro dela, uma tag `h1`. O texto da tag `h1` deve ser "Sistema Solar".
    
  - Renderize o componente `Header` dentro do componente principal `App`.

  ![Screenshot](/examples/req1.png)
</details>

<details>
  <summary><strong>O que será verificado</strong></summary><br />

  * Se o componente `<Header />` é renderizado.

  * Se o componente `<Header />` contém uma tag `header`.

  * Se o componente `<Header />` contém uma tag `h1`.

  * Se o componente `<Header />` renderiza corretamente o texto "Sistema Solar".

  * Se o componente `<Header />` está sendo renderizado no componente principal `App`.
</details>

---

## 2. Crie um componente chamado `SolarSystem`

<details>
  <summary>Crie um componente chamado <code>SolarSystem</code> dentro da pasta <code>src/components</code>.</summary>

  - O componente `SolarSystem` deve ter uma `div` que envolva todo seu conteúdo e que tenha o atributo `data-testid="solar-system"`.

  - Renderize o componente `SolarSystem` abaixo do `Header`, dentro do componente principal `App`.
</details>

<details>
  <summary><strong>O que será verificado</strong></summary><br />

  * Se o componente `<SolarSystem />` é renderizado.

  * Se há uma `div` que tem o `data-testid="solar-system"`.

  * Se o componente `<SolarSystem />` está sendo renderizado no componente principal `App`.
</details>

---

## 3. Crie um componente chamado `Title`

<details>
  <summary>Crie um componente chamado <code>Title</code> dentro da pasta <code>src/components</code>.</summary>

  - O componente `Title` deve receber uma prop `headline`.
    
  - Ele deve conter uma tag `h2`, que deve renderizar o texto recebido pela prop `headline`.
</details>

<details>
  <summary><strong>O que será verificado</strong></summary><br />

  * Se o componente `<Title />` é renderizado.

  * Se o componente `<Title />` contém uma tag `h2`.

  * Se o componente `<Title />` renderiza o texto passado pela prop `headline` dentro de uma tag `h2`.
</details>

---

## 4. Renderize o componente `Title` dentro do componente `SolarSystem`

<details>
  <summary>Renderize o componente <code>Title</code> dentro do componente <code>SolarSystem</code>.</summary>

  - O componente `Title` deve ser renderizado recebendo a prop `headline` com o valor "Planetas".

  ![Screenshot](/examples/req4.png)
</details>

<details>
  <summary><strong>O que será verificado</strong></summary><br />

  * Será validado se o texto "Planetas" é renderizado usando o componente `Title` dentro do componente `SolarSystem`.
</details>

---

## 5. Crie um componente chamado `PlanetCard`
<details>
  <summary>Crie um componente chamado <code>PlanetCard</code> dentro da pasta <code>src/components</code>.</summary>

  - O componente `PlanetCard` deve receber duas props: uma chamada `planetName` e outra, `planetImage`.
    
  - O componente `PlanetCard` deve ter uma `div` que envolva todo seu conteúdo e que tenha o atributo `data-testid="planet-card"`.
    
  - O componente `PlanetCard` deve renderizar o texto recebido pela prop `planetName`. Sugerimos a utilização de tags de [Conteúdo de Fluxo](https://developer.mozilla.org/pt-BR/docs/Web/Guide/HTML/Content_categories#conte%C3%BAdo_de_fluxo), como `<p>`, que deve conter o atributo `data-testid="planet-name"`.
    
  - O componente `PlanetCard` deve renderizar uma imagem que tenha o atributo `src` com o valor recebido pela prop `planetImage`.

  - Além do atributo `src`, a imagem renderizada deve ter o atributo `alt` com o texto `Planeta {planetName}`, em que `{planetName}` é o valor recebido pela prop `planetName`.
</details>

<details>
  <summary><strong>O que será verificado</strong></summary><br />

  * Se o componente `<PlanetCard />` é renderizado.

  * Se o componente `<PlanetCard />` tem uma div com o atributo `data-testid="planet-card"`.

  * Se é renderizado o texto recebido pela prop `planetName`.

  * Se é renderizada uma imagem com o atributo `src` com o mesmo valor recebido pela prop `planetImage`.

  * Se, além do atributo `src`, a imagem renderizada tem o atributo `alt` com o texto `Planeta {planetName}`, em que `{planetName}` é o valor recebido pela prop `planetName`.
</details>

---

## 6. Renderize uma lista com os planetas do Sistema Solar

<details>
  <summary>Renderize uma lista com os planetas do Sistema Solar dentro do componente <code>SolarSystem</code>.</summary>

  - Utilize o componente `PlanetCard` para renderizar cada item da lista de planetas.

  - Você encontrará a lista com os nomes e as imagens de cada planeta do Sistema Solar no arquivo `src/data/planets.js`.
    
  - Você deve importar a lista no componente `SolarSystem` usando o código:
  ```javascript
  import planets from '../data/planets';
  ```

  - A lista de planetas é um _array_ de objetos no seguinte formato:
  ```javascript
  {
    name: "Nome do planeta",
    image: "caminho-para-imagem-do-planeta"
  }
  ```

  - Para cada planeta da lista, você deverá renderizar um componente `PlanetCard`, passando o atributo `name` para a prop `planetName` e o atributo `image` para a prop `planetImage`.

  ![Screenshot](/examples/req6.png)
</details>

<details>
  <summary>:bulb: Dica: </summary> 

  - Lembre-se do método que permite a você criar vários componentes iguais com base em valores presentes em um _array_. Lembre-se também de que, ao renderizar uma lista, você deve passar o atributo `key` para cada item. Ainda, você pode usar o nome do planeta como `key`.
</details>

<details>
  <summary><strong>O que será verificado</strong></summary><br />

  * Se é renderizado um componente `<PlanetCard />` para cada planeta da lista de planetas.

  * Se todos os planetas do Sistema Solar estão sendo listados na tela.
</details>

---

# Requisitos Bônus

## 7. Crie um componente chamado `Missions`

<details>
  <summary>Crie um componente chamado <code>Missions</code> dentro da pasta <code>src/components</code>.</summary>

  - Esse componente deve ter uma `div` que envolva todo seu conteúdo e que tenha o atributo `data-testid="missions"`.

  - Renderize o componente `Missions` abaixo do `SolarSystem`, dentro do componente principal `App`.
</details>

<details>
<summary><strong>O que será verificado</strong></summary><br />

  * Se o componente `<Missions />` é renderizado.

  * Se há uma `div` que tem o `data-testid="missions"`.

  * Se o componente `<Missions />` está sendo renderizado no componente principal `App`.
</details>

---

## 8. Renderize o componente `Title` dentro do componente `Missions`

<details>
  <summary>Renderize o componente <code>Title</code> dentro do componente <code>Missions</code>.</summary>

  - O componente `Title` deve ser renderizado recebendo a prop `headline` com o valor "Missões".

  ![Screenshot](/examples/req8.png)
</details>
<details>
<summary><strong>O que será verificado</strong></summary><br />

  * Será validado se o texto "Missões" é renderizado usando o componente `Title` dentro do componente `Missions`.
</details>

---

## 9. Crie um componente chamado `MissionCard`

<details>
  <summary>Crie um componente chamado <code>MissionCard</code> dentro da pasta <code>src/components</code>.</summary>

  - O componente `MissionCard` deve receber quatro props:
    - `name`
    - `year`
    - `country`
    - `destination`

  - O componente `MissionCard` deve ter uma `div` que envolva todo seu conteúdo e que tenha o atributo `data-testid="mission-card"`.
  
  - O componente `MissionCard` deve renderizar o texto recebido pela prop `name`. Sugerimos a utilização de tags de [Conteúdo de Fluxo](https://developer.mozilla.org/pt-BR/docs/Web/Guide/HTML/Content_categories#conte%C3%BAdo_de_fluxo), como `<p>`, que deve conter o atributo `data-testid="mission-name"`.
  
  - O componente `MissionCard` deve renderizar o texto recebido pela prop `year`. Sugerimos a utilização de tags de [Conteúdo de Fluxo](https://developer.mozilla.org/pt-BR/docs/Web/Guide/HTML/Content_categories#conte%C3%BAdo_de_fluxo), como `<p>`, que deve conter o atributo `data-testid="mission-year"`.
  
  - O componente `MissionCard` deve renderizar o texto recebido pela prop `country`. Sugerimos a utilização de tags de [Conteúdo de Fluxo](https://developer.mozilla.org/pt-BR/docs/Web/Guide/HTML/Content_categories#conte%C3%BAdo_de_fluxo), como `<p>`, que deve conter o atributo `data-testid="mission-country"`.
  
  - O componente `MissionCard` deve renderizar o texto recebido pela prop `destination`. Sugerimos a utilização de tags de [Conteúdo de Fluxo](https://developer.mozilla.org/pt-BR/docs/Web/Guide/HTML/Content_categories#conte%C3%BAdo_de_fluxo), como `<p>`, que deve conter o atributo `data-testid="mission-destination"`.
</details>

<details>
  <summary><strong>O que será verificado</strong></summary><br />

  * Se o componente `<MissionCard />` é renderizado.

  * Se o componente `<MissionCard />` tem uma div com o atributo `data-testid="mission-card"`.

  * Se é renderizado o texto recebido pela prop `name`.

  * Se é renderizado o texto recebido pela prop `year`.

  * Se é renderizado o texto recebido pela prop `country`.

  * Se é renderizado o texto recebido pela prop `destination`. 
</details>

---

## 10. Renderize uma lista com as missões espaciais

<details>
  <summary>Renderize uma lista com as missões espaciais dentro do componente <code>Missions</code>.</summary>

  - Utilize o componente `MissionCard` para renderizar cada item da lista de missões.

  - Você encontrará a lista com as informações de cada missão espacial no arquivo `src/data/missions.js`.

  - Você deve importar a lista no componente `Missions` usando o código:
  ```javascript
  import missions from '../data/missions';
  ```

  - A lista de missões espaciais é um _array_ de objetos no seguinte formato:
  ```javascript
  {
    name: 'Nome da missão',
    year: 'Ano de lançamento da missão',
    country: 'País que lançou a missão',
    destination: 'Destino da missão',
  }
  ```

  - Para cada missão espacial da lista, você deverá renderizar um componente `MissionCard`, passando cada atributo para a respectiva prop.

  <img src="/examples/req10.png" alt="Screenshot" width=528 />

</details>
<details>
<summary>:bulb: Dica:</summary>

  - Lembre-se do método que permite a você criar vários componentes iguais com base em valores presentes em um _array_. Lembre-se também de que, ao renderizar uma lista, você deve passar o atributo `key` para cada item. Ainda, você pode usar o nome da missão como `key`.
</details>

<details>
  <summary><strong>O que será verificado</strong></summary><br />

  * Se é renderizado um componente `<MissionCard />` para cada missão espacial da lista de missões.

  * Se todas as missões espaciais estão sendo listadas na tela.
</details>

---
