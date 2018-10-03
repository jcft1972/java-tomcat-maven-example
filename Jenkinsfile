pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat "mvn -version"
                bat 'mvn -B -DskipTests clean package'
                bat 'mvn archetype:compile'
                bat 'mvn archetype:generate -DarchetypeArtifactId=maven-archetype-webapp'
            }
        }
        stage('Delivery') {
            steps {
                bat "echo Aqui delivery"
            }
        }
        stage('Deploy') {
            steps {
                bat "echo Aqui Deploy"
            }
        }
    }
}
