pipeline {
    agent any
    stages {
        stage ("vcs"){
            steps {
                git url: "https://github.com/GitPracticeRepo/js-e2e-express-server.git",
                branch: "main"
            }
        }
        stage ("install"){
            steps {
                sh "npm install",
                sh "npm run build"
            }
        }
    }
}