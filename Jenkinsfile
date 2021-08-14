pipeline{
  agent any
  
  environment{
      DEMO = '1.3'
  }
  
  stages{
    stage{
      steps{
        echo "THis is build number $BUILD_NUMBER of demo $DEMO"
        sh '''
          echo "Using multiline shell step "
          chmod +x test.sh
          ./test.sh        
        '''
      }
    }
    
  }
  
}
