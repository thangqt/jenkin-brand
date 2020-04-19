pipeline {
   agent {
        docker {
            image 'gradle:6.3.0-jdk8'
        }
    }
   stages {
      stage('Build') {
         steps {
            sh 'gradle clean build'
            junit '**/target/surefire-reports/TEST-*.xml'
         }
      }
   
      stage('Deloy') {
         steps {
            echo "Deloy stagin"
         }
      }
   }
}
