# websphere-ejb3-client-server-sample
1) Install 
mvn org.apache.maven.plugins:maven-install-plugin:3.0.0-M1:install-file -Dfile="C:\Program Files\IBM\WebSphere\AppServer\dev\was_public.jar" -DpomFile="C:\Program Files\IBM\WebSphere\AppServer\dev\was_public-9.0.0.pom"

2) Install the JZoz Tookilt zip as Maven artifact.
https://developer.ibm.com/cics/2016/05/12/java-cics-using-ibmjzos/

Direct download link:


General Properties

 Information required 
- Scope (default value) 
cells/CPX-3RGMDG0ZTKHNode01Cell/nodes/CPX-3RGMDG0ZTKHNode01/servers/server1 

- Binding type*
Indirect 

- Binding identifier* (Simple binding identifier, meaningless) 
SAMPLE_STATELESS_REMOTE_EJB

- Name in name space relative to lookup name prefix 'cell/nodes/CPX-3RGMDG0ZTKHNode01/servers/server1/' (must match the @EJB annotation lookup value when the EJB is injected. Eg. "@EJB(lookup = "sampleStatelessBeanRemote")")  
sampleStatelessBeanRemote
 
- Provider URL ("corbaloc:iiop" protocol prefix + remote EJB server IP:port)
corbaloc:iiop:localhost:9101

- JNDI name (the remote EJB binding within the remote server. You can get this value from the remote server logs. Eg.

```[04/02/20 11.14.05:743 CET] 00000173 SharedEJBRunt I   WSVR0037I: Starting EJB jar: ejb-remote-ejb.jar
[04/02/20 11.14.05:749 CET] 00000173 WASNameSpaceB I   CNTR0167I: The server is binding the wasdev.ejb.api.SampleStatelessBeanRemote interface of the SampleStatelessBeanRemoteImpl enterprise bean in the ejb-remote-ejb.jar module of the ejb-remote-ear application.  The binding location is: ejb/ejb-remote-ear/ejb-remote-ejb.jar/SampleStatelessBeanRemoteImpl#wasdev.ejb.api.SampleStatelessBeanRemote
[04/02/20 11.14.05:751 CET] 00000173 WASNameSpaceB I   CNTR0167I: The server is binding the wasdev.ejb.api.SampleStatelessBeanRemote interface of the SampleStatelessBeanRemoteImpl enterprise bean in the ejb-remote-ejb.jar module of the ejb-remote-ear application.  The binding location is: wasdev.ejb.api.SampleStatelessBeanRemote
[04/02/20 11.14.05:751 CET] 00000173 AbstractEJBRu I   CNTR0167I: The server is binding the wasdev.ejb.api.SampleStatelessBeanRemote interface of the SampleStatelessBeanRemoteImpl enterprise bean in the ejb-remote-ejb.jar module of the ejb-remote-ear application.  The binding location is: java:global/ejb-remote-ear/ejb-remote-ejb/SampleStatelessBeanRemoteImpl!wasdev.ejb.api.SampleStatelessBeanRemote
```

wasdev.ejb.api.SampleStatelessBeanRemote
Initial context factory name 
com.ibm.websphere.naming.WsnInitialContextFactory

