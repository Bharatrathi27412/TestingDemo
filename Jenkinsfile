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

pipeline 
{
    agent 
    {
        docker 'node:18.17.1-alpine3.18' 
    }
    stages
    {
        stage ('Test')
        {
            steps {
                sh 'node --version'
            }
        }
    }
}