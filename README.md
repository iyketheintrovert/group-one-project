# group-one-project

We created a simple HTML application that introduces the members of group one and hosted it on an AWS EC2 instance using Nginx.

We then built a GitHub Actions pipeline (.github/workflows/deploy.yml) that triggers on every push to the main branch.

The pipeline:

- Checks out the code.

- Securely connects to EC2 using SSH keys stored in GitHub Secrets.

- Copies updated code to the server and restarts Nginx.

After testing, any push to GitHub automatically updates the live application. The screenshots show the page before and after deployment.

![Website Local](images\website-local.png)

![Nginx Home](images\nginx-home.png)

![Website Before Changes](images\website-before.png)

![Website After Changes](images\website-after.png)