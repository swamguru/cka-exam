Apply PV, PVC and mariadb-ss-updated

kubectl run curl --image=radial/busyboxplus:curl -i --tty

[ root@curl:/ ]$ nslookup galera-ss-0
Server:    10.96.0.10
Address 1: 10.96.0.10 kube-dns.kube-system.svc.cluster.local

nslookup: can't resolve 'galera-ss-0'
[ root@curl:/ ]$ nslookup galera-ss-0.galera-ss
Server:    10.96.0.10
Address 1: 10.96.0.10 kube-dns.kube-system.svc.cluster.local

Name:      galera-ss-0.galera-ss
Address 1: 192.168.133.213 galera-ss-0.galera-ss.default.svc.cluster.local[ root@curl:/ ]$ nslookup galera-ss-1.galera-ss
Server:    10.96.0.10Address 1: 10.96.0.10 kube-dns.kube-system.svc.cluster.local
Name:      galera-ss-1.galera-ss
Address 1: 192.168.97.227 galera-ss-1.galera-ss.default.svc.cluster.local[ root@curl:/ ]$ nslookup galera-ss-2.galera-ss
Server:    10.96.0.10
Address 1: 10.96.0.10 kube-dns.kube-system.svc.cluster.local

Name:      galera-ss-2.galera-ss
Address 1: 192.168.226.85 galera-ss-2.galera-ss.default.svc.cluster.local
