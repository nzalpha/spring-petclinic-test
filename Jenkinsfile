pipeline {
    agent {
        label 'K8-slave'
    }
    tools {
        maven 'mvn 3.8'
        jdk 'jdk-17'
    }

      stages {
        stage ('Build') {
                     // This step will take care of building the application
            steps {
                echo "test"
            }
        }
      }
}
