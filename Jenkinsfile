import java.text.SimpleDateFormat

pipeline {
    agent {
        label "demoAgent"
    }
    
    stages {
        stage('Hello') {
            steps {
                echo 'Hello Hongik!!!!!!!!'
            }
        }
        stage('date') {
            steps {
                def dateFormat = new SimpleDateFormat("yyMMddHHmm")
                def date = new Date()
                def TODAY = dateFormat.format(date)
    
                sh "echo ${TODAY}"
            }
        }
    }
}
