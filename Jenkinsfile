pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/chandanarajasri/OnlineArtGalleryy.git'
            }
        }

        stage('Build Backend') {
            steps {
                dir('ArtGalleryFinal') {
                    sh 'chmod +x mvnw'
                    sh './mvnw clean package -DskipTests'
                }
            }
        }
    }
}
