<script setup lang="ts">
import kaguya3 from '../assets/imgs/kaguya3.png';
import attackontitan from '../assets/imgs/attackontitan.jpg';
import codegeassposter from '../assets/imgs/codegeassposter.jpg';

function activeTag(evt: MouseEvent): void {
    const element = evt.target as HTMLElement;
    if (element.classList.contains("active")) {
        element.classList.remove("active");
        return
    }
    element.classList.add("active");
}
</script>

<template>
    <div class="container p-3">
        <!-- Title -->
        <h1 class="display-3 mb-3">Reviews</h1>

        <!-- Tags -->
        <div class="tags d-flex gap-3 overflow-x-scroll pb-2">
            <h5><span class="badge border rounded-pill bg-primary p-2" @click="activeTag">Adventure</span></h5>
            <h5><span class="badge border rounded-pill bg-success p-2" @click="activeTag">Action</span></h5>
            <h5><span class="badge border rounded-pill bg-pink p-2" @click="activeTag">Drama</span></h5>
            <h5><span class="badge border rounded-pill bg-warning p-2" @click="activeTag">Magic</span></h5>
            <h5><span class="badge border rounded-pill bg-dark p-2" @click="activeTag">Horror</span></h5>
            <h5><span class="badge border rounded-pill bg-someblue p-2" @click="activeTag">Psychological</span></h5>
            <h5><span class="badge border rounded-pill bg-info p-2" @click="activeTag">Sci-Fi</span></h5>
            <h5><span class="badge border rounded-pill bg-danger p-2" @click="activeTag">Romance</span></h5>
        </div>

        <!-- Reviews Grid -->
        <div class="reviews-container row justify-content-center justify-content-lg-start gap-4">
            <!-- Card -->
            <div class="card g-col my-3 mb-3 border-0 shadow-lg p-0">
                <div class="row g-0">
                    <div class="card-image-container col-md-4 col-4">
                        <img :src="kaguya3" class="img-fluid object-fit-cover h-100 rounded-start shadow">
                    </div>
                    <div class="col-md-8 col-8">
                        <div class="card-body">
                            <h5 class="card-title">Kaguya-Sama: Love Is War - Season 3</h5>
                            <p class="card-text">The third season of Kaguya-sama: Love Is War, titled Kaguya-sama: Love Is
                                War –
                                Ultra Romantic, is a 2022 Japanese anime series, based on the manga series of the The third
                                season
                                of Kaguya-sama: Love Is War, titled Kaguya-sama: Love Is War –
                                Ultra Romantic, is a 2022 Japanese anime series, based on the manga series of the</p>
                            <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
                            <div class="d-flex gap-2">
                                <span class="badge active border rounded-pill bg-danger p-2">Romance</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Card -->
            <div class="card g-col my-3 mb-3 border-0 shadow-lg p-0">
                <div class="row g-0">
                    <div class="card-image-container col-md-4 col-4">
                        <img :src="attackontitan" class="img-fluid object-fit-cover h-100 rounded-start">
                    </div>
                    <div class="col-md-8 col-8">
                        <div class="card-body">
                            <h5 class="card-title">Attack on Titan - Season 4</h5>
                            <p class="card-text">TShingeki no Kyojin (進撃の巨人 lit. Titã de Ataque?) também conhecido pelo
                                título
                                em
                                inglês Attack on Titan, é uma série de mangá escrita e ilustrada por Hajime Isayama. É
                                ambientado em
                                um mundo onde a humanidade vive dentro de cidades cercadas por três enormes muralhas que os
                                protegem
                                dos gigantescos humanóides devoradores de humanos chamados de Titãs; a história segue Eren
                                Yeager,
                                que jura exterminar os Titãs após um Titã causar a destruição de sua cidade natal e a morte
                                de
                                sua
                                mãe. Shingeki no Kyojin teve seus capítulos publicados na revista mensal de mangás shōnen
                                Bessatsu
                                Shōnen Magazine da editora Kodansha entre setembro de 2009 a abril de 2021, com os seus
                                capítulos
                                compilados em 34 volumes tankōbon.</p>
                            <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
                            <div class="d-flex gap-2">
                                <span class="badge active border rounded-pill bg-primary p-2">Adventure</span>
                                <span class="badge active border rounded-pill bg-success p-2">Action</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Card -->
            <div class="card g-col my-3 mb-3 border-0 shadow-lg p-0">
                <div class="row g-0">
                    <div class="card-image-container col-md-4 col-4">
                        <img :src="codegeassposter" class="img-fluid object-fit-cover h-100 rounded-start shadow">
                    </div>
                    <div class="col-md-8 col-8">
                        <div class="card-body">
                            <h5 class="card-title">Code Geass: Lelouch of the Rebellion</h5>
                            <p class="card-text">Code Geass: Lelouch of the Rebellion (コードギアス 反逆のルルーシュ Kōdo Giasu: Hangyaku
                                no
                                Rurūshu?) é um anime da franquia Code Geass, de 2006, com 25 episódios, criado pela Sunrise.
                                Dirigida por Gorō Taniguchi e escrita por Ichirō Ōkouchi, ambos tendo anteriormente
                                trabalhado em
                                outra série da Sunrise, chamado Planetes. Code Geass - Lelouch of the Rebellion apresenta
                                character
                                design original da CLAMP.

                                A primeira temporada da série foi apresentada no Japão pela MBS em 6 de outubro de 2006 e
                                foi
                                concluída em 28 de Julho de 2007, após 25 episódios. A segunda temporada e sequência da
                                série, Code
                                Geass: Lelouch of the Rebellion R2 começou a ser apresentada nas redes MBS e TBS em 6 de
                                abril de
                                2008.</p>
                            <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
                        </div>
                    </div>
                </div>
            </div>

        </div>
    </div>
</template>

<style scoped>
::-webkit-scrollbar {
    height: 4px;
}

::-webkit-scrollbar-thumb {
    background-color: #bbb;
    border-radius: 2px;
}

.badge {
    cursor: pointer;
    filter: saturate(0);
    transition: 0.1s ease-in-out filter;
    user-select: none;
}

.badge.active {
    filter: saturate(1);
}

.bg-pink {
    background-color: #de5c9d;
}

.bg-someblue {
    background-color: #6e99b4;
}

.card {
    max-width: 420px;
    overflow: hidden;
}

.card .card-title {
    display: -webkit-box;
    -webkit-line-clamp: 1;
    -webkit-box-orient: vertical;
    overflow: hidden;
    text-overflow: ellipsis;
}

.card p {
    display: -webkit-box;
    -webkit-line-clamp: 6;
    -webkit-box-orient: vertical;
    overflow: hidden;
    text-overflow: ellipsis;
}
</style>