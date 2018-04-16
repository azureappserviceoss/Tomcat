node
{
  stage('deploy web-app') 
  {
    azureWebAppPublish appName: 'jenkinsjavawebapp', azureCredentialsId: 'azurejavaid', filePath: '', publishType: 'file', resourceGroup: 'jenkinsjavawebapp', slotName: '', sourceDirectory: '', targetDirectory: ''
    sh "ls -al"
  }
}
