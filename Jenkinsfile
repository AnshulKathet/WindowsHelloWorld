pipeline {
    agent none
    stages {
        stage("Stage 1") {
            steps {
                node('Jenkins-Win'){
                    script {
                        writeFile(file: 'test.txt', text: 'Hello World!', encoding: 'UTF-8')
                    }
                    // This should print the file content on slave (Hello World!)
                    bat "type test.txt"
                }
            }
        }
    }
}