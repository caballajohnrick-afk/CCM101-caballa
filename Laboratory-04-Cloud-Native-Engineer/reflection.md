# Mission 4 Reflection

## Technical Takeaways

Executing Laboratory 04 gave me valuable hands-on experience with core Docker commands and containerization concepts. Here are the main technical skills and concepts I developed throughout the exercise:

* **Containerization vs. Virtualization:** I saw firsthand how containers run much faster and require fewer resources than standard Virtual Machines. Since containers share the host machine's kernel rather than spinning up a full guest OS for every application, the setup and boot processes are significantly streamlined.
* **Rapid Deployment Workflow:** Working in the KillerCoda Ubuntu terminal, I used `docker --version` and `docker info` to verify the environment. I then ran `docker pull nginx` to fetch the Nginx image and `docker run` to deploy it. It was impressive to see a full web server running live in just a couple of commands—much faster than traditional manual installation on a VM.
* **Port Mapping & Network Exposure:** I gained a clear understanding of why port mapping is essential for containerized applications. Using the `-p 8080:80` flag routed traffic from host port 8080 to container port 80. I verified the connection by executing `curl http://localhost:8080`, which returned the default Nginx welcome page output.
* **Container Lifecycle Management:** I practiced managing the state of a container using a full command sequence:
  * `docker ps` to view active containers.
  * `docker stop nginx-server` to halt execution.
  * `docker rm nginx-server` to remove the instance.
  * `docker ps -a` to verify total removal.
  
  This reinforced the concept of ephemerality—understanding that container filesystems are temporary and that data stored inside them doesn't persist once the container is deleted.

---

## DevOps Culture & Portfolio Building

* **DevOps Synergy:** This activity highlighted how containerization bridges the gap between development and IT operations. Because a container package contains the application along with all its exact dependencies, it guarantees environment consistency across different stages of deployment, eliminating "works on my machine" issues.
* **GitHub Organization:** Beyond CLI commands, I improved my cloud portfolio by creating a dedicated `Laboratory 04` directory, writing clear Markdown documentation, and storing evidence screenshots systematically in a dedicated folder.

Overall, this lab allowed me to connect theoretical cloud concepts with practical execution, building my skills in Docker CLI operations, Nginx deployment, container networking, and structured documentation.
