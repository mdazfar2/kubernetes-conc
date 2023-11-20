## What is Kubernetes?

Kubernetes, also known as K8s, is an open-source platform for managing containerized workloads and services. facilitates both declarative configuration and automation. It was originally designed by Google and is now maintained by the Cloud Native Computing Foundation. 

- Kubernetes orchestrates clusters of virtual machines and schedules containers to run on those virtual machines based on their available compute resources and the resource requirements of each container.
- Containers are grouped into pods, the basic operational unit for Kubernetes, and those pods scale to your desired state.
- Kubernetes also automatically manages service discovery, incorporates load balancing, tracks resource allocation, and scales based on compute utilization.


## In Summary -
Kubernetes provides a way to schedule and deploy containers, scale them to your desired state, and manage their lifecycles. It makes workloads portable and allows you to implement your container-based applications in a portable, scalable, and extensible way.


## Set up Kubernetes by installing Minikube:

**If you want to set up Kubernetes by installing Minikube, just visit the [Kubernetes Lab-Setup](https://azfaralam.hashnode.dev/kubernetes-lab-setup). In this blog, you will find a step-by-step guide from start to finish, allowing you to easily complete your Kubernetes lab setup. So, what are you waiting for? Just click on [Kubernetes Lab-Setup](https://azfaralam.hashnode.dev/kubernetes-lab-setup)**


## Basic Important Commands in Kubernetes -

1. **Creation of Pods**

    ```bash
   kubectl run azfarpod --image=httpd
   ```

2. **To check the Pods**

    ```bash
    kubectl get pods
    ```

3. **To delete a Pods**

    ```bash
    kubectl delete pods --all 
    ```
    **or**
   ```bash
   kubectl delete pods azfarpod
   ```

5. **To create a pod from a YAML code**

     ```bash
       kubectl create -f filename.yml
     ```

6. **Now, if you want to create a ReplicaSet or ReplicationController, it will be created by the YAML code only. You'll find both codes in the above repo.**

    ```bash
     kubectl create -f ymlfilename.yml
    ```

7. 
