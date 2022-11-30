pipeline {
    agent any 
    stages {
        stage('clone repo') { 
            steps {
                sh "git: https://github.com/dharmaraj257/angular-project.git"
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
