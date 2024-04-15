# Lucas C. Alecrim - Portfólio
### Este é o repositório do meu portfólio online, onde compartilho informações sobre minha carreira, habilidades e projetos.

### Conteúdo
HTML: O arquivo index.html contém a estrutura principal do meu site, incluindo a navegação, seções sobre mim, minhas habilidades, projetos destacados, empresas onde trabalhei e informações de contato.

CSS: O arquivo styles.css contém estilos personalizados para o meu site, incluindo formatação, layout e responsividade.

# JavaScript: O arquivo index.js contém scripts para interatividade na página, como a funcionalidade do menu hamburguer e a mudança de estilo da barra de navegação ao rolar a página.

### JavaScript (index.js)
## Seleção de Elementos: O JavaScript começa selecionando os elementos HTML relevantes, como a barra de navegação (navbar), o menu "hamburguer (button)" e a versão móvel da navegação (mobileNavbar)
### (A funcionalidade do "menu hamburguer" refere-se ao ícone de menu que geralmente é exibido em dispositivos móveis para ocultar e exibir o menu de navegação. Quando clicado, ele abre ou fecha o menu de navegação, proporcionando uma experiência de navegação otimizada para telas menores)

const navbar = document.querySelector('.navbar'); 

const mobileNavbar = document.querySelector('.navbar__mobile');

const button = document.querySelector('.burguer');

button.addEventListener('click', function () {
  mobileNavbar.classList.toggle('active');
});

window.addEventListener('scroll', function () {
  if (this.window.pageYOffset > 0) return navbar.classList.add('active');
  return navbar.classList.remove('active');
});

### Evento de Cliques: Adiciona um ouvinte de eventos para o clique no botão hamburguer, que alterna a classe active na versão móvel da navegação para mostrar ou ocultar o menu.

### Evento de Rolagem: Adiciona um ouvinte de eventos para o rolamento da página, que adiciona a classe active à barra de navegação quando o usuário rola para baixo na página, e remove essa classe quando o usuário retorna ao topo.
