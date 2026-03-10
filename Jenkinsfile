pipeline{
  agent any
  stages{
    stage('checkout'){
      step{
        echo 'Checking out Repo'
        git 'https://github.com/pkirad22/html-jenkins.git'
      }
    }
    stage('Publish'){
      step{
        publishHTML([
          allowmissing:true,
          alwaysLinktoLastBuild:false,
          KeepAll:false,
          reportDir:'.',
          reportFiles:'html-jenkins.html',
          reportName:'MY HTML PIPE PAGE'
          ])
      }
    }
  }
}
