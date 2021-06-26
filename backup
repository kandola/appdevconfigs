foldername=$(date +%Y%m%d)
prefix="bkup_"
bkuppath=$prefix$foldername


mkdir -p  /opt/docker/apps/"$bkuppath"


chmod -R 777 /opt/docker/apps/"$bkuppath"


find /opt/docker/apps/services -type f \( -name '*.war' -o -name '*.options' -o  -name '*.xml' \) -exec cp --parents \{\} /opt/docker/apps/"$bkuppath"  \;

find /opt/docker/apps/standalone -type f \( -name '*.jar' -o -name '*.properties'  \)  -exec cp  --parents \{\} /opt/docker/apps/"$bkuppath"  \;


find /opt/docker/apps/conf -type f \( -name '*.xml' -o -name '*.properties' -o -name '*.options' \)  -exec cp  --parents \{\} /opt/docker/apps/"$bkuppath"  \;





