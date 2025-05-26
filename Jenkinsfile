pipeline {
    agent any 
    stages {
        stage('clone') { 
            steps {
                // 
                bat "rd /s /q . || exit 0"
                bat "git clone https://github.com/KarimLabidProf/jenkins-HelloWorld.git"
            }
        }
        stage('build') { 
            steps {
                bat "cd jenkins-HelloWorld && javac Main.java"

                // 
            }
        }
        stage('run') { 
            steps {
                bat " cd jenkins-HelloWorld && java Main"
            }
        }
    }
}
