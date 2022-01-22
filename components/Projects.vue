<template>
  <section id="projects">
    <div class="container">
      <h2 class="title">Featured Projects</h2>

      <ul class="project">
        <li v-for="project in projects" :key="project.id" class="project__item">
          <img class="project__thumb" :src="project.thumb" alt="teste" />
          <h3 class="project__title">
            {{ project.title }}
            <a
              class="project__link"
              :href="project.link"
              target="_blank"
              title="Go to project"
              ><i class="icon-link"></i
            ></a>
          </h3>
          <span class="project__category">{{ project.category }}</span>
          <p class="project__description">{{ project.description }}</p>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          id: 1,
          title: 'Acervo',
          description:
            'UI Design and Front-end developed at the WEBi Agency for this.',
          category: 'HTML, CSS, Javascript, WordPress',
          thumb: '/projects/acervo.jpg',
          link: 'http://acervonet.com.br',
        },
        {
          id: 2,
          title: 'Instituto Bettina Moritz',
          description:
            'UI Design and Front-end developed at the WEBi Agency for this client.',
          category: 'HTML, CSS, Javascript, Wordpress',
          thumb: '/projects/bettina.jpg',
          link: 'http://bettinamoritz.com.br',
        },
        {
          id: 3,
          title: 'Escola Guga Kuerten',
          description:
            'UI Design and Front-end developed at the WEBi Agency for this client.',
          category: 'HTML, CSS, Javascript, Wordpress',
          thumb: '/projects/escolaguga.jpg',
          link: 'http://escolaguga.com.br',
        },
        {
          id: 4,
          title: 'Kauffer Pilates',
          description:
            'UI Design and Front-end developed at the WEBi Agency for this client.',
          category: 'HTML, CSS, Javascript, Wordpress',
          thumb: '/projects/kauffer.jpg',
          link: 'http://kaufferpilates.com.br',
        },
        {
          id: 5,
          title: 'Qualyvist',
          description:
            'UI Design and Front-end developed at the WEBi Agency for this client.',
          category: 'HTML, CSS, Javascript, Wordpress',
          thumb: '/projects/qualyvist.jpg',
          link: 'http://qualyvist.com.br',
        },
        {
          id: 6,
          title: 'Solare Imóveis',
          description:
            'UI Design and Front-end developed at the WEBi Agency for this client.',
          category: 'HTML, CSS, Javascript, Wordpress',
          thumb: '/projects/solare.jpg',
          link: 'http://solareimoveis.com.br',
        },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
#projects {
  background-color: $color-bg-alt;
}

.project {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  list-style: none;

  @media (min-width: 768px) {
    flex-direction: row;
    flex-wrap: wrap;
  }

  &__item {
    display: flex;
    flex-direction: column;
    gap: 0.75rem;

    @media (min-width: 768px) {
      width: calc(50% - 1.5rem);
    }

    @media (min-width: 1200px) {
      width: calc(33% - 1.5rem);
    }
  }

  &__thumb {
    width: 100%;
    border-radius: 0.5rem;
    aspect-ratio: 16/9;
    object-fit: cover;
    object-position: center;
  }

  &__title {
    font-family: $font-title;
    font-size: 1.15rem;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  &__category {
    color: $color-primary-alt;
    font-size: 0.875rem;
  }

  &__description {
    line-height: 150%;
  }

  &__link {
    text-decoration: none;
    color: $color-primary;
    font-size: 1.25rem;
  }
}
</style>
