pipeline {
    agent any
    triggers {
        pollSCM('* * * * *')
    }
    stages {
        stage('Compile') {
            steps {
                sh "./gradlew compileJava"
            }
        }
    }
    post {
	 always {
		sh "echo 'Hello World'"
	 }
    }
}
