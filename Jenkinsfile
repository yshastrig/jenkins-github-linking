pipeline{
    agent{
        label 'ansible'
    }

    stages{
        stage('SCM Checkout'){
            steps{
                git 'https://github.com/yshastrig/jenkins-github-linking'
            }
        }
        stage('Ansible Execution'){
            steps{
                sh 'ansible-playbook -v playlist.yml'
            }
        }
    }
}
