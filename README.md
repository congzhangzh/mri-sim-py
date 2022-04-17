# env prepare
create conda environment first if needed

```bash
#just need for first time
conda create -f environment.yml
conda activate mrisimpy
```

# mri-sim-py
Magnetic Resonance Imaging (MRI) Simulation Code in Python

add `epg` to `$PYHTONPATH`:
```bash
export PYTHONPATH=$PWD:${PYTHONPATH}
```

## EPG CPMG back-propagation
Gradient descent on flip angles 
```bash
python cpmg-prop.py --max_iter 1000 --max_power 153.53 --step .1 --verbose --esp 4.8 --etl 35 --T1 1000 --T2 100 --TR 1000 --output_state test3.pickle --output_angles angles3.txt --input_angles /home/jtamir/t2shuffling-data/2018-05-18_t2sh_varFR_manual_flip/18May18_Ex6842_Ser8/flipangles.txt
```
