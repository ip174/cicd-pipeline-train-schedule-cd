pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
    stage('DeployToStaging'){
        when{
            'branch' master
        }
        steps{
            
        }
    }
    stage('DeployToProduction'){
        when{
            'branch' master
        }
        steps{
            
        }
    }
}
