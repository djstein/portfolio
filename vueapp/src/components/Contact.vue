<template>
<div id="contact-data" class="data-padding ">
  <md-layout md-gutter md-align="center">
    <md-row>
      <md-column>
        <h1 id="contact-header">CONTACT</h1>

          <md-card md-with-hover>

            <md-card-header>
              <md-card-header-text>
                <div class="md-title">Software Engineer</div>
                <div class="md-subhead">Full Stack | Back End | Front End</div>
                
                <ul>
                  <li>Email: <a href="">djstein@ncsu.edu</a></li>
                  <li>LinkedIn: <a href="">linkedin.com/in/dylanstein</a></li>
                  <li>GitHub: <a href="">github.com/djstein</a></li>
                </ul>

              </md-card-header-text>
              <md-card-media md-medium>
                <img id="profile" src="https://avatars3.githubusercontent.com/u/8503952?v=3&s=460"/>
              </md-card-media>
            </md-card-header>

          </md-card> 

      </md-column>
    </md-row>
  </md-layout>
  </div>

</template>

<script>
export default {
  name: 'contact',
  data () {
    return {
    }
  },
  methods: {
  }
}
</script>

<style scoped>

#contact-data {
  background-color: #78909c;
}

#contact-header {
  font-weight: light;
  color: white;
}

ul {
  list-style-type: none;
  padding: 0 0 0 0;
  margin: 0 0 0 0;
}

li {
  padding: 0 0 0 0;
  margin: 0 0 0 0;
}
</style>