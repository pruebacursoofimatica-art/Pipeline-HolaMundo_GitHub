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
                echo 'Compilando el código Java...'
                bat 'javac Holamundo.java'  // ✅ javac compila
            }
        }
        stage('Ejecución') {
            steps {
                echo 'Ejecutando la aplicación...'
                bat 'java Holamundo'  // ✅ java ejecuta (sin .java)
            }
        }
    }
}
