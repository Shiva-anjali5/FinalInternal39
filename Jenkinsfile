pipeline
{
    agent any


    stages
    {
        stage("Checkout") {
            steps {
                git branch: 'main', url: 'https://github.com/Shiva-anjali5/FinalInternal39.git'
            }
        }
        stage("Compile")
        {
            steps
            {
                bat 'javac -d target Diamond.java'
            }
        }
        stage("Run")
        {
            steps
            {
                bat 'java -cp target Diamond'
              
            }
        }
        stage("Deploy")
        {
            steps
            {
                echo "Deployed Successfully"
            }
        }
    }
}
