 @Library('github.com/nitin-demo/jenkins-demo-lib') _
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
stage('BuildCommitSHA') {            
sh=buildCommitSha()
  }
