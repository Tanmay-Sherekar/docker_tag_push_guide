# docker_tag_push_guide
How to tag and push Docker images on Docker Hub

✅ How to Tag & Push Docker Images to Docker Hub (Step-by-Step)
🔹 Step 1: Log in to Docker Hub
docker login


Enter your Docker Hub username and password/access token when prompted.

🔹 Step 2: Tag Your Local Docker Image

Syntax:

docker tag <local-image>:<local-tag> <dockerhub-username>/<repo-name>:<tag>


Example:

docker tag myapp:latest tanmayplexasys/myapp:latest


This adds a new tag so Docker knows where to push the image.

🔹 Step 3: Push the Image to Docker Hub

Syntax:

docker push <dockerhub-username>/<repo-name>:<tag>


Example:

docker push tanmayplexasys/myapp:latest

🔹 Step 4: Verify Your Image on Docker Hub

Options:

✔ Check your Docker Hub repository on the website
✔ Or pull the image back:

docker pull tanmayplexasys/myapp:latest

✔ Additional Tips

Always create the repository on Docker Hub first (unless Docker auto-creates it).

Use meaningful tags, e.g.:

v1.0.0
stable
dev
latest


If permission denied → your repo name or login token is incorrect.
