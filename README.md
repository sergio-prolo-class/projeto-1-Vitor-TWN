# SiteFront
site FrontEnd I

 ## HTML (index.html)
O arquivo index.html é responsável por estruturar a sua página pessoal de forma semântica e organizada. Logo na primeira linha, o documento declara <!DOCTYPE html>, indicando que se trata de um arquivo HTML5. Na linha seguinte, a tag <html lang="pt-br"> define o idioma da página como português do Brasil, garantindo melhor acessibilidade e otimização para motores de busca.

Nas linhas 3 e 4, temos as meta tags <meta charset="UTF-8"> e <meta name="viewport" content="width=device-width, initial-scale=1.0">. A primeira define a codificação de caracteres como UTF-8, evitando problemas com acentuação, enquanto a segunda garante que a página seja responsiva, adaptando-se a diferentes tamanhos de tela (mobile e desktop).

A estilização externa é aplicada por meio da tag <link rel="stylesheet" href="style.css"> na linha 5, que importa o arquivo CSS.

A estrutura da página começa com o <header> (linha 8), onde está presente o título com seu nome, "Vitor Nascimento". Logo depois, na linha 11, a tag <nav> cria um menu de navegação com links para outras seções da página e páginas adicionais, como Perfil Profissional, Seção Acadêmica e Seção Pessoal.

O conteúdo principal está dentro da tag <main> (linha 16), utilizando uma <div id="container-textmain"> para organizar o texto "Sobre mim" e a imagem pessoal. A imagem é adicionada com a tag <img> (linha 22), que inclui um atributo alt para melhorar a acessibilidade e descrever a imagem. IDs e classes (id="paragrafo_main", class="mainfoto") são usados para facilitar a estilização via CSS.

O rodapé da página é construído com <footer> (linha 25), onde você inclui seu nome, links para redes sociais (Instagram e LinkedIn) e um link para retornar ao início da página usando a âncora <a id="voltar" href="#">Voltar ao inicio</a>. Links externos possuem target="_blank" para abrir em uma nova aba, melhorando a experiência de navegação.

## CSS (style.css)
O arquivo style.css define o design visual da página e melhora a experiência do usuário. Logo no início (linha 1), @charset "UTF-8"; garante a compatibilidade de caracteres.

Nas linhas 3 e 4, o seletor universal * é usado para remover margens e paddings padrão dos navegadores, permitindo maior controle sobre a estilização. A seguir, nas linhas 6 a 9, a regra @font-face importa a fonte personalizada "Bacalisties", que é usada para estilizar o cabeçalho.

O corpo da página (body, linha 13) utiliza Flexbox (display: flex; flex-direction: column;) para organizar o layout em coluna, garantindo que o rodapé fique sempre na parte inferior da página (min-height: 100vh). Também foram definidas cores de fundo e texto para manter a leitura confortável.

O <header> recebe uma imagem de fundo nas linhas 17 a 20 usando background-image, com propriedades background-size: cover e background-position: center para ajustar a visualização em diferentes telas. A personalização de texto inclui text-shadow (linha 24), que adiciona sombra ao nome para destacá-lo no cabeçalho.

O menu de navegação (nav, linha 26) está posicionado de forma fixa no topo da página com position: fixed, garantindo que os links estejam sempre visíveis durante a rolagem. Os links dentro do nav são estilizados com uma transição suave (transition-duration: 0.2s) e efeito :hover (linha 41), que muda a cor de fundo e texto ao passar o mouse, melhorando a interatividade.

O container principal (#container-textmain, linha 68) utiliza Grid Layout para organizar o conteúdo interno, com limites de largura (max-width e min-width) para garantir responsividade. Ele também aplica bordas arredondadas (border-radius) e muda de cor quando o usuário passa o mouse sobre ele, utilizando a pseudoclasse :hover para alterar o plano de fundo e cor do texto.

Imagens são centralizadas usando display: flex e justify-content: center (linha 67) e estilizadas com border-radius: 50% (linha 90) para criar um formato circular.

O rodapé (footer, linha 95) possui cores contrastantes, centralização de texto e ícones de redes sociais alinhados com espaçamento adequado. O botão de voltar ao início (#voltar, linha 104) também tem transições para suavizar a mudança de cor ao passar o mouse.

Outras seções, como Perfil Profissional, Seção Acadêmica e Seção Pessoal, seguem a mesma lógica de estrutura com display: grid para organização e ajustes de responsividade com max-width e margens automáticas, garantindo uma experiência consistente em todo o site.