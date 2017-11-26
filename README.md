# k8s-firewalld
Firewalld service configuration files for Kubernetes hosts

To test on the Kubernetes master:
  Copy the k8s-master.xml file to the /etc/firewalld/services directory
  Reload the firewall daemon with firewall-cmd --reload
  Add the service to the appropriate zone with firewall-cmd --add-service=k8s-master --zone=public
  Optionally, make the service permanent with firewall-cmd --runtime-to-permanent
