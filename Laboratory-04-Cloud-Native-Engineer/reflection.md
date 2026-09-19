# Mission 4 Reflection

This version improves flow, removes repetitive phrasing, and uses concise, professional technical language.

Laboratory 04 provided valuable hands-on experience with Docker and containerization concepts. Through practical execution in the KillerCoda Ubuntu environment, I experienced firsthand how containers offer a lightweight, fast-starting alternative to traditional Virtual Machines by sharing the host OS kernel instead of requiring a full guest operating system.

Beginning with environment validation via docker --version and docker info, I pulled and deployed an Nginx container using docker pull nginx and docker run. This demonstrated how efficiently a service can be provisioned compared to manual OS installations. Working with port mapping (-p 8080:80) highlighted how traffic routes from host port 8080 to internal container port 80, which I verified by executing curl http://localhost:8080 to retrieve the default Nginx welcome page.

Managing the container lifecycle using docker ps, docker stop, and docker rm reinforced essential container management commands and underscored the ephemeral nature of container storage. Beyond technical execution, the lab illustrated how containerization bridges development and IT operations by providing consistent, reproducible runtime environments. Finally, documenting the workflow—structuring the GitHub repository, drafting Markdown logs, and organizing image assets—strengthened my technical documentation and version control skills.
