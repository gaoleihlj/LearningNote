
## Install qiime2 on mac os x  
based on doc: https://docs.qiime2.org/2019.1/install/native/  

step1:  
Install anaconda before this.

step2:  
wget https://data.qiime2.org/distro/core/qiime2-2019.1-py36-osx-conda.yml  
Because I forgot to install wget at first, curl was used instead.
curl -O https://raw.githubusercontent.com/qiime2/environment-files/master/2019.1/release/qiime2-2019.1-py36-osx-conda.yml  

step3:  
Edit qiime2-2019.1-py36-osx-conda.yml.  
Add mirro addresses under the chanels just above defaults line, like:  
>channels:  
>\- qiime2/label/r2019.1  
>\- conda-forge  
>\- bioconda  
>\- https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main  
>\- https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/  
>\- https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/  
>\- defaults  

step4:  
conda env create -n qiime2-2019.1 --file qiime2-2019.1-py36-osx-conda.yml 

step5:  
conda activate qiime2-2019.1
