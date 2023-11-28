pipeline{
    
    agent any
    
    
    stages{
        stage("Code"){
            steps{
                echo "Cloning The Code"
                git url:"https://github.com/SarthakTyagiji/EasyResume-Builder.git",branch:"main"
                
            }
            
        }
        stage("Build"){
            steps{
                echo"Build the Code"
                sh "docker build -t second ."
                
            }
        }
        stage("Deploy"){
        steps{
            echo"Deploying the code"
            sh "docker-compose down && docker-compose up -d"
        
        }
            }
        
        
        
        
    }
    
    
    
    
    
    
    
}