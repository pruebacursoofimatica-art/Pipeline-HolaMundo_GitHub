pipeline {
    agent any
    environment {
        // Ajusta esta ruta a la instalación real de JDK en tu servidor
        JAVA_HOME = 'C:\\Program Files\\Java\\jdk-17'
        PATH = "${JAVA_HOME}\\bin;${env.PATH}"
    }
    stages {
        stage('Checkout') {
            steps {
                echo 'Obteniendo el código desde GitHub...'
            }
        }
        stage('Compilación') {
            steps {
                echo 'Compilando el código Java...'
                bat 'javac Holamundo.java'
            }
        }
        stage('Ejecución') {
            steps {
                echo 'Ejecutando la aplicación...'
                bat 'java Holamundo'
            }
        }
    }
}
