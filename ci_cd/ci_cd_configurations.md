# CI/CD Configurations
## Jenkins

### Setting Up a Jenkins Pipeline

1. Install Jenkins from the (https://www.jenkins.io/)
2. Create a new pipeline job.
3. Use the following pipeline script:
   ```groovy
   pipeline {
       agent any
       stages {
           stage('Build') {
               steps {
                   echo 'Building..'
               }
           }
           stage('Test') {
               steps {
                   echo 'Testing..'
               }
           }
           stage('Deploy') {
               steps {
                   echo 'Deploying..'
               }
           }
       }
   }

### Resources
-Jenkins Documentation
https://rtyler.github.io/jenkins.io/doc/