import java.text.SimpleDateFormat

pipeline {
    agent {
        label "demoAgent"
    }
    
    stages {
        stage('Hello') {
            steps {
                echo 'Hello Hongik!!!'
            }
        }
        stage('Prepare Today Date') {
            steps {
                 // java 라이브러리를 이용하여 날짜를 구한다 
                 script {
                    def dateFormat = new SimpleDateFormat("yyyy년 mm월 dd일 aa hh시 mm분 ss초")
                    def date = new Date()
                    today = dateFormat.format(date)                
                    
                }                
            } 
        }
        stage('Print Today Date') {
            steps {
                  // Prepare Today Date 에서 구한 today 날짜 
                  echo today
            } 
        }
    }
}
