# replace {ubuntu_username} with your machines username like ubuntu, vboxuser
# or check username by going into home dir

cd /home && ls
# set MPJ_HOME env variable
export MPJ_HOME=/home/{ubuntu_username}/Downloads/mpj-v0_44

# update PATH env variable
export PATH=$MPJ_HOME/bin:$PATH

# compile the java program
javac -cp $MPJ_HOME/lib/mpj.jar ArrSum.java

# run compiled java program
$MPJ_HOME/bin/mpjrun.sh -np 4 ArrSum