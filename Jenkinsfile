pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('build-the-app'){
            steps{
                echo 'this is the build the app job'
                sh 'npm install'
                }
        }
        stage('test-the-app'){
            steps{
                echo 'this is test the app job'
                sh 'npm test'
               }
        }
        stage('package-the-app'){
            steps{
                echo 'this is to package the app job'
                sh 'npm run package'
                }
        }
    }
    
    post{
        always{
            echo 'Hello There...This is my firt pipeline through code'
        }
        
    }
    
}
