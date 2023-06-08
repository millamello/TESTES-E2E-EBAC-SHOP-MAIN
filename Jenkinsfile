pipeline {
    agent any

    stages {
        stage('Clonar Repositorio') {
            steps {
               git branch: 'main', url: 'https://github.com/millamello/TESTES-E2E-EBAC-SHOP-MAIN.git'
            }
        } stage('Instalar Dependências') {
            steps {
               sh 'npm install'
            }
        }
        }stage('Executar Testes') {
            steps {
               sh 'npm run start-server-and-test start-server http://localhost:3000/api-doc test'
            }
        }
    }

}
    