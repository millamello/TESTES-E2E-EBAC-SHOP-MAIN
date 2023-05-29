pipeline {
    agent any

    stages {
        stage('Clonar repositório') {
            steps {
                git branch: 'main', url: 'https://github.com/millamello/TESTES-E2E-EBAC-SHOP-MAIN.git'
            }
        }
        stage('Instalar dependências') {
            steps {
                powershell 'npm install'
            }
        }
        stage('Ativar plugin ansiColor') {
            steps {
                ansiColor('gnome-terminal') {
    // some block
}
            }
        }
        
        stage('exercutar os testes ') {
            steps {
                powershell 'npm run cy:run'
            }
        }
    }
}