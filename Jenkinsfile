pipeline {
    agent any

    stages {
        stage('Testing Environment') {
            steps {
                    sh 'mvn test -Dtest=ControllerAndServiceSuite'
		sh 'mvn test -Dtest=IntegrationSuite'
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

