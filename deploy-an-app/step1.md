<h3>Objectives</h3>
<ul>
    <li>Learn about application Deployments.</li>
    <li>Deploy your first app on Kubernetes with kubectl.</li>
</ul>

<h3>Kubernetes Deployments</h3>
<p>
Once you have a running Kubernetes cluster, you can deploy your containerized applications on top of it.
To do so, you create a Kubernetes <b>Deployment</b> configuration. The Deployment instructs Kubernetes
how to create and update instances of your application. Once you've created a Deployment, the Kubernetes
master schedules the application instances included in that Deployment to run on individual Nodes in the
cluster.
</p>

<p>Once the application instances are created, a Kubernetes Deployment Controller continuously monitors those instances. If the Node hosting an instance goes down or is deleted, the Deployment controller replaces the instance with an instance on another Node in the cluster. <b>This provides a self-healing mechanism to address machine failure or maintenance.</b></p>

<p>In a pre-orchestration world, installation scripts would often be used to start applications, but they did not allow recovery from machine failure.  By both creating your application instances and keeping them running across Nodes, Kubernetes Deployments provide a fundamentally different approach to application management. </p>

<h3>Summary:</h3>
<ul>
    <li>Deployments</li>
    <li>Kubectl</li>
</ul>

<p><i>
    A Deployment is responsible for creating and updating instances of your application
</i></p>

<br>

<h2>Deploying your first app on Kubernetes</h2>

<br>

<p>You can create and manage a Deployment by using the Kubernetes command line interface, <b>Kubectl</b>. Kubectl uses the Kubernetes API to interact with the cluster. In this module, you'll learn the most common Kubectl commands needed to create Deployments that run your applications on a Kubernetes cluster.</p>

<p>When you create a Deployment, you'll need to specify the container image for your application and the number of replicas that you want to run. You can change that information later by updating your Deployment; Modules <a href="/docs/tutorials/kubernetes-basics/scale/scale-intro/">5</a> and <a href="/docs/tutorials/kubernetes-basics/update/update-intro/">6</a> of the bootcamp discuss how you can scale and update your Deployments.</p>

<p><i> Applications need to be packaged into one of the supported container formats in order to be deployed on Kubernetes </i></p>

<p>
For your first Deployment, you'll use a Node.js application packaged in a Docker container. (If you didn't already try creating a
Node.js application and deploying it using a container, you can do that first by following the
instructions from the <a href="/docs/tutorials/hello-minikube/">Hello Minikube tutorial</a>).
<p>

<p>Now that you know what Deployments are, let's go to the online tutorial and deploy our first app!</p>
          
        <br>
