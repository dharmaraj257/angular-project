pipeline {
    agent any 
    stages {
        stage('clone repo') { 
            steps {
                bat "git https://github.com/dharmaraj257/angular-project.git"
                bat "ng clean -f angular-project"
            }
        }
        stage('build') { 
            steps {
                bat "ng build -f angular-project"
            }
        }
        stage('Serve') { 
            steps {
                bat "ng serve -f angular-project"
            }
        }
    }
}
