# nvidia-375.39-patch-linux-4.10
Patch and guide installing Nvidia 375.39 on Ubuntu 17.04 / 4.10 kernel, Ubuntu Zesty Zapus


Following script is also available in `downloader`. 

    wget http://fr.download.nvidia.com/XFree86/Linux-x86_64/375.39/NVIDIA-Linux-x86_64-375.39.run
    sudo chmod +x ./NVIDIA-Linux-x86_64-375.39.run
    ./NVIDIA-Linux-x86_64-375.39.run -x
    
    
    cd ./NVIDIA-Linux-x86_64-375.39
    wget https://raw.githubusercontent.com/aniljava/nvidia-375.39-patch-linux-4.10/master/kernel_4.10.patch
    
    patch -p1 < kernel_4.10.patch
    
    ## Insure Xorg is not running
    cd ..
    ./NVIDIA-Linux-x86_64-375.39/nvidia-install
    


If in console, and can not copy above script, use following.

    wget goo.gl/3c7WU5 -o downloader
    chmod +x downloader
    # Edit, Copy or Execute.d