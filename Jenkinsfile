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

pipeline {
    agent {
        docker { image 'node:18.17.1-alpine3.18' }
    }
    stages {
        stage('Test') {
            steps {
                environment {
                  HOME="."
                }
                echo 'node --version'
            }
        }
    }
}

// pipeline {
//     agent any
//     stages {
//         stage ('Pulling Image'){
//             steps{
//                 // This step should not normally be used in your script. Consult the inline help for details.
//                 withDockerContainer(args: '-it -d', image: 'node') {
//                 // some block
// }
//             }
//         }
//     }
// }