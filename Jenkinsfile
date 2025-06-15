pipeline {
    agent any
    tools {
        gradle 'Gradle8.14.2'
    }
    stages {
        stage("run frontend") {
            steps {
                echo 'execute yarn'
                nodejs('node 24.2') {
                    sh 'yarn install'
            }
            }
        }
  
        stage("run backend") {
            steps {
                echo 'execute gradle'
                
                    sh 'chmod +x gradlew'
                    sh './gradlew -v'
                
            }
        }
    }
    }

