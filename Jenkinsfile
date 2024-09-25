pipeline {
    agent any
  
    stages {
        
        // stage('Checkout') {
        //     steps {
        //         git branch: 'main', url: 'https://github.com/medhammadi/stage.git'
        //     }
        // }
        
        // stage('Build Backend image') {
        //     steps {
        //         script {
        //             // Construction de l'image backend
        //             docker.build("medhammadi/backend:latest", "-f ./Backend/Dockerfile .")
        //         }
        //     }
        // }
        
        
        // stage('Push Backend image to Docker Hub') {
        //     steps {
        //         script {
        //             try {
        //                 docker.withRegistry('https://registry.hub.docker.com', 'medhammadi') {
        //                     docker.image("medhammadi/backend:latest").push()
        //                 }
        //             } catch (e) {
        //                 error "Échec du push de l'image backend: ${e}"
        //             }
        //         }
        //     }
        // }
        
        // stage('Build Frontend image') {
        //     steps {
        //         script {
        //             // Construction de l'image avec le nom correct
        //             docker.build("medhammadi/frontend:latest", "-f ./Frontend/Dockerfile .")
        //         }
        //     }
        // }


        // stage('Push Frontend image to Docker Hub') {
        //     steps {
        //         script {
        //             try {
        //                 docker.withRegistry('https://registry.hub.docker.com', 'medhammadi') {
        //                     docker.image("medhammadi/frontend:latest").push()
        //                 }
        //             } catch (e) {
        //                 error "Échec du push de l'image frontend: ${e}"
        //             }
        //         }
        //     }
        // }
        
        stage('Deploy Application with Docker Compose') {
            steps {
                script {
                    // Déployer l'application avec Docker Compose
                    sh "docker-compose up -d"
                }
            }
        }

    }
}
