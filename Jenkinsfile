pipeline {
    agent any 
    stages {
        stage('clone repo') { 
            steps {
                sh "git branch: 'main', credentialsId: 'd271284c-7874-4725-ab78-43323f7b8de6', url: 'https://github.com/dharmaraj257/angular-project.git'"
                sh "ng clean -f angular-project"
            }
        }
        stage('build') { 
            steps {
                sh "ng build -f angular-project"
            }
        }
        stage('Serve') { 
            steps {
                sh "cd angular-project -f angular-project"
                sh "ng serve -f angular-project"
            }
        }
    }
}
