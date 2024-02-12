pipeline {
  agent any
  
  stages {
    stage('checkout stage') {
      steps {
        sh 'rm -rf grafana_ansible'
        sh 'git clone https://github.com/88janu/grafana_ansible.git'
      }
    }
    stage('running playbook') {
      steps {
        sh 'ansible-playbook -i hosts grafana.yml'
      }
    }
  }
}
