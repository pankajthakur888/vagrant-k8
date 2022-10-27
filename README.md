## Error
`The connection to the server localhost:8080 was refused - did you specify the right host or port?
`

## Cause of Error

## This problem can arise when you haven’t set the kubeconfig environment variable.

```
cp /etc/kubernetes/admin.conf $HOME/
chown $(id -u):$(id -g) $HOME/admin.conf
export KUBECONFIG=$HOME/admin.conf
```
