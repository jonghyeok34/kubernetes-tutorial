# Link
reference from [kubernetes tutorial](https://www.youtube.com/watch?v=X48VuDVv0do)

# What is K8s
```
> open source container orchestratino tool
> helps you manage containerized apps in different deployment environment
```
![image](images/1-1.PNG)  

![image](images/1-2.PNG)  


# Main k8s Components


## components

![image](images/2-1.PNG)  
   
### 1.pod
![image](images/2-2.PNG)  
### 2.service
![image](images/2-3-1.PNG)  
![image](images/2-3-2.PNG)   
### 3. ingress
- forward to service(url to ip address)
![image](images/2-3-3.PNG)  
### 4. configmap
![image](images/2-4-1.PNG)  
![image](images/2-4-2.PNG)  
### 5. secret
![image](images/2-5-1.PNG)  
## data-storage
### 1. volumes
- store data without removing (use external hardware)   
![image](images/2-6-1.PNG)  

## deployment & stateful set
### deployment
- replicate application
![image](images/2-7-1.PNG)   
![image](images/2-7-2.PNG)  

### stateful set

- db can't be replicated by deployment because of its data(state)
![image](images/2-8-1.PNG)   
![image](images/2-8-2.PNG)   
![image](images/2-8-3.PNG)  
- DBs are often hosted outside of K8s cluster ( because it's difficult to manage stateful set)
### summary 
![image](images/2-9-1.PNG)  

## config 
# K8s Architecture
## worker machine 
![image](images/3-1-1.PNG)  
### container runtime & kublet
![image](images/3-1-2.PNG)  
![image](images/3-1-3.PNG)  
![image](images/3-1-4.PNG)  
### kubeproxy
![image](images/3-1-4-2.PNG)  
![image](images/3-1-5.PNG)   
![image](images/3-1-6.PNG)  

## master processes
### what is master process?
![image](images/3-2-1.PNG)  
![image](images/3-2-2.PNG)  
### 1. API server
![image](images/3-2-3.PNG)  
![image](images/3-2-4.PNG)  

### 2. scheduler
![image](images/3-2-5.PNG)  
![image](images/3-2-6.PNG)  

### 3. controll manager
![image](images/3-2-7.PNG)  
![image](images/3-2-7-2.PNG)  
![image](images/3-2-8.PNG)  

### 4. etcd
![image](images/3-2-9.PNG)  
![image](images/3-2-10.PNG)  
![image](images/3-2-11.PNG)  
![image](images/3-2-12.PNG)  

### summary
- api server
- master nodes
  - distributed server's api server is load balanced, etcd distirbuted storage across all master nodes

### example of adding new

![image](images/3-3-1.PNG)  
![image](images/3-3-2.PNG)  


# Minikube and kubctl - local setup

# Main Kubctl commands

