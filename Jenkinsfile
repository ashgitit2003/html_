pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/ashgitit2003/html_'
            }
        }
        stage('Deploy to Xampp') {
            steps {
                bat 'xcopy /s /y "C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\html deployment\\*.html" "C:\\xampp\\htdocs\\"'
            }
        }
    }
}
