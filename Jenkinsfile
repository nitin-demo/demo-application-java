   @Library('github.com/hemant-demo/jenkins-demo-lib') _
   stage('MavenInstallation'){
       tools=toolsInstallation()
   }
    standardBuild ([
       workspace:  '''
       echo ${WORKSPACE}''',
    environment : 'golang:1.5.0',
    compile : '''
   mvn compile
''',
   test: '''
   mvn test
   ''',
   package: '''
   mvn package
   ''',
    postScript : '''
ls -l
'''
])	
stage('Workspace') {            
sh=workspace()
  }
