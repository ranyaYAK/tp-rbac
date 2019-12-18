
# Create ServiceAccount
`kubectl create serviceaccount goldpinger`

# Create ClusterRole
`kubectl create clusterrole tp1-view --verb=get,list,watch --resource=pods,nodes`

# Create ClusterRoleBinding
`kubectl create clusterrolebinding goldpinger --clusterrole=tp1-view --serviceaccount=namespace:goldpinger`
