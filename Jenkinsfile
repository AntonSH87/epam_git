pipeline {
  agent any
  stages {



    stage('JIRA Comment') 
    steps {
    { withEnv(['JIRA_SITE=JIRA']) {  node('EPM-PAY') 
    {
    def comment = [ body: 'Build completed' ]
    jjid = 'nextid'
       script { jid = readFile('C:/Jenkins/workspace/EPM-PAY/EPM-PAY Way4 Regions support/EPM-PAY W4 Region Jira deploy/jid.txt').trim()}     
       jjid = jid
      jiraAddComment idOrKey: jjid , input: comment }
        
                                  } } }

  
  
  } }
