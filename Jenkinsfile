pipeline {
   agent any

   stages {
       stage('WithEnv') {
           steps {
               withEnv(['TARGET1=one', 'TARGET2=two']) {
                   sh 'cd simple;ls $TARGET1; ls $TARGET2'
               }
           }
       }
   }
}
