pipeline {

    agent any


    stages {


        stage('Checkout desde Git') {

            steps {

                git 'https://github.com/rebecamorales/Practica.git'

            }

        }



        stage('Docker Compose Down') {

            steps {

                sh 'docker compose down'

            }

        }



        stage('Docker Compose Up') {

            steps {

                sh 'docker compose up -d'

            }

        }



        stage('Verificar despliegue') {

            steps {

                sh 'docker ps'

            }

        }


    }

}