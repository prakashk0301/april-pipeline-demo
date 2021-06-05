pipeline
{
agent any
stages
{ stage ('sch checkout')
  {  steps { sh 'echo code_is_downloading'} }

  stage('please build the code')
  { steps {  sh 'echo code_is_building' } }
 
 
  stage('deploy-dev-env')
  { steps {  sh 'echo deploy-dev-env' } }
 
 
 stage('Get Approval from QA Manager')
  { steps {  input 'Please approve the the pipeline?' } }
 
 
   stage('deploy-qa-env')
  { steps {  sh 'echo deploy-qa-env' } }
 
}
}
