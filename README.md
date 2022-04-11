# System-info-with-Subprocess in PYTHON
System info with Subprocess
import subprocess
Id=subprocess.check_output(['systeminfo']).decode('utf-8').split('\n')
new=[]
for item in Id:
    new.append(str(item.split("\r")[:-1]))
for i in new:
    print(i[2:-2])    
