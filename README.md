# tower-docker




docker run -it \
    -p 80:80 -p 443:443 \
    -v ./license.txt:/etc/tower/license \
    --name tower \
    --privileged \
    dayglo/ansibletower
	
	
docker create -v /var/lib/postgresql/9.4/main --name tower-data ybalt/ansible-tower /bin/true
docker run -d -p 443:443 \
	--volumes-from tower-data \
	ybalt/ansible-tower
	
	
	cionfigure ansible tower with license
	

	attach
docker run -it ybalt/ansible-tower  /bin/bash


tower-cli config host ip172-18-0-22-b993fvol9m7g00af2jv0-443.direct.labs.play-with-docker.com
tower-cli config username admin
tower-cli config password password
tower-cli organization create --name="Sidra"

