pipeline {
    agent { label 'NODE 1' }
    triggers {
        cron('*/5 * * * *')
      }
    stages {
        stage('Source Code') {
            steps {
                git url: 'https://github.com/saiprakashreddivari/spring-petclinic.git', 
                branch: 'develop'
            }
            
        }
        stage(Maven) {
            steps {
                sh 'mvn package'
                  }
                      }
             

      }
}