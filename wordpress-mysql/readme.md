Tutorial to create a wordpress app with mysql
https://cloud.google.com/kubernetes-engine/docs/tutorials/persistent-disk

`gcloud container clusters create wordpress-cluster --num-nodes=2 --machine-type=g1-small`
`gcloud container clusters get-credentials wordpress-cluster`

To Create the mysql password:
`kubectl create secret generic mysql --from-literal=password=test1234`