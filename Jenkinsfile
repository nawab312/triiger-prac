pipelines {
    agent any
    triggers {
        githubPush()
    }
    stages {
        stage('Clone the Repo') {
            steps {
                git url: 'https://github.com/nawab312/triiger-prac.git', branch: 'main'
            }
        }
        stage('Execute the Script') {
            steps {
                sh './hello-world.sh'
            }
        }
    }
}