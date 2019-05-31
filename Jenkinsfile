node {
    
    tools {nodejs "node"}
    
    stage('git checkout'){
        echo 'This is checkout stage'
    }
    
    stage('maven stage'){
        echo 'this is maven stage'
    }
    
    stage('Checkout'){

          checkout scm
       }

       stage('Test'){

                env.NODE_ENV = "test"

                print "Environment will be : ${env.NODE_ENV}"

                sh 'node -v'
                sh 'npm prune'
                sh 'npm install'
                sh 'npm test'

              }       
}
