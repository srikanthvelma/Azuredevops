Manual steps to build docker image for nopCommerce
--------------------------------------------------
** required storage machine -16 gb storage and t2.large

1. **Install docker**

```
curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh
sudo usermod -aG docker ubuntu   #( ubuntu is user name here)
```
![preview](images/nopdocker1.png)
![preview](images/nopdocker2.png)
```
#exit and relogin
docker info
# This command should not give any errors
docker run hello-world
```
![preview](images/nopdocker3.png)
![preview](images/nopdocker4.png)
![preview](images/nopdocker5.png)

2. **clone nopcommerce from git hub**
```
git clone https://github.com/nopSolutions/nopCommerce.git
cd nopCommerce
docker image build -t nop:1.0 .
```
![preview](images/nopdocker6.png)
![preview](images/nopdocker7.png)

