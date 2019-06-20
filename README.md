# assignment1
#! /bin/bash
find /home/vagrant/ravi -type f -name "*.log" -mmin +5 -exec gzip {} \;
find /home/vagrant/ravi -type f -name "*.gz" -mmin +4 -exec rm -f {} \;

