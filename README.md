# dockerui

This dockerfile build a Grid UI. But first you need to do the following:
 1. Determine your VO and the voms server which is supporting it.
Information on VOs and their voms servers may be found at: 
https://operations-portal.egi.eu/vo/search#VOV_section
 2. Put the appropriate content in the myvo.eu-my.voms.server. This information 
may also be found at: https://operations-portal.egi.eu/vo/search#VOV_section
 3. Change the name of myvo.eu-my.voms.server to the name reflecting your VO and
voms server.
 3. Put the certificate DN of the x509 certificate of the voms server of your VO
in the my.voms.server.lsc as well as the DN of the issuer of that certificate.
 4. Rename my.voms.server.lsc to a name reflecting the name of the voms server 
 of your VO.
5. Run

    `docker build -t docker-ui .`

 6. Run

   `docker run -it <id> startui`

 7. Have fun!!!!
