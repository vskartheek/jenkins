pipeline {
        agent any
    stages{
        stage('fetch code from git'){
            steps{
                git branch: 'main', url: 'https://github.com/vskartheek/jenkins.git'
            }
        }
          stage('install server on node'){
            steps{
               ansiblePlaybook credentialsId: '8e390fc3-0441-4d1c-b315-00cdd6117392', inventory: 'dev', playbook: 'playbook1.yml', vaultTmpPath: ''
            }
        }
    }
}
