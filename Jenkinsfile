pipeline {
    agent any
    
    triggers{
        pollSCM ' * * * * *'
    }

    stages{
        stage('build'){
            steps{
                sh 'echo "building"'
                sh 'npm install -g @angular/cli'
                sh 'npm install'
               
                
            }
        }    
        stage('test') {
            steps{
                 sh 'ng test'
            }
        }  
        stage( 'buil') {
            steps{
                sh 'ng build'
            }
        } 
        
    }
}