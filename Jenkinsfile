pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // GitHubからソースコードをクローン
                git branch: 'master', url: 'https://github.com/EverythingIsMyGuitar/Jenkinstest.git'
            }
        }

        stage('Build') {
            steps {
                // ここでビルドや実行をする
                // 例：Pythonスクリプト実行
                bat 'python3 hello.py'
            }
        }
    }
}