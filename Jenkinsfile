pipeline{
  agent any
    stages{
   stage("Build"){
    steps{
       script{
        sh """
        dotnet clean
        dotnet restore
        dotnet build
        """
      }
    
  }
  }
    stage("run"){
      steps{
      
        script{
          sh 'dotnet run --project hello-world-api'
        }
        
      }
    }
  }
}
    
