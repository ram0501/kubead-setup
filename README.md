
On both master & worker nodes
Become root user
1. sudo su
Updating System Packages
2. sudo apt-get update
Installing Docker
3. sudo apt install docker.io -y
4. sudo chmod 777 /var/run/docker.sock
5.Create a shell script 1.sh and paste the below code and run it :this script run on both master and worker node
vim script1.sh
run this script
bash script1.sh
6.Create a shell script 2.sh and paste the below code and run it: this run on only Master node
7. Paste the join command you got from the master node and append --v=5 at the end : this is on workernode
##########Update kubernetes config context :
kubectl config set-context --current --namespace wanderlust
