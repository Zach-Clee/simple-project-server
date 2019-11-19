pipeline {
    agent any

    stages {
        stage('Testing Environment') {
            steps {
                    sh 'mvn test -Dtest=ControllerAndServiceSuite'
                }
            }
        stage('Build') {
            steps {
		echo "build"
                }
            }
        stage('Deploy') {
            steps {
		echo "deploy"
            }
        }
    }
}

