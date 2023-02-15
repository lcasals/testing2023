@Grab('oorg.apache.pdfbox:pdfbox:2.0.1')
import org.apache.pdfbox.pdfbox.2.0.1
void parallelize(int count) {
   if (!Primes.isPrime(count)) {
       error "${count} was not prime"
   }
   // …
}
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
