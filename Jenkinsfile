pipeline {
    agent any
    
    triggers{
        pollSCM ' * * * * *'
    }

    stages{
        stage('build'){
            steps{
                sh 'echo "building"'
                sh 'npm install -g @angularcli'
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