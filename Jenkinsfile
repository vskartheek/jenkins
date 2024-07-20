pipeline {
        agent any
    stages{
        stage('fetch code from git'){
            steps{
                git branch: 'main', url: 'https://github.com/vskartheek/jenkins.git'
            }
        }
        stage('install web server on client'){
                steps{
                        ansiblePlaybook playbook: 'playbook1.yml', vaultTmpPath: ''
                }
            }
        stage('deploy application'){
                steps{
                        ansiblePlaybook playbook: 'playbook2.yml', vaultTmpPath: ''
                }
            }
    }
}
