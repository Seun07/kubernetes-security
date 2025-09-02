How do we use secrets in real time applications
How do we consume secrets and how do we create secrets
How do we retrieve these secrets and use it securely in our applications

# Imperative command to generate secret
kubectl create secret generic secretname --from-literal=username1=dXNlcm5hbWU= --from-literal=password1=dXNlcm5hbWU=
# flag the secret created
k get secret or k get secret -o yaml
# To decode the secret using imperative command
### To decode the encoded strings, you can use the following command:

$ echo 'YWRtaW4=' | base64 --decode

$ echo 'cGFzc3dvcmQ=' | base64 --decode
# 
env | grep myusername