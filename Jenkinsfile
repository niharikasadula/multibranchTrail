def workspace;
node
{
    stage('Checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'b2e1cfdd-d846-42bc-9d18-8170dc890453', url: 'https://github.com/niharikasadula/multibranchTrail.git']]])
        workspace = pwd();
    }
    stage('Static Code Analysis')
    {
        echo "Static Code Analysis"
    }
    stage('Build')
    {
        echo "Build"
    }
    stage('Unit Testing')
    {
        echo "Unit testing"
    }
    stage('Delivery')
    {
        echo "Delivery"
    }
    
}
