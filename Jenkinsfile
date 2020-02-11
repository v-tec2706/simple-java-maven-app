// pipeline {
//     agent {
//         docker {
//             image 'maven:3-alpine'
//             args '-v /root/.m2:/root/.m2'
//         }
//     }
//     options {
//         skipStagesAfterUnstable()
//     }
//     stages {
//         stage('Build') {
//             steps {
//                 sh 'mvn -B -DskipTests clean package'
//             }
//         }
//         stage('Test') {
//             steps {
//                 sh 'mvn test'
//             }
//             post {
//                 always {
//                     junit 'target/surefire-reports/*.xml'
//                 }
//             }
//         }
//         stage('Deliver') {
//             steps {
//                 sh './jenkins/scripts/deliver.sh'
//             }
//         }
//         stage('Summary') {
//             steps {
//                 sh 'echo heloooo! it works'
//                 sh './jenkins/myScripts/myScript.sh'
//             }
//         }
//     }
// }


pipeline {
    agent any
    stages {
        stage('Initial') {
            steps {
                sh 'echo Hello from this job, now we have: $(time) !'
            }
        }
    }
}