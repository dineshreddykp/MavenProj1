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
        sh 'mvn -f clean'
        }
		}
        stage('MavenBuild'){
		steps {
        sh 'mvn -f test'
        }
		}
        stage('BuildSuccessMessage'){
		steps{
            sh "echo =============success============="
            }
        }
    }
}
