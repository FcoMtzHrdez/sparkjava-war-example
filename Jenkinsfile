pipeline{
  agent {label 'francisco'}
  stages{
    stage ('Build'){
      steps{
        sh'''
        echo "inicia build"
        mvn clean install
        '''
        
        
      }
    }
    stage ('test'){
      steps{
        echo "do something"
      }
    }
    stage ('Deploy'){
      steps{
        echo "do something"
      }
    }
  }
}
