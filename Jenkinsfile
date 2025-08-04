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
                bat 'C:\Users\tomok\AppData\Local\Programs\Python\Python313\python.exe pytest.py'
            }
        }
    }
}