<template>
  <section id="projects">
    <div class="container">
      <h2 class="title">Featured Projects</h2>
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
</style>
