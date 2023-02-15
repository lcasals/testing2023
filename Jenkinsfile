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
        stage('Run Java program') {
            steps {
                echo "Running File Detection program..."
                script {
                    echo "Checking Files Uploaded..."
                    cd src
                    sh "java -jar myJar.jar"
                 }
            }
        }
    }
}
