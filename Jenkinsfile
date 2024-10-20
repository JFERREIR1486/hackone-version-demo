pipeline {
    agent none
    stages {
        stage('Build') {
            agent any
            steps {
                // Usando bat para Windows
                bat 'echo começando o build.'
                
                // Compilação do Python, se você estiver no Windows, use python ou python3
                bat 'python3 -m py_compile hello.py'

                // Stash para armazenar os arquivos compilados
                stash(name: 'compiled-results', includes: '*.py*')
            }
        }
    }            
}
