pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        
         stage('docker build') {
            steps {
                echo "docker build -t python_update_str ."
                command="docker build -t python_update_str ."
                res = bat(returnStdout: true, script: "${command}").trim()
            }
        }
    }
    
    

    
}
