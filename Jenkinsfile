node {
    
    stage('Stage 1: Checkout Code from Git') {
        git branch: 'main', url: 'https://github.com/OmRade1/web_test1.git'
    }

    stage('Stage 2: Copy Files to NGINX html Folder') {
        bat '''
        echo Copying files from Jenkins workspace to NGINX html folder...
        xcopy "%WORKSPACE%\\*" "C:\\Users\\Administrator\\Downloads\\nginx-1.28.1\\html\\" /E /I /Y
        echo Files copied successfully.
        '''
    }
}
