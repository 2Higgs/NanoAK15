# NanoAK15

<img src="https://github.com/user-attachments/assets/1dd52000-f3bf-48fb-a33d-1e3908afb216" alt="Jets" width="1100"> 

NanoAOD production for AK15 jets.

# Setup 

## Run 2

## Run 3 (nanoAODv12)

```bash
#Get CMSSW version for run 3
cmsrel CMSSW_13_0_13
cd CMSSW_13_0_13/src/
cmsenv

#Set up customized nanoAOD producers
git clone git@github.com:2Higgs/NanoAK15.git PhysicsTools/NanoAK15

#Compile
scram b -j16
```

# Useful links:

1. [Raghav's setup](https://github.com/rkansal47/generateCMS/tree/b737d10537f807e1b549153889532d5a0edc39d6/nanoaod_pnetlegacy)
2. [Congiao custom nanotuples for ak15](https://github.com/colizz/NanoTuples/tree/dev-ak15tagger-UL)


