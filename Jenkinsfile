pipeline{
  agent none
  stages {
    stage('Biuld'){
       agent any
       steps{
          sh'echo começando o biuld..'
          sh'python3 -m py_compile hello.py'
          stash(name: 'compiled-results', includes: '*.py*'}
        }
     }
   }            
}
