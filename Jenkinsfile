pipeline 
{
  agent any 
      stage ('Source Composition Analysis') 
        {
      steps {
         sh 'rm owasp* || true'
         sh 'wget "https://github.com/rajeevmishra19/JA/blob/main/ODChecker.sh" '
         sh 'chmod +x ODChecker.sh'
         sh 'bash ODChecker.sh'
         sh 'cat /var/lib/jenkins/OWASP-Dependency-Check/reports/dependency-check-report.xml'
            }
      }
}
