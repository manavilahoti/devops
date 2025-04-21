pipeline {
    agent any

    stages {


        stage('Run Backend') {
            steps {
                echo 'Executing Gradle for backend...'
                withGradle {
                    sh './gradlew -v'
                }
            }
        }
    }
}
