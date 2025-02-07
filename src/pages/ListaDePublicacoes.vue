<template>
  <!-- Banner -->
  <section class="section-banner row justify-center">
    <div class="custom-spacing-border">
      <q-breadcrumbs gutter="md" class="banner-breadcrumbs q-pb-lg text-grey-6">
        <q-breadcrumbs-el class="text-green-5" label="Início" icon="chevron_left" />
        <q-breadcrumbs-el class="text-grey-6" label="Blog" />
      </q-breadcrumbs>
      <div class="banner bg-green-4 row justify-center items-center">
        <p class="no-margin">Espaço Banner</p>
      </div>
    </div>
  </section>
  <!-- Categorias -->
  <section class="categorias row justify-center">
    <div class="categorias-container custom-spacing-border row">
      <!-- aside -->
      <aside>
        <h6 class="mobile-out text-grey-1 text-weight-bold">Categorias</h6>
        <q-input dense class="search-bar q-my-md" outlined v-model="text" placeholder="Pesquisar">
          <template v-slot:prepend>
            <q-icon name="search" />
          </template>
        </q-input>
        <div class="categorias-select column">
          <div class="categoria row bg-green-6">
            <div class="marcador bg-primary"></div>
            <p class="no-margin text-primary text-weight-medium q-pl-sm">Categoria X</p>
          </div>
          <div class="categoria row">
            <div class="marcador"></div>
            <p class="no-margin text-grey-5 text-weight-medium q-pl-sm">Categoria P</p>
          </div>
          <div class="categoria row">
            <div class="marcador"></div>
            <p class="no-margin text-grey-5 text-weight-medium q-pl-sm">Categoria T</p>
          </div>
          <div class="categoria row">
            <div class="marcador"></div>
            <p class="no-margin text-grey-5 text-weight-medium q-pl-sm">Categoria O</p>
          </div>
        </div>
      </aside>
      <!-- conteúdo -->
      <div class="categoria-content">
        <h6 class="mobile-weight-change text-primary text-weight-bold q-pb-md">Categoria X</h6>
        <div class="card-post row q-mb-lg">
          <div class="img-post">
            <q-img src="../assets/card-1.jpg" />
          </div>
          <div class="card-content column justify-between">
            <p class="no-margin text-primary text-weight-medium mobile-out">Categoria</p>
            <div>
              <h6 class="text-weight-bold">Desenvolvimento Comunitário</h6>
              <p class="card-assunto no-margin text-grey-5">
                Novos Projetos Comunitários: Informações sobre novos projetos e iniciativas que
                estão sendo lançados para melhorar as condições de vida.
              </p>
            </div>
            <p class="ler-mais mobile-weight-change no-margin text-primary">Ler mais</p>
          </div>
        </div>
        <div class="card-post row q-mb-lg">
          <div class="img-post">
            <q-img src="../assets/card-2.jpg" />
          </div>
          <div class="card-content column justify-between">
            <p class="no-margin text-primary text-weight-medium mobile-out">Categoria</p>
            <div>
              <h6 class="text-weight-bold">10 lições sobre Educação e Capacitação!</h6>
              <p class="card-assunto no-margin text-grey-5">
                Perfis de alunos e suas conquistas, mostrando o impacto dos programas educacionais.
              </p>
            </div>
            <p class="ler-mais mobile-weight-change no-margin text-primary">Ler mais</p>
          </div>
        </div>
        <div class="card-post row q-mb-lg">
          <div class="img-post">
            <q-img src="../assets/card-3.jpg" />
          </div>
          <div class="card-content column justify-between">
            <p class="no-margin text-primary text-weight-medium mobile-out">Categoria</p>
            <div>
              <h6 class="text-weight-bold">Saúde e Bem-Estar: Por onde começar?</h6>
              <p class="card-assunto no-margin text-grey-5">
                Notícias sobre campanhas de vacinação, cuidados de saúde e programas de nutrição.
              </p>
            </div>
            <p class="ler-mais mobile-weight-change no-margin text-primary">Ler mais</p>
          </div>
        </div>
        <div class="card-post row q-mb-lg">
          <div class="img-post">
            <q-img src="../assets/card-4.jpg" />
          </div>
          <div class="card-content column justify-between">
            <p class="no-margin text-primary text-weight-medium mobile-out">Categoria</p>
            <div>
              <h6 class="text-weight-bold">
                Treinamento e Desenvolvimento: Emergências e Respostas
              </h6>
              <p class="card-assunto no-margin text-grey-5">
                Informações sobre como a ONG está ajudando em situações de emergência, como
                desastres naturais ou crises humanitária.
              </p>
            </div>
            <p class="ler-mais mobile-weight-change no-margin text-primary">Ler mais</p>
          </div>
        </div>
        <div class="card-post row q-mb-lg">
          <div class="img-post">
            <q-img src="../assets/card-5.jpg" />
          </div>
          <div class="card-content column justify-between">
            <p class="no-margin text-primary text-weight-medium mobile-out">Categoria</p>
            <div>
              <h6 class="text-weight-bold">Campanhas de Ajuda: Como você pode ajudar?</h6>
              <p class="card-assunto no-margin text-grey-5">
                Apelos e campanhas para arrecadação de fundos e doações em resposta a emergências.
              </p>
            </div>
            <p class="ler-mais mobile-weight-change no-margin text-primary">Ler mais</p>
          </div>
        </div>
        <div class="card-post row q-mb-lg">
          <div class="img-post">
            <q-img src="../assets/card-6.jpg" />
          </div>
          <div class="card-content column justify-between">
            <p class="no-margin text-primary text-weight-medium mobile-out">Categoria</p>
            <div>
              <h6 class="text-weight-bold">
                Voluntariado e Envolvimento - Saiba mais sobre o movimento
              </h6>
              <p class="card-assunto no-margin text-grey-5">
                Notícias sobre novas oportunidades para voluntários e eventos de recrutamento.
              </p>
            </div>
            <p class="ler-mais mobile-weight-change no-margin text-primary">Ler mais</p>
          </div>
        </div>
        <div class="card-post row q-mb-lg">
          <div class="img-post">
            <q-img src="../assets/card-7.jpg" />
          </div>
          <div class="card-content column justify-between">
            <p class="no-margin text-primary text-weight-medium mobile-out">Categoria</p>
            <div>
              <h6 class="text-weight-bold">
                Alimentação e psicológico: o que é, exemplos e limitações
              </h6>
              <p class="card-assunto no-margin text-grey-5">
                Lorem Ipsum is simply dummy text of the printing and typesetting industry.
              </p>
            </div>
            <p class="ler-mais mobile-weight-change no-margin text-primary">Ler mais</p>
          </div>
        </div>
        <div class="page-selector mobile-out row justify-end q-mb-xl">
          <div class="selectors row items-center">
            <q-icon name="chevron_left" color="grey-1" size="20px" />
            <div class="selector-num bg-primary text-white">1</div>
            <div class="selector-num text-grey-1">2</div>
            <div class="selector-num text-grey-1">3</div>
            <div class="selector-num text-grey-1">4</div>
            <q-icon name="chevron_right" color="grey-1" size="20px" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
//
</script>
