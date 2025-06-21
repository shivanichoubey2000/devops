pipeline{
    agent any
    
    stages{
        stage("checkout from github")
        {
            steps{
                echo"github"
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github', url: 'https://github.com/shivanichoubey2000/devops.git']])
            }
        }
        stage("checkout from docker")
        {
            steps{
                echo"docker"
                sh '''ls -ltr
                df -h'''
            }
        }
    }
}
