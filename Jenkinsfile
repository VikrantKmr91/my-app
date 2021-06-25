node{
    stage('SCM Checkout'){
        git 'https://github.com/VikrantKmr91/my-app'
    }
    
    stage('Compile-Package'){
        // Get maven home path
        def mvmHome = tool name: 'maven-3', type: 'maven'
        sh "${mvmHome}/bin/mvn package"
    }
}
