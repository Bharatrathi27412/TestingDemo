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
    agent any
    stages {
        stage('Test') {
            steps {
                powershell 'docker pull node'
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