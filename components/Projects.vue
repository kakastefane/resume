<template>
  <section id="projects">
    <div class="container">
      <h2 class="title">Featured Projects</h2>

      <ul class="project">
        <li v-for="project in projects" :key="project.id" class="project__item">
          <NuxtLink to="/">
            <img class="project__thumb" :src="project.thumb" alt="teste" />
          </NuxtLink>
          <h3 class="project__title">
            {{ project.title }}
            <a class="project__link" :href="project.link" title="Go to project"
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
          title: 'Project Title',
          description:
            'Lorem ipsum dolor sit amet consectetur adipisicing elit. Id ipsam soluta, voluptatem dolor illo consectetur!',
          category: 'UI Design, Front-End',
          thumb: 'http://placehold.it/300x200',
          link: 'http://google.com',
        },
        {
          id: 2,
          title: 'Project Title',
          description:
            'Lorem ipsum dolor sit amet consectetur adipisicing elit. Id ipsam soluta, voluptatem dolor illo consectetur!',
          category: 'UI Design, Front-End',
          thumb: 'http://placehold.it/300x200',
          link: 'http://google.com',
        },
        {
          id: Math.random(),
          title: 'Project Title',
          description:
            'Lorem ipsum dolor sit amet consectetur adipisicing elit. Id ipsam soluta, voluptatem dolor illo consectetur!',
          category: 'UI Design, Front-End',
          thumb: 'http://placehold.it/300x200',
          link: 'http://google.com',
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
