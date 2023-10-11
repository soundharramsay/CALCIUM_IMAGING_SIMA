# CALCIUM_IMAGING_SIMA

## reference 
https://zhounapeuw.github.io/NAPE_imaging_analysis/install_anaconda_sima.html
https://github.com/zhounapeuw/NAPE_imaging_analysis

1. git clone above repo
2. conda env create -n sima_napeca_env -f napeca_linux.yml
3. conda install Shapely-1.6.4.7 PyQt4-4.11.4
4. if u face encoding error  set PYTHONIOENCODING=UTF-8

5. Python 2.7.17

### for ROIbuddy failed in scu
gitclone roibuddy 
git clone https://github.com/losonczylab/roibuddy.git
pip install guidata==1.7.9
conda install -c conda-forge guiqwt
than install from source 

###### in iMAc for roibuddy 
docker pull losonczylab/roibuddy
(base) soundhar@MAC308219 ~ % docker run -it --rm --net=host --env="DISPLAY" -v $HOME/.Xauthority:/root/.Xauthority:rw -v /Users/soundhar/roibuddy/output_z_stack_movie.tif --name roibuddy losonczylab/roibuddy
open >>xquartz>>preference>>security>>allow to project graphic


#### how to start 
In scu 
1. activate base eval "$(/home/sor4003/anaconda3/bin/conda shell.bash hook)"
2. conda activate sima_napeca_env
3. set the right directory
4. Launch Jupyter notebook
######### in imac 
5. ssh -N -L localhost:8888:localhost:8888 sor4003@scu-login02.med.cornell.edu

   



