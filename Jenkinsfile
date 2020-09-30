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
        sh 'mvn -f MavenProj1/pom.xml clean'
        }
		}
        stage('MavenBuild'){
		steps {
        sh 'mvn -f MavenProj1/pom.xml test'
        }
		}
        stage('BuildSuccessMessage'){
		steps{
            sh "echo =============success============="
            }
        }
    }
}
