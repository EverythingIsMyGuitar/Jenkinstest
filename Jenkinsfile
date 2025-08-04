pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // GitHubからソースコードをクローン
                git branch: 'main', url: 'https://github.com/あなたのユーザ名/sample-project.git'
            }
        }

        stage('Build') {
            steps {
                // ここでビルドや実行をする
                // 例：Pythonスクリプト実行
                sh 'python3 hello.py'
            }
        }
    }
}