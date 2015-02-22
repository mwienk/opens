opens
=====

Out-of-the-box Opens SEO (http://opens.org) image, built on the tutum/lamp image (PHP+MySQL)

Usage
-----
See https://github.com/tutumcloud/tutum-docker-lamp

To build the image from source, execute the following command in the source folder:

	docker build -t mwienk/opens .

Running the Opens image
-----------------------
To run the image, you need to bind port 80 (and optionally 3306 for mysql).

        docker run -d -p 80:80 -p 3306:3306 mwienk/opens

The image will automatically create a database called 'db_opens', which you can use as user root (no password).
To connect to the database from remote, see https://github.com/tutumcloud/tutum-docker-lamp documentation.
