pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL} with ${env.JAVA_HOME} and ${env.EXECUTOR_NUMBER} with ${env.JOB_NAME} on ${env.NODE_NAME} in ${env.WORKSPACEW}"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
		bat 'cmake .'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
