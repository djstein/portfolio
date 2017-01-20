<template>

  <div class="portfolio">
    <h1 id="name">{{ name }}</h1>
    <contact></contact>
    <resume></resume>
    <projects></projects>
  </div>
</template>

<script>
import Contact from './Contact'
import Resume from './Resume'
import Projects from './Projects'

export default {
  components: {
    Contact,
    Resume,
    Projects
  },
  name: 'portfolio',
  data () {
    return {
      name: 'DYLAN STEIN'
    }
  },
  methods: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

#name {
  font-size: 3em;
  white-space: nowrap;
  font-weight: light;
  margin-top: .3em;
  margin-bottom: .5em;
  margin-left: .3em;
}


.md-card-header > .md-card-header-flex {
  padding: 0 0 0 0;
  margin: 0 0 0 0;
}

@media screen and (min-width: 576px) {
  #name {
    font-size: 5em;
    margin-left: .2em;
  }
  .data-padding {
    padding-left: 1em;
    padding-right: 1em;
    padding-bottom: 4em;
  }
}

@media screen and (min-width: 768px) {
  #name {
    font-size: 7em;
    margin-left: .12em;
  }
}

</style>
