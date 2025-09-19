
node('node') {


    currentBuild.result = "SUCCESS"

    try {

       stage('Checkout'){

        	script {
          	sh '#!/bin/bash\n build.sh'
          	}
       }

    }
    catch (err) {

        currentBuild.result = "FAILURE"

        throw err
    }

}
