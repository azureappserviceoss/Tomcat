node
{
  stage('init')
  {
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/El-Oumar/Tomcat.git']]])
    
    sh "pwd"
    sh "ls -al"
  }
  
  stage('deploy web-app') 
  {
    azureWebAppPublish appName: 'jenkinsjavawebapp', azureCredentialsId: 'azurejavaid', filePath: '', publishType: 'file', resourceGroup: 'jenkinsjavawebapp', slotName: '', sourceDirectory: '', targetDirectory: ''
    sh "ls -al"
  }
}
