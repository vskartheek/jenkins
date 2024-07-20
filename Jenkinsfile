pipeline {
        agent any
    stages{
        stage('fetch code from git'){
            steps{
                git branch: 'main', url: 'https://github.com/vskartheek/jenkins.git'
            }
        }
    }
    
}
