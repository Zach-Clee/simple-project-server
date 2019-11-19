pipeline {
    agent any

    stages {
        stage('Testing Environment') {
            steps {
                    sh 'mvn test -Dtest=ControllerAndServiceSuite'
		sh 'mvn test -Dtest=IntegrationSuite'
		sh 'mvn package -DskipTests'                
		sh 'docker build -t="zachclee/simple-project:latest".'
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

