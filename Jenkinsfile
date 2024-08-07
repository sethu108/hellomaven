pipeline {
    agent any 
    stages{
        stage('Build Maven'){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/sethu108/hellomaven']]])
                bat 'mvn clean install'
            }
        }
		stage('package'){
		   steps{
				echo "hello package"
				}
		}
        
    }
}