<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    p.mb-5 Las empresas del siglo XXI deben hacer constantemente un diagnóstico organizacional para identificar situaciones de mejora continua, por lo que la única forma de comparar situaciones es mediante información de periodos que les permita, conocer dónde, qué, quién, cuándo, por qué, cómo, etc., se presentan fallas para generar un plan de mejora continua mediante un PHVA y un seguimiento permanente del proceso, por lo que en el siguiente mapa conceptual podrá identificar cada uno de los pasos que se deben seguir para lograr implementar un sistema de gestión de calidad empresarial y de igual manera ver resumida la temática tratada en el componente formativo.

    .row.justify-content-center
      .col-lg-10.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="alt")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
