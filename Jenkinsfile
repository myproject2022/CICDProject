pipeline {
    agent { label 'ansible' }
    
    stages {
        stage ('Checkout') {
          steps {
            git 'git@github.com:myproject2022/CICDProject.git'
          }
        }
      stage ('run playbook') {
          steps {
            sh "ansible-playbook apache.yaml"
          }
        }
       
    }
}
