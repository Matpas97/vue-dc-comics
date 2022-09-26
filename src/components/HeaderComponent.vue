<template>
  <div class="container">
    <header>
      <div id="logo">
        <img src="../assets/img/dc-logo.png" alt="DC logo" />
      </div>
      <nav>
        <ul>
          <li v-for="link in links" :key="link.title">
            <a :href="link.link" :class="{ active: link.active }">
              {{ link.title }}
            </a>
          </li>
        </ul>
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  name: 'HeaderComponent',
  data() {
    return {
      links: [
        {
          title: 'Characters',
          link: '#',
          active: false,
        },
        {
          title: 'Comics',
          link: '#',
          active: true,
        },
        {
          title: 'Movie',
          link: '#',
          active: false,
        },
        {
          title: 'TV',
          link: '#',
          active: false,
        },
        {
          title: 'Games',
          link: '#',
          active: false,
        },
        {
          title: 'Collectibles',
          link: '#',
          active: false,
        },
        {
          title: 'Videos',
          link: '#',
          active: false,
        },
        {
          title: 'Fan',
          link: '#',
          active: false,
        },
        {
          title: 'News',
          link: '#',
          active: false,
        },
        {
          title: 'Shop',
          link: '#',
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import '@/styles/variables';

header {
  display: flex;
  justify-content: space-between;
}

#logo{
width: 50px;
    margin: 10px 5px;
}

ul {
  list-style-type: none;
  height: 100%;
  display: flex;
  li {
    height: 100%;
    padding: 0px 15px;
    a {
      text-decoration: none;
      color: #000;
      text-transform: uppercase;
      display: flex;
      height: 100%;
      align-items: center;
       &.active {
        border-bottom: 2px solid $brand-color;
      }
    }
  }
}
</style>