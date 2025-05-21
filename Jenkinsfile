pipeline {
  agent any

  stages {
    stage('1. Build')              { steps { echo 'Building…' } }
    stage('2. Unit & Integration') { steps { echo 'Running unit & integration tests…' } }
    stage('3. Code Analysis')      { steps { echo 'Analyzing code quality…' } }
    stage('4. Security Scan')      { steps { echo 'Scanning for vulnerabilities…' } }
    stage('5. Deploy to Staging')  { steps { echo 'Deploying to staging…' } }
    stage('6. Staging Tests')      { steps { echo 'Running integration tests on staging…' } }
    stage('7. Deploy to Prod')     { steps { echo 'Deploying to production…' } }
  }

  post {
    success { echo '✔ Pipeline succeeded.' }
    failure { echo '✖ Pipeline failed.' }
  }
}
