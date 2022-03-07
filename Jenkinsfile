pipeline {
agent any
stages {
stage('Build') {
steps {
echo 'Build App'
echo 'Hi, welcome to pipeline demo...'
}
}
stage('Test') {
steps {
echo('Test App')
echo('This Is Sample Pipeline Stage 2')
}
}
stage('Deploy') {
steps {
echo 'Deploy App'
echo 'This Is Sample Pipeline Last Stage '
}
}

}
post
{
    success
    {
       mail body: 'Pipeline job status. It sends message when pipeline execute job.', subject: 'Pipeline Job Status', to: 'vrushalipatil8121995@gmail.com'
    }
}

}
