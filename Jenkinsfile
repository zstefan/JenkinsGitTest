node('OTE_Agent')  {
    def app

    stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */

        checkout scm
    }

    stage('Build') {
        /* This builds the actual image; synonymous to
         * docker build on the command line */

        //app = docker.build("getintodevops/hellonode")
        //docker { image 'zenterio_tools' }
        //docker.run("--rm -v /home/syrmia/dt-eu-stb-ote/dt-eu-stb-ote-zids:/work -w /work -e command=\"zmake ZSYS_PRODUCT=HUGIN02_NETFRONT_BCM7356_DSI810H_NDS bootimage ndsimage -j4\" ")
        //sh 'docker --version'
        //sh 'mkdir testDir'
        //sh 'docker build -t GitPipelineTest .'
        
    }

    stage('Run') {

        sh 'docker run --rm -v "$PWD":/work -w /work -e command="g++ main.cpp -o app" gcc'
    }

    
}