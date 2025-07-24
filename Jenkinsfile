pipeline {
    agent any

    stages {
        stage('Clonar repositorio') {
            steps {
                git branch: 'develop', url: 'https://github.com/JoseRojas22/etl-risk-python.git'
            }
        }

        stage('Ejecutar ETL') {
            steps {
                sh 'python extract.py'
            }
        }
    }
}
