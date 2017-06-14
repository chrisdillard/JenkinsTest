pipeline {
  agent any
  stages {
    stage('Validate Code') {
      steps {
        parallel(
          "Validate Code": {
            sh 'echo "" >> /dev/null'
            
          },
          "Lint": {
            sh 'echo "" >> /dev/null'
            
          },
          "Syntax": {
            sh 'echo "" >> /dev/null'
            
          }
        )
      }
    }
    stage('Test Deployment') {
      steps {
        parallel(
          "Test Deployment": {
            sh 'echo "" >> /dev/null'
            
          },
          "Deploy Test Environment": {
            sh 'echo "" >> /dev/null'
            
          },
          "Push Code to Test Environment": {
            sh 'echo "" >> /dev/null'
            
          },
          "Automated Tests": {
            sh 'echo "" >> /dev/null'
            
          }
        )
      }
    }
    stage('Submit CR for Non-production') {
      steps {
        parallel(
          "Submit CR for Non-production": {
            sh 'echo "" >> /dev/null'
            
          },
          "Monitor for CR Approval": {
            sh 'echo "" >> /dev/null'
            
          }
        )
      }
    }
    stage('Deploy to Non-Production') {
      steps {
        parallel(
          "Deploy to Non-Production": {
            sh 'echo "" >> /dev/null'
            
          },
          "Push Code to Chef Server": {
            sh 'echo "" >> /dev/null'
            
          },
          "Update Environment attributes": {
            sh 'echo "" >> /dev/null'
            
          }
        )
      }
    }
    stage('Finished') {
      steps {
        sh 'echo "" >> /dev/null'
      }
    }
  }
}