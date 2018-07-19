<template lang="pug">
  v-app#backgroundone
    v-toolbar.elevation-0(
      color="teal lighten-3"
      scroll-off-screen
      scroll-target="#scrolling-techniques"
      )
      v-toolbar-title Portfolio
      v-spacer
      v-toolbar-items
        v-btn-toggle.transparent(v-model="toggle_exclusive")
          v-btn(flat color="purple" :value="1") Sobre Mim
          v-btn(flat color="purple" :value="2") Educação
          v-btn(flat color="purple" :value="3") Experiência
          v-btn(flat color="purple" :value="4") Habilidades
    v-content.white
      v-container
        v-layout.blue(column wrap align-center justify-center)
          v-flex(xs12)
            v-avatar.red
      section
</template>

<script>
export default {
  data() {
    return {
      toggle_exclusive: 2,
      rightDrawer: false,
      items: [
        { title: 'Sobre Mim' },
        { title: 'Educação' },
        { title: 'Experiência' },
        { title: 'Habilidades' },
      ],
    };
  },
  name: 'Site',
};
</script>
<style lang="scss">
  #backgroundone {
    background-color: pink
  };
</style>
