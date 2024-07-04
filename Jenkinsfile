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
            when{
                anyOf{
                    expression{
                        params.buildOnly == 'yes'
                    }
                }
            }


            // This step will take care of building the application
            steps {
                script{
                 buildApp().call()
                }
            }
        }
      }
}
