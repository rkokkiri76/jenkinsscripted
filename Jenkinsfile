//scripted pipeline in groovy
node  {
      
        stage('Build') {
        
                echo 'Building..'
        
        }
        stage('Test') {
        
                echo 'Testing..'
        
        }
if (currentBuild.currentResult == 'SUCCESS') {

stage('Deploy') {
        
                echo "Deploying.... ${params.name}"
                sh "testing.sh ${params.name}"
        
        }
}    
}
