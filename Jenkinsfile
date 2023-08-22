// pipeline
// {
//     agent any

//     stages {
//         stage('Build') {
//             steps {
//                 echo 'Building...'
//             }
//         }
//         stage('Test') {
//             steps {
//                 echo 'Testing...'
//             }
//         }
//         stage('Deploy'){
//             steps {
//                 echo 'Deploying...'
//             }
//         }
//     }
// }

// pipeline {
//     agent {
//         docker { image 'node:18.17.1-alpine3.18' }
//     }
//     stages {
//         stage('Test') {
//             steps {
//                 echo 'node --version'
//             }
//         }
//     }
// }

pipeline {
    agent any
    stages {
        stage ('Pulling Image'){
            steps{
                script {
                    sh 'docker run -it -d node'
                    sh 'echo "hello jenkins"'
                }
            }
        }
    }
}