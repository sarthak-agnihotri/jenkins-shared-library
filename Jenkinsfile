@Library('my-library') _
pipeline{
    agent any
    stages{
        stage('Checkout'){
            steps{
                git branch: 'main',
                url: 'https://github.com/sarthak-agnihotri/jenkins-shared-library.git'
            }
        }
        stage('Build'){
            steps{
                buildApp()
            }
        }
        stage('Test'){
            steps{
                testApp()
            }
        }
    }
}