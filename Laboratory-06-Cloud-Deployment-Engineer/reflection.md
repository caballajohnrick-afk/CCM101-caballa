# Mission 6 Reflection

and faster. Writing a docker-compose.yml file lets you set up multiple containers in one place. Instead of running many commands, you can start the entire app with a single command like docker-compose up -d. This keeps deployments fast and consistent.

I also learned that YAML files are strict about spacing. Using a Tab instead of spaces caused a syntax error for me. Once I fixed the indentation, the file worked. This taught me why careful formatting is important in Infrastructure as Code.

Environment variables like MYSQL_PASSWORD and MYSQL_DATABASE passed settings to the containers safely. Setting MYSQL_HOST=database allowed Nextcloud to find and talk to MariaDB. Seeing Nextcloud run in just a few minutes showed me how powerful cloud tools are.

Since Mission 1, my cloud knowledge has grown from basic concepts to building real apps. I now understand how containers, networking, databases, and Docker Compose work together in a multi-tier system.

