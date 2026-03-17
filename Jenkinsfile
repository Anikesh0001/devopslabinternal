pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git url: 'https://github.com/anikesh0001/devopslabinternal.git',
                    branch: 'main'
            }
        }

        stage('Run Script') {
            steps {
                python 'modification.py'
            }
        }
    }
}
