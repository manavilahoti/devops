pipeline {
    agent any

    stages {
        stage('Run Frontend') {
            steps {
                echo 'Executing yarn for frontend...'
                sh 'yarn install' 
            }
        }

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
