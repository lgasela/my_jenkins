pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    java -version
                '''              
                
               }
            }
        stage('read') {
           steps {
               script {
                   def data = readFile(file: 'rubbish)
                   println(data)
               }
           }
        }
    }
}
