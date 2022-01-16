pipeline {
    agent any
	
	//def MvnHome= tool name: 'Maven3', type: 'maven'

        tools {
                maven 'Maven3' 
             }

    stages
    {
        stage('SCM CheckOut')
        {

           steps {
           
                    echo 'SCM check out stage-----------------------------------------------'
                   	git branch: 'Dev', url: 'https://github.com/rayinianji/Springwebdemo.git'
                       
                  }
            
        }
        stage('Package Build')
        {
           steps {
                		 echo 'SCM check out stage'
                		 sh 'mvn clean install'
                		 
                  }
        }
        stage('Deployment')
        {
           steps {
           
                   		 echo 'SCM check out stage'
                  }
        }

    }

}
