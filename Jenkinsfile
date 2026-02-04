pipeline {
    agent any

    stages {
        stage('Deploy to Web Server') {
            steps {
                dir('/var/www/html') {
                    git branch: 'master',
                        url: 'https://github.com/priyankabakship-afk/myrepo.git',
                        credentialsId: 'github-jenkins'
                }
            }
        }
    }
}
