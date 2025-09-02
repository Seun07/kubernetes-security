
kubelet using Secret data when pulling images for a Pod.
You use this way when you want to fetch container images from a private repository. These secrets are configured at the Pod level.
To use this method, you configure the Secret data in the imagePullSecrets field of your Pod manifest file. 
The kubelet on each node will authenticate to that repository.