<template lang="pug">
  v-app#backgroundOne
    v-toolbar.elevation-0(
      color="teal lighten-3"
      scroll-off-screen
      scroll-target="#scrolling-techniques"
      )
      v-toolbar-title.white--text Patrícia P.L. Machado
      v-spacer
      v-toolbar-items
        v-btn-toggle.transparent(v-model="toggle_exclusive")
          v-btn(route="" flat color="purple" :value="1") Sobre Mim
          v-btn(flat color="purple" :value="2") Educação
          v-btn(flat color="purple" :value="3") Experiência
          v-btn(flat color="purple" :value="4") Habilidades
    v-content
      v-container(grid-list-lg)
        p.cyan--text.text-xs-center.display-3.font-weight-regular.font-italic Desenvolvedora | UX/UI Designer
      img(src="@/assets/desktop.jpg" width="100%" height="auto")
      v-spacer
      v-avatar minha foto
      p.text-xs-center Sobre Mim
      p.text-xs-center Nome
      p.text-xs-center E-mail
      p.text-xs-center Contato
      p.text-xs-center Resumo
      v-btn download resume
      v-spacer
      p.text-xs-center Educação
      p.text-xs-center Experiência
      p linha do tempo
      v-spacer
      p.text-xs-center Habilidades
      p com porcentagem
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
  #backgroundOne {
    background-color: pink
  };
</style>
