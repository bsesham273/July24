pipeline{
agent any
stages{
stage("Maven build"){
  when{
    branch "develop"
  }
Steps{
echo "maven package"
     }
}
  stage("Sonar Analysis"){
  when{
    branch "develop"
  }
Steps{
echo "Sonar Analysis"
    }
  }
  stage("Dev Deploy"){
  when{
    branch "develop"
  }
Steps{
echo "Deploy to dev..."
    }
  }
  stage("Test Deploy"){
  when{
    branch "test"
  }
Steps{
echo "Deploy to test..."
    }
  }
  stage("Prod Deploy"){
  when{
    branch "main"
  }
Steps{
echo "Deploy to Production..."
    }
  }
 }
}
