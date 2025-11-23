pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Pull code from your GitHub repo
                git branch: 'main',
                    url: 'https://github.com/chandanarajasri/OnlineArtGalleryy.git'
            }
        }

        stage('Build Backend') {
            steps {
                dir('ArtGalleryFinal') {
                    // Use Maven wrapper to build Spring Boot project
                    sh './mvnw clean package -DskipTests'
                }
            }
        }
    }
}
