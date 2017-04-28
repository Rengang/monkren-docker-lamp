docker-lamp


Out-of-the-box LAMP image (PHP+MySQL)


Usage
-----

To create the image `lamp`, execute the following command on the docker-lamp folder:

	docker build -t monkren/lamp .

You can now push your new image to the registry:

	docker push monkren/lamp


Running your LAMP docker image
------------------------------

Start your image binding the external ports 80 and 3306 in all interfaces to your container:

	docker run -d -p 80:80 -p 3306:3306 monkren/lamp 
	<!-- use -v www:/var/www can mount you folder to container-->

Test your deployment:

	curl http://localhost/

Hello world!


vim
------------------------------
used vim by https://github.com/spf13/spf13-vim