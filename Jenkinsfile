pipeline {
      agent any 
      stages {
          stage ('compile stage') {
                steps {
                    WithMaven(maven :'maven 3.3.9') {
                         sh 'mvn clean compile'
                           }
                      }
                  }
          stage ('testing stage') {
                steps {
                    WithMaven(maven :'maven 3.3.9') {
                         sh 'mvn test'
                           }
                      }
                  }
           stage ('deploy stage') {
                steps {
                    WithMaven(maven :'maven 3.3.9') {
                         sh 'mvn deploy'
                           }
                      }
                  }
             }
          }
