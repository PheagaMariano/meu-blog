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


      <main>
        <div class="m-5 px-5">
            <div class="mx-5 p-2">
                <div class="mx-5 px-5">
                    <h1>Sobre Mim</h1>
                    <p>Desenvolvido por <a href="http://google.com" target="_blank">Pedro figueiredo</a></p>
                    <p>Olá! Sou um desenvolvedor apaixonado por tecnologia, com um forte foco em programação. Além de adorar criar soluções inovadoras e eficientes, também sou um entusiasta de café e um habilidoso na modelagem 3D. Com experiência em desenvolvimento de software e colaboração em equipes, estou sempre em busca de novos desafios e oportunidades para aprender e aplicar as últimas tecnologias. Estou animado para contribuir com meu conhecimento e habilidades em projetos que buscam excelência e impacto positivo</p>
                </div>
            </div>
        </div>
      </main>
  
</template>
