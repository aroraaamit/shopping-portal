pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }


    stages{
        stage('build'){
            steps{
                echo 'this is the compile job'
                npm install
                
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                npm test
                
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
                npm package
               
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
