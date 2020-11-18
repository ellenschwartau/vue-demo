<template>
  <div class="profile">
    <h2>Skills</h2>
    <Competence title="Main Competencies" :competencies=main />
    <Competence title="Backend" :competencies=backend />
    <Competence title="Frontend" :competencies=frontend />
    <Competence title="Database" :competencies=database />
    <Competence title="Messaging" :competencies=messaging />
    <Competence title="Platform" :competencies=platform />
    <Competence title="Tooling" :competencies=tooling />
    <Competence title="Processes" :competencies=processes />
  </div>
</template>

<script>
import Competence from './Competence.vue'

export default {
  name: 'Profile',
  data: function () {
    return {
      main: [ 'Fullstack Development', 'Microservices', 'Web Development', 'Java', 'Javascript', 'React' ],
      backend: [ 'Java', 'Dropwizard', 'Jersey', 'Jackson', 'Elasticsearch', 'Kotlin', 'Machine Learning', 'Python', 'Haskell', 'Spring Boot' ],
      frontend: [ 'JavaScript', 'Node', 'React', 'Redux', 'Flow', 'Html', 'Scss', 'Angular' ],
      database: [ 'MySql', 'PostgreSQL', 'Bigtable', 'BigQuery', 'Jdbi', 'Hibernate' ],
      messaging: [ 'Kafka', 'RabbitMQ' ],
      platform: [ 'Docker', 'Google Cloud Services', 'Kubernetes' ],
      tooling: [ 'Git', 'Gitlab', 'Bitbucket', 'Jenkins', 'Jira', 'Confluence' ],
      processes: [ 'Scrum', 'Kanban' ],
    }
  },
  components: { Competence }
}
</script>