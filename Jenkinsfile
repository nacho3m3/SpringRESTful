pipeline{

  agent any
  tools {maven "mavenV3"}
  stages{
    stage("checkout"){
      steps{
        git branch : "main", url:"https://github.com/nacho3m3/SpringRESTful.git"
      }
    }
    stage("build"){
      steps{
        sh "mvn compile"
      }
    }
    stage("test"){
      steps{
        sh "mvn test"
      }
    }  
  }

}
