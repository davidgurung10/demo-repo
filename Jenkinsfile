pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                sh 'python3 -m py_compile code.py --user'
            }
        }
        stage('install pytest'){
         steps{
            sh'pip3 install pytest'}
            }
        stage('test') {
            steps {
                sh 'python3 -m pytest'
            }
        }
        }

}


