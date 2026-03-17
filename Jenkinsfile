pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                // The 'git' step automatically checks out the repository to the workspace
                git url: 'https://github.com/anikesh0001/simplejenkins.git',
                    branch: 'main'
            }
        }

        stage('Run Script') {
            steps {
                // Ensure the script is executable and run it using 'sh'
                sh 'chmod +x script.sh'
                sh './script.sh'
            }
        }
        
        stage('Run python') {
            steps {
                // Use the 'sh' step to execute the python script with the python interpreter
                sh 'python modification.py'
            }
        }
    }
}
