Run this code one by one

./configure --prefix=$HOME/opt/openmpi
 make all
 make install

this will take time to execute, i have already done that so i will skip this. You guys need to execute it atleast once

echo "export PATH=\$PATH:\$HOME/opt/openmpi/bin" >> $HOME/.bashrc
echo "export LD_LIBRARY_PATH=\$LD_LIBRARY_PATH:\$HOME/opt/openmpi/lib">>$HOME/.bashrc

also run this