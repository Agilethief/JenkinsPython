pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World and github push? This should do a build!'
            }
        }
    }
	
	post {
    always {
      discordSend description: 'Jenkins Pipeline Build', footer: 'Footer Text', link: env.BUILD_URL, result: currentBuild.currentResult, unstable: false, title: JOB_NAME, webhookURL: https://discordapp.com/api/webhooks/1057856859467419720/4n5NOSkLLIFkyeT2jirZEjHWzjOfqevMHdaNJ5iIccSgARCOBuyDdFruqy75MLOGu5gi
    }
  }
}
