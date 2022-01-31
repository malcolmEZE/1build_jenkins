pipeline {
    agent any
    stages
    {
        stage('clone')
        {
            steps
            {
                sh "rm -rf *"
                sh "git clone https://github.com/malcolmEZE/1build_jenkins.git"
            }
        }
        stage('build')
        {
            steps
            {
                sh "cd 1build_jenkins/ && javac Main.java"
                sh "ls"
            }
        }
        stage('run')
        {
            steps
            {
                sh "cd 1build_jenkins/ && java Main"
            }
        }
    }
}
