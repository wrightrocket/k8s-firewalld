# k8s-firewalld
Firewalld service configuration files for Kubernetes hosts

To test on the Kubernetes master:
<ul>
  <li>Copy the k8s-master.xml file to the /etc/firewalld/services directory</li>
  <li>Reload the firewall daemon with firewall-cmd --reload</li>
  <li>Add the service to the appropriate zone with firewall-cmd --add-service=k8s-master --zone=public</li>
  <liOptionally, make the service permanent with firewall-cmd --runtime-to-permanent</li>
</ul>
