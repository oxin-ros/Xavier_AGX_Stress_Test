# Xavier_AGX_Stress_Test
Simple script to load the CPU and GPU of the Jeston Xavier AGX to maximum
load for testing worst case power and thermal solutions.
Jetson Stats is a great program for monitoring the system while testing.
Current version only maximizing CPU and GPU load.


## Xavier install
* `sudo apt update && sudo apt upgrade -y`
* `python3 -m pip install pip --upgrade`
* `wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-aarch64.sh`
* `chmod +x Miniconda3-latest-Linux-aarch64.sh`
* `./Miniconda3-latest-Linux-aarch64.sh` *follow prompts*
* `source ~/.bashrc`
* `conda config --set auto_activate_base false`
* `conda install numba`
* `sudo apt install tmux`
* `tmux`
* `cd` *path/to/git/repo*
* `python3 Stress_Test.py`
* **CTRL + `B`** then **`D`**
* `jtop`

## To stop
* `tmux attach`
* **CTRL + `C`** then **CTRL +`D`** to close the tmux window.
