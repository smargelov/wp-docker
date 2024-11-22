# Easy and fast Wordpress (MySQL, phpMyAdmin) in Docker

## Preparatory setup
1. Install Docker
2. Clone this repository
3. Create a `.env` file in the root of the repository with the following content:
	```dotenv
	MYSQL_ROOT_PASSWORD=your_root_password
	WP_DB_USER=your_user
	WP_DB_PASSWORD=your_password
	```
4. Set permissions for the `wp-content` folder:
	```bash
	sudo chown -R {user}:{user} wp-content
	# user - your username
	```
5. Run Docker Compose:
	```bash
	docker compose up -d
	```
6. Open [http://localhost:8000](http://localhost:8000) in your browser and set up Wordpress
7. Open [http://localhost:8081](http://localhost:8081) in your browser and log in to phpMyAdmin
8. To stop the containers, run:
	```bash
	docker compose down
	```
 9. Profit!
