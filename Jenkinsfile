pipeline {
  agent any
  
  stages {
    stage('checkout stage') {
      steps {
        sh 'rm -rf Ansible_project'
        sh 'git clone https://github.com/88janu/grafana.git'
      }
    }
    stage('running playbook') {
      steps {
        sh 'ansible-playbook -i hosts grafana.yml'
      }
    }
  }
}
