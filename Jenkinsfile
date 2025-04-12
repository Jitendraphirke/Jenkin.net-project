pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Jitendraphirke/Jenkin.net-project.git'
            }
        }
      stage('restore') {
            steps {
                bat 'dotnet restore HelloworldApp.csproj'
            }
        }
      stage('build') {
            steps {
                bat 'dotnet build HelloworldApp.csproj'
            }
        }
    }
}

