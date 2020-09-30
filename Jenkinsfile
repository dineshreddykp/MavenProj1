pipeline {
    agent any
    stages {
        stage('MavenVersion') {
            steps {
                sh "mvn --version"
            }
        }
		 stage('clean'){
		steps {
        sh 'mvn clean'
        }
		}
        stage('MavenBuild'){
		steps {
        sh 'mvn test'
        }
		}
        stage('BuildSuccessMessage'){
		steps{
            sh "echo =============success============="
            }
        }
    }
}
