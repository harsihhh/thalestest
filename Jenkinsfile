pipeline {
  agent anykjsbjsbjsdbvkjfdjlvdfvjbskjvbskjssssssssbvkjsbvkjsbvkjsbvkjskvjbskjvbw
  stages {
    stage('Test') {
      parallel {
        stage('Maven') {
          steps {
            echo 'Running from Jenkins file'
            sh(script: 'mvn compile', label: 'maven')
          }
        }

        stage('Cucumber') {
          steps {
            cucumber '**/*.json'
          }
        }

      }
    }

  }
}
