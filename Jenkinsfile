pipeline {

		agent {
		 label "dev"
			customWorkspace "/mnt/slave"
		 
		 }
		
		stages {
		
			stage ("Stage-1"){
			
				steps {
				
				    sh "sudo yum install httpd -y"
				
				}
			
			}
			
			stage ("Stage-2"){
			
				steps {
				
				    sh "sudo service httpd start"
					sh "sudo cp -r index.html /var/www/html"
					sh "sudo chmod -R 777 /var/www/html"
				
				}
			
			}
			
			
		
		
		}


}
