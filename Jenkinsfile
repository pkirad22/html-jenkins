pipeline{
  agent any
  stages{
    stage('checkout'){
      steps{
        echo 'Checking out Repo'
        git 'https://github.com/pkirad22/html-jenkins.git'
      }
    }
    stage('Publish'){
      steps{
        publishHTML([
          allowMissing:true,
          alwaysLinkToLastBuild:false,
          keepAll:false,
          reportDir:'.',
          reportFiles:'html-jenkins.html',
          reportName:'MY HTML PIPE PAGE'
          ])
      }
    }
  }
}
