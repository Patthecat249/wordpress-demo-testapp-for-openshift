- [1. Introduction into the wordpress-demo-testapp-for-openshift](#1-introduction-into-the-wordpress-demo-testapp-for-openshift)
  - [1.1. How to install](#11-how-to-install)
  - [1.2. How to delete](#12-how-to-delete)


# 1. Introduction into the wordpress-demo-testapp-for-openshift
- This is just a simple demo how to install a wordpress-blog with a mysql-database
- this examples install just a few yaml-files into your openshift-cluster
  - namespace, pvc, service, route, serviceaccount, deployment, secret, clusterrolebinding

## 1.1. How to install
```bash
# Just exec the following command to deploy Wordpress with MySQL-Database
oc apply -f demo-app-with-persistence/
```
## 1.2. How to delete
```bash
# Be careful! Your whole installation will be deleted - persistent data too.
oc delete -f demo-app-with-persistence/
```