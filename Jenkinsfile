pipeline {
    agent any
    
    stages {
        
        stage('compile ') {
            steps {
                sh 'mvn compile'
            }
        }

        stage('build') {
            steps {
                 sh 'mvn clean install'
            }
        }

        
    }

  post{

  success{
     echo 'Build success 1'
  }
    
  failure{
       echo 'Failure in the build'
   }

  }


}
