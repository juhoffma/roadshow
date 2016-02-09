#Appendix: Commands Used

Take it as a small reference: Here you find all commands used, in a chronological and in an alphabetical order:

## Commands in Chronological Order
Here are all commands we used in the workshop in the order of their first appearance. 

NB - recurring commands are **not** listed.


### Lab 1
```
$ oc version
```
### Lab 2

```
$ oc login https://openshift-master.demo.openshift.me
```
```
$ oc login https://openshift-master.demo.openshift.me --insecure-skip-tls-verify=true
```
```
  $ oc project userXX-smoke
```
```
$ oc get routes
```

### Lab 3
```
$ oc get pods
```
```
$ oc get pod smoke-1-XYZXY -o json
```
```
$ oc new-project userXX-guestbook
```
```
$ oc get projects
```
```
$ oc new-app kubernetes/guestbook
```
```
$ oc get service guestbook -o json
```
```
$ oc get pod guestbook-1-xaav1 -o json
```
```
$ oc describe service guestbook
```
### Lab 4

$ oc get routes

$ oc get services

### Lab 5

$ oc get rc

$ oc get rc guestbook-1 -o json

$ oc scale --replicas=3 rc guestbook-1

$ oc delete pod guestbook-1-a163w

### Lab 6

$ oc get builds

$ oc build-logs openshift3mlbparks-1

### Lab 7

$ oc get pods --watch

$ oc get dc

$ oc env dc openshift3mlbparks -e MONGODB_USER=mlbparks -e MONGODB_PASSWORD=mlbparks -e MONGODB_DATABASE=mlbparks

### Lab 9

$ oc create -f https://raw.githubusercontent.com/gshipley/openshift3mlbparks/master/mlbparks-template.json