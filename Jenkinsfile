pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/SUSHANTSATONKAR/ansible-jenkins-lab.git'
            }
        }

        stage('Run Ansible Playbook') {
            steps {
                // Ensure you use 'sh' for shell commands in Linux environments
                sh 'ansible-playbook -i hosts install_apache.yml'
            }
        }
    }
}
