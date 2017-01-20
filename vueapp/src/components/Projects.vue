<template>
 <div id="resume-data" class="data-padding">
  <md-layout md-gutter md-align="center">
    <md-row>
      <md-column>
        <h1 id="resume-header">PROJECTS</h1>
        <md-card md-with-hover>
          <md-card-header>

            <div class="md-title">Full Stack Engineer | Back End Engineer | Front End Designer</div>
          </md-card-header>

          <md-card-content>
            <md-layout md-gutter>
              <md-layout md-flex-xsmall="100" md-flex-small="100" md-flex-medium="100" md-flex-large="100">
              <p>Education:
              North Carolina State University - Bachelor of Science in Computer Science
              </p>
              </md-layout>
              <md-layout md-flex-xsmall="100" md-flex-small="33" md-flex-medium="33" md-flex-large="33">
                <a class="resume-links" href="">LinkedIn: </a>
              </md-layout>
              <md-layout md-flex-xsmall="100" md-flex-small="33" md-flex-medium="33" md-flex-large="33">
                <a class="resume-links" href="">GitHub</a>
              </md-layout>
              <md-layout md-flex-xsmall="100" md-flex-small="33" md-flex-medium="33" md-flex-large="33">
                <a class="resume-links" href="">Medium</a>
              </md-layout>
            </md-layout>
          </md-card-content>

          <md-card-actions>
            <md-button>
              <md-icon>phone</md-icon>
            </md-button>
            <md-button class="md-raised md-primary">
              <md-icon>mail</md-icon>
            </md-button>
          </md-card-actions>

        </md-card> 
      </md-column>
    </md-row>
  </md-layout>
</div>
</template>

<script>
export default {
  name: 'resume',
  data () {
    return {
    }
  },
  methods: {
  }
}
</script>

<style scoped>
#resume-data {
  background-color: #a5d6a7;
}

#resume-header {
  font-weight: light;
  color: white;
}

</style>