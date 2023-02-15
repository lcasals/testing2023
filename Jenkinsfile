library identifier: 'org.apache.commons:commons-math3:3.4.1', retriever: modernSCM([$class: 'GitSCMSource', credentialsId: '', remote: 'https://mvnrepository.com/artifact/org.apache.commons/commons-math3/3.4.1', traits: [gitBranchDiscovery()]])
pipeline {
   agent any
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                echo "doing build stuff.."
                
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                echo "doing test stuff.."
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                echo "doing delivery stuff.."
            }
        }
        stage('Compile Java program') {
            steps {
                echo "working on Java program.."
                script {
                    echo "Compiling File Detection program..."
                    sh " javac ./src/FileTypeDetection.java"
                 }
            }
        }
        stage('Run Java program') {
            steps {
                echo "Running File Detection program..."
                script {
                    echo "Checking Files Uploaded..."
                    sh " java ./src/FileTypeDetection.java"
                 }
            }
        }
    }
}
