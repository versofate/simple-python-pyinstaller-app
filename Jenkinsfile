pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                label 'slave1'
            }
            steps {
                sh 'python3 -m py_compile sources/add2vals.py sources/calc.py' 
            }
        }
    }
}
