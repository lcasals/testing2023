<dependency>
    <groupId>org.apache.pdfbox</groupId>
    <artifactId>pdfbox</artifactId>
    <version>2.0.1</version>
</dependency>
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
                    sh " javac ./src/PdfFile.java"
                 }
            }
        }
        stage('Run Java program') {
            steps {
                echo "Running File Detection program..."
                script {
                    echo "Checking Files Uploaded..."
                    sh " java ./src/PdfFile.java"
                 }
            }
        }
    }
}
