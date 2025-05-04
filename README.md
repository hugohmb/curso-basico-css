# CSS na Prática: Estrutura, Estilização e Interação

Este repositório documenta a prática de conceitos fundamentais de CSS aplicados em um projeto de interface web com foco em estruturação visual, estilização responsiva e interações dinâmicas. O HTML foi utilizado como suporte estrutural para a aplicação dos estilos, sem aprofundamento nas boas práticas ou semântica da linguagem.

# Objetivo do Projeto

Aplicar conhecimentos de CSS em:

- Estilização visual de elementos

- Layouts responsivos com inline-block

- Manipulação de estilos via pseudo-classes como :hover

- Transições visuais com transition

- Ocultação e revelação de elementos com display

- Substituição de conteúdo e imagem via hover



# Conceitos CSS Estudados e Aplicados

1. Estruturação Visual

- Utilização de div com class="card" para criar blocos independentes

- Cada bloco possui imagem e texto visível por padrão e conteúdo oculto (texto alternativo e nova imagem)


2. Layout com inline-block

- Organização horizontal dos cards

- Controle de espaçamento entre eles com margin e padding


3. Ocultação e revelação de elementos

```css
   .texto-oculto {
  display: none;
}

.card:hover .card-text {
  display: none;
}

.card:hover .texto-oculto {
  display: block;
}
```

- Garante troca de conteúdo ao passar o mouse



4. Substituição de imagem via seletor direto

```css
.card > img {
  display: block;
}

.card:hover > img {
  display: none;
}
```

- A imagem original está solta diretamente na div.card, então foi usada a seletividade direta com > para ocultá-la no hover, sem afetar imagens internas da div.texto-oculto



5. Centralização de imagem substituta

```css
.texto-oculto img {
  display: block;
  margin: 0 auto;
}
```

- A nova imagem que aparece no hover foi centralizada horizontalmente via margin: 0 auto



6. Transição suave

```css
.card {
  transition: background 0.3s ease;
}
```

- Cria uma mudança de cor suave ao passar o mouse, melhorando a experiência do usuário


7. Mudança de cor no hover

```
.card:hover {
  background: #FF2978;
  color: white;
}
```

- Aplica estilo interativo que realça o bloco ao receber foco do mouse



# Aplicação Final

A seção desenvolvida representa uma área de "Serviços" com três cards, cada um contendo:

- Uma imagem principal

- Um título e parágrafo descritivo

- E, ao interagir com hover, uma nova imagem e texto substituem os anteriores

Esse comportamento simula uma interação de destaque ou "explicação estendida" para serviços ou funções em um site institucional ou portfólio.


# Habilidades Desenvolvidas

- Domínio de seletores CSS

- Compreensão da hierarquia de seletores e especificidade

- Controle de visibilidade com display

- Uso de pseudo-classes como :hover

- Estilização de interação visual

- Manipulação de espaçamento e alinhamento de elementos


# Considerações Finais

Este projeto teve como finalidade consolidar a compreensão de CSS através de prática aplicada em situações comuns de interface, com foco em estilização e interações visuais responsivas. Embora HTML tenha sido utilizado, o foco foi inteiramente na estilização CSS.
   
