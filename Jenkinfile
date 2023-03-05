pipeline {
  agent {label'gradle'}  
  stages {
    stage('vcs') {
      steps {
        git url: 'https://github.com/spring-projects/spring-petclinic.git',
          branch: 'declarative'               
        }
     }
     stage('build') {
       steps {
         sh './gradlew build'
         }
       }
    }  
  }