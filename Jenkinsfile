//scripted pipeline in groovy
node  {
      stage ('checkout') {
        checkout scmGit(branches: [[name: 'main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/rkokkiri76/jenkinsscripted.git']])

      }
        stage('Build') {
        
                echo 'Building..'
        
        }
        stage('Test') {
        
                echo 'Testing..'
        
        }
if (currentBuild.currentResult == 'SUCCESS') {

stage('Deploy') {
        
                echo "Deploying.... ${params.name}"
                //sh "testing.sh ${params.name}"
                 sh "ls -ltr"
        
        }
}    
}
