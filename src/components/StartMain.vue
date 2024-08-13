<template>
  <!-- NAVBAR -->


  <nav class="navbar navbar-expand-lg p-3 navbar-light bg-light">
    <div class="container-fluid">
      <a class="navbar-brand " href="#">Navbar</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown"
              aria-expanded="false">
              Dropdown
            </a>
            <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
              <li><a class="dropdown-item" href="#">Action</a></li>
              <li><a class="dropdown-item" href="#">Another action</a></li>
              <li>
                <hr class="dropdown-divider">
              </li>
              <li><a class="dropdown-item" href="#">Something else here</a></li>
            </ul>
          </li>
          <li class="nav-item">
            <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
          </li>
        </ul>
        <form class="d-flex">
          <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-success" type="submit">Search</button>
        </form>
      </div>
    </div>
  </nav>

  <!-- TERMINO NAV BAR -->



  <!-- MAIN -->

  <main>
    <div class="m-5 px-5">
      <div class="mx-5 p-2">
        <div class="mx-5 px-5">
          <h1>Sobre Mim</h1>
          <p>Desenvolvido por <a href="http://google.com" target="_blank">Pedro Figueiredo</a></p>
          <p>Olá! Sou um desenvolvedor apaixonado por tecnologia, com um forte foco em programação. Além de adorar criar
            soluções inovadoras e eficientes, também sou um entusiasta de café e um habilidoso na modelagem 3D. Com
            experiência em desenvolvimento de software e colaboração em equipes, estou sempre em busca de novos desafios
            e oportunidades para aprender e aplicar as últimas tecnologias. Estou animado para contribuir com meu
            conhecimento e habilidades em projetos que buscam excelência e impacto positivo</p>
          <a href="#" class="routerGreen">Saiba Mais
            <i class="bi bi-chevron-right chevron-bold"></i>
          </a>
          <ul id="lista-topicos"></ul>
        </div>
      </div>
    </div>
  </main>

  <ul id="lista-topicos">
    <li class="topico-template" style="display: none;">
      <a href="#">
        <h2>

        </h2>
      </a>
      <div class="img-robo">
        <img src="" width="70%" class="img-fluid" alt="">
      </div>
      <p></p>
      <a href="#" class="routerGreen">Saiba Mais
        <i class="bi bi-chevron-right chevron-bold"></i>
      </a>
    </li>
  </ul>
  

</template>

<script>

document.addEventListener('DOMContentLoaded', function () {
  const listaTopicos = document.getElementById('lista-topicos');
  const topicoTemplate = document.querySelector('.topico-template');

  const topicos = [
    {
      titulo: 'Robo Para Máquina de Injeção',
      imagem: 'https://i.ibb.co/bJYdk7X/Injetora-Site-page-0001.jpg',
      descricao: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Laborum beatae culpa officiis ducimus adipisci tempore facere sequi asperiores saepe? Nihil, doloribus reprehenderit? Dolor animi ullam aliquam unde soluta deleniti nobis.lll',
      link: '#'
    },
    {
      titulo: 'Outro Projeto Inovador',
      imagem: 'https://via.placeholder.com/300',
      descricao: 'Descrição de outro projeto interessante.',
      link: '#'
    },
    // Adicione mais tópicos conforme necessário
  ];

  if (listaTopicos && topicoTemplate) {
    topicos.forEach(topico => {
      const novoTopico = topicoTemplate.cloneNode(true);
      novoTopico.style.display = ''; // Mostra o item

      const titulo = novoTopico.querySelector('h2');
      titulo.textContent = topico.titulo;

      const imagem = novoTopico.querySelector('img');
      imagem.src = topico.imagem;
      imagem.alt = topico.titulo;

      const descricao = novoTopico.querySelector('p');
      descricao.textContent = topico.descricao;

      const link = novoTopico.querySelector('a.routerGreen');
      link.href = topico.link;

      listaTopicos.appendChild(novoTopico);
    });

    // Remove o template original do DOM
    listaTopicos.removeChild(topicoTemplate);
  } else {
    console.error('Elemento #lista-topicos ou .topico-template não encontrado na página.');
  }
});



</script>
