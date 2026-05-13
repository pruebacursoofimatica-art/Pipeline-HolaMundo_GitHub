pipeline {
    agent any 
    stages {
        stage('Checkout') {
            steps {
                echo 'Obteniendo el código desde GitHub...'
            }
        }
        stage('Compilación') {
            steps {
                // Se asume que el servidor es Windows por las capturas anteriores
                bat 'java Holamundo.java' 
            }
        }
        stage('Ejecución') {
            steps {
                bat 'java Holamundo'
            }
        }
    }
}
