pipeline {
    agent any
    pollSCM('* * * * *')
    stages {
        stage('Compile') {
            steps {
                sh "./gradlew compileJava"
            }
        }
    }
}
