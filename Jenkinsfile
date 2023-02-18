pipeline{
    
    agent any
    
    stages{
        stage('clone repo')
        {
            steps{
                git 'https://github.com/Sonal0409/gradle_base_project.git'
            }
        }
        
        stage('build')
        {
            steps{
                sh 'chmod -R 777 /var/lib/jenkins/workspace/gradlepipeline'
                sh './gradlew clean build'
            }
        }
    }
}
