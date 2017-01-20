<template>
 <div id="resume-data" class="data-padding">
  <md-layout md-gutter md-align="center">
    <md-row>
      <md-column>
        <h1 id="resume-header">RESUME</h1>
        <md-card md-with-hover>
          <md-card-header>

            <div class="md-title">Education</div>
                        <div class="md-subtitle">North Carolina State University | Bachelor of Science in Computer Science</div>

          </md-card-header>

          <md-card-content>
            <md-layout md-gutter>
              <md-layout md-align="center" md-flex-xsmall="100" md-flex-small="100" md-flex-medium="100" md-flex-large="100">

              <md-list class="course-list">
                <md-list-item>
                  <md-icon>school</md-icon>
                  <span>Course Work</span>
                  
                  <md-list-expand>
                    <md-list v-for="course in courses">
                      <md-list-item class="course">{{course}}</md-list-item>
                    </md-list>
                  </md-list-expand>
                </md-list-item>
              </md-list>

              </md-layout>
              </md-layout>
            </md-layout>
          </md-card-content>

        </md-card>
      </md-column>
    </md-row>

</br>

<md-layout md-gutter md-align="center">
              <md-layout></md-layout>

  <md-row>
    <md-column v-for="job in jobs">
      <md-card md-with-hover>
        <md-card-header>

          <div class="md-title">{{job.company}}</div>
          <div class="md-subtitle">{{job.title}} {{job.start}} - {{job.end}}</div>
          </md-card-header>

          <md-card-content>
            <md-layout md-gutter>
              <md-layout md-align="center" md-flex-xsmall="100" md-flex-small="100" md-flex-medium="100" md-flex-large="100">
                {{job.description}}
              </md-layout>
              </md-layout>
            </md-layout>
          </md-card-content>
        </md-card>
      </md-column>
    </md-row>
  </md-layout>
              <md-layout></md-layout>

  </md-layout>
</div>
</template>

<script>
export default {
  name: 'resume',
  data () {
    return {
      courses: [
        'CSC 116 - Introduction to Computing - Java',
        'CSC 216 - Programming Concepts - Java',
        'CSC 226 - Discrete Mathematics for Computer Scientists',
        'CSC 230 - C and Software Tools',
        'CSC 236 - Computer Organization and Assembly Language for Computer Scientists',
        'CSC 246 - Concepts and Facilities of Operating Systems for Computer Scientists',
        'CSC 316 - Data Structures for Computer Scientists',
        'CSC 326 - Software Engineering',
        'CSC 316 - Data Structures for Computer Scientists',
        'CSC 333 - Automata, Grammars, and Computability',
        'CSC 379 - Ethics in Computing',
        'CSC 405 - Introduction to Computer Security',
        'CSC 440 - Database Management Systems',
        'CSC 454 - Human-Computer Interaction',
        'CSC 492 - Senior Design Project'
      ],
      jobs: [
        { 'company': 'Oscar Labs - NCSU  ITNG',
          'title': 'Software Engineer',
          'start': 'August 2014',
          'end': 'December 2016',
          'description': 'Work in a small team environment developing internal applications. In charge of creating requirement documentation, developing, testing, and dep loying   Django  applications. Communicate decisions to other engineers to meet goals, deadlines, and close production issues.'
        },
        { 'company': 'BoostOurTeam LLC',
          'title': 'Chief Technology Officer',
          'start': 'October 2015',
          'end': 'Current',
          'description': 'Front end development for Sears Parts Direct Team. Determine complexity of pages aiming to improve packet transfer, client runtime, and server side load. Use a variety of skills to improve site flow including:   Javascript (jQuery, Han dleba r.js, Angular.js ),  Java, CSS3 ( SASS  ), HTML5,  B  ootstrap,  Adobe CQ.'
        },
        { 'company': 'Sears Holdings',
          'title': 'Member Technology Intern',
          'start': 'May 2016',
          'end': 'August 2016',
          'description': 'Front end development for Sears Parts Direct Team. Determine complexity of pages aiming to improve packet transfer, client runtime, and server side load. Use a variety of skills to improve site flow including:   Javascript (jQuery, Han dleba r.js, Angular.js ),  Java, CSS3 ( SASS  ), HTML5,  B  ootstrap,  Adobe CQ.'
        },
        { 'company': 'IBM Open Project - NCSU Senior Design',
          'title': 'Team Leader',
          'start': 'January 2016',
          'end': 'May 2016',
          'description': 'Create addition to  IBM Enterp rise Exception Handler. Framework created to recognize exceptions using a class’s Abstract Syntax Tree to standardize usage across all projects.  Adv  anced Jav  a techniques,  JazzHub usage.  Demo and theory presentations give for IBM Open Project and large scale conference.'
        },
        { 'company': 'Principal Financial Group',
          'title': 'IT Intern - Java Application Developer',
          'start': 'May 2015',
          'end': 'August 2015',
          'description': 'Create Java  web applications  for assets under management participants to administer their company service plans. Translate data from legacy  Cob  ol systems to Java objects  that are manipulated on front end. Advanced debugging and restructuring of e xisting pages. Multiple  Agile  teams st ructured a round  Confluence  and   JIRA.  Team leader for PFG CodeJam, where internal  Django  web application was created.'
        },
        { 'company': 'Principal Financial Group',
          'title': 'IT Intern - Java Application Developer',
          'start': 'May 2014',
          'end': 'August 2014',
          'description': 'Work on projects for Principal Financial Groups Retirement and Investment Services group. Projects included development on  backend Java applica  tions.Trained on SCRU  M/Agile, IBM DB2, SQL ( JDBC),  Jenkins,  Maven. Created video game project during three days at PFG Code Jam.'
        },
        { 'company': 'Principal Financial Group',
          'title': 'IT Intern',
          'start': 'May 2013',
          'end': 'August 2013',
          'description': 'Worked on systems that involved the creation of new servers for a Business Objects upgrade. Designed and created user interface for mobile application in PFG three day Code Jam. Work included using MS SharePoint, Business Objects, and Adaptive softwares. Trained on corporate dynamics.'
        }
      ]
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

ul {
  list-style-type: none;
  padding: 0 0 0 0;
  margin: 0 0 0 0;
}

li {
  padding: 0 0 0 0;
  margin: 0 0 0 0;
  }

@media screen and (min-width: 576px) {

}

</style>