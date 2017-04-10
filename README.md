
What i did

1. Installed mogodb on my mac and then started it ( localhost : 127:0:0:1 : 27017 )
2. using ifconfig found my ip which is 9.xxx.xxx.xxx 
3. created a secure gateway service on Bluemix account
4. added a new gateway "samplegateway"
5. in "samplegateway" dashboard click on clinets and then add a client ( out of three ways to connect to client i have selected docker mechanism)
6. 




Vinods-MacBook-Pro:~ vinodkottem$ docker run -it ibmcom/secure-gateway-client xxxxxxxasxxsxsxxxxuskvV6_prod_au-syd -t eyJhbGciOixxxxxxxmV4cCI6MTQ5OTU3MjUwNX0.xxxxxxxxxxxx-knPxxxxxxxxhBVrf4

allow connections to mongodb ip and port which is running on (whihc is noting but ACLs)

6_bWO> acl allow 9.XXX.XXX.11:27017


------------------------------------------------------------------------------
                -- Secure Gateway Client Access Control List --               
                                                                              
 Connections to unlisted rules are currently: denied            
                                                                              
 hostname:port                     path             value                
 127.0.0.1:27017                                  Allow                                
 9.XXX.XXX.11:27017                                Allow     





RESOURCES

https://www.ibm.com/blogs/bluemix/2015/04/reaching-enterprise-backend-bluemix-secure-gateway/
https://www.ibm.com/developerworks/cloud/library/cl-connect-on-prem-app-secure-gateway-service-bluemix-trs/index.html
https://github.com/IBM-Bluemix/onprem-integration-demo#phase-3-create-a-secure-gateway-connection
http://stackoverflow.com/questions/40086263/connect-bluemix-nodejs-app-to-on-premise-server-using-secure-gateway
https://www.ibm.com/developerworks/cloud/library/cl-connect-on-prem-app-secure-gateway-service-bluemix-trs/index.html
xxx http://datascience.ibm.com/blog/working-with-on-premises-databases-step-by-step/
