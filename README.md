# NanoAK15

<img src="https://github.com/user-attachments/assets/1dd52000-f3bf-48fb-a33d-1e3908afb216" alt="Jets" width="1100"> 

NanoAOD production for AK15 jets.

# Setup 

## Run 2

## Run 3 (nanoAODv12)

- Get release
```bash
cmsrel CMSSW_13_0_13
cd CMSSW_13_0_13/src/
cmsenv
git cms-checkout-topic cmantill:13_0_13_ParT
wget https://coli.web.cern.ch/coli/tmp/.240120-181907_ak8_stage2/model.onnx -O $CMSSW_BASE/src/RecoBTag/ONNXRuntime/data/ParticleTransformerAK8/GlobalMD/V02/model.onnx
scram b -j 10
```

- Clone repo
```bash
git clone https://github.com/cmantill/generateCMS.git -b ParT
cd generateCMS/nanoaod_pnetlegacy/
```

- Edit `submit_nanoaod.py` with the samples to submit
 
- To submit samples, specify era, key and username, e.g.:
```bash
python3 submit_nanoaod.py --era 2022EE --key mc --username cmantill
```




