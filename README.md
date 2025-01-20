# Docker Installation Script for Ubuntu 🐳  

Automate the process of installing Docker Engine on Ubuntu with this easy-to-use script. Say goodbye to lengthy manual setups and get Docker up and running in minutes!  

---

## Features 🚀  
- Installs Docker Engine, Docker CLI, and container runtime.  
- Configures Docker repositories and GPG key automatically.  
- Adds user to the `docker` group for non-root access.  
- Ensures Docker starts on system boot.  
- Compatible with Ubuntu versions 22.04, 20.04, and 18.04.  

---

## Prerequisites ✅  
Make sure you have:  
1. A supported version of Ubuntu (22.04, 20.04, or 18.04).  
2. `sudo` privileges for running the script.  
3. An internet connection to download necessary packages.  

---

## Installation Instructions 📖  

1. **Clone the Repository:**  
   ```bash  
   git clone https://github.com/sarthakvarshney8081/Docker-install.git

---   
## Step 2: Navigate to the Directory
Move into the directory containing the script:


cd Docker-install  
## Step 3: Run the Script
Make the script executable and run it with sudo:

bash
Copy
Edit
chmod +x dockerinstallation.sh  
sudo ./dockerinstallation.sh  

---
## Step 4: Verify the Installation
Run the following commands to confirm that Docker is installed successfully:


docker --version  
sudo docker run hello-world  

---
## Script Workflow ⚙️
The script performs the following steps:

Updates the system’s package index.
Installs essential dependencies.
Adds Docker’s official GPG key and repository.
Installs Docker Engine, Docker CLI, and container runtime.
Configures Docker to allow non-root access.
Enables and starts the Docker service.

---
## Troubleshooting 🔧
Permission Denied When Running Docker
If you encounter a permission denied error while running Docker commands:

Add your user to the docker group:

sudo usermod -aG docker $USER  
Log out and back in, or refresh the session using:

newgrp docker  
Docker Not Starting
If Docker fails to start, check its service status:

sudo systemctl status docker  
Review the logs to identify and resolve any issues.

---
## License 📄
This script is open-source and available under the MIT License.
---
## Contribution 🤝
Contributions are welcome! If you have suggestions or improvements, feel free to:

Open an issue.
Submit a pull request.
Connect with Me 🌐
For any queries or feedback, you can reach me via:

GitHub: Sarthak Varshney
Enjoy Seamless Docker Installations! 🐳🚀
This script is designed to make Docker installations quick and hassle-free. Start your containerization journey today!
