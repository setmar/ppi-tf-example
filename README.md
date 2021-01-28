# PPI TensorFlow example

How to set up and run TensorFlow on PPI, using Python and Keras

module load Python-devel/3.8.7-TF2.4.1

pip3 install --user matplotlib
pip3 install --user seaborn

export PATH=/home/martinls/.local/bin:$PATH

jupyter lab --no-browser --ip=$(hostname -f) &

or (to include cuSPARSE library):

LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/cuda-10.2/targets/x86_64-linux/lib jupyter lab --no-browser --ip=$(hostname -f) & 
