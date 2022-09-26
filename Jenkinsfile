pipeline {
    agent any

    stages {
        stage('Clone resources') {
            steps {
                git branch: 'main', url: 'https://github.com/cheevavorn/lab4-multiple-stage.git'
            }
        }

        stage('Create new file') {
            steps {
                sh 'touch multiple.txt'
            }
        }

        stage('Concat \'Hello\'') {
            steps {
                sh 'echo \'Hello\' >> multiple.txt'
            }
        }

        stage('Concat \' Jenkins\'') {
            steps {
                sh 'echo \' Jenkins\' >> multiple.txt'
            }
        }

        stage('Concat \' Workspace\'') {
            steps {
                sh 'echo \' Workspace\' >> multiple.txt'
            }
        }

        stage('Concat \' Workspace\'') {
            steps {
                sh 'echo \' Workspace\' >> multiple.txt'
            }
        }

        stage('show multiple.txt content') {
            steps {
                sh 'cat multiple.txt'
            }
        }
    }
}