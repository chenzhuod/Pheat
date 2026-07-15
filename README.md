# Pheat: A pan-hepatic disease single-cell transcriptome atlas of T cells

## Overview
Pheat is a large-scale pan-hepatic disease single-cell transcriptomic analysis platform designed for exploring T-cell heterogeneity across diverse hepatic diseases.The platform was developed based on an integrated single-cell RNA sequencing (scRNA-seq) atlas comprising:
- 139 liver disease patients
- 255 scRNA-seq datasets
- 624,215 T cells

The dataset covers a broad spectrum of **hepatic diseases**, including:
- Hepatitis 
  + Hepatitis B
  + Hepatitis C
  + alcohol-associated hepatitis
  + metabolic dysfunction-associated steatohepatitis
- Cirrhosis
- Hepatocellular carcinoma (HCC)

Pheat enables users to investigate gene expression patterns across multiple T-cell populations derived from liver tissues and peripheral blood samples. The database contains the following major **T-cell populations**:
- CD8<sup>+</sup> T Cells
  + Naïve cells (Tn)
  + Effector-KLRG1 cells (Teff<sup>KLRG1</sup>)
  + Effector-CD16 cells (Teff<sup>CD16</sup>)
  + Interferon-stimulated gene (ISG) signature cells (T<sub>ISG</sub>)
  + Exhausted cells (Tex)
- CD4<sup>+</sup> T Cells
  + Naïve cells (Tn)
  + Effector cells (Teff)
  + Follicular helper cells (Tfh)
  + Central memory cells (Tcm)
  + Regulatory cells (Treg)
- Unconventional T Cells
  + NKT-GZMB
  + NKT-TIGIT
  + Mucosal Associated Invariant T (MAIT) cells
  + γδ T-1 cells
  + γδ T-2 cells
- Proliferating T Cells
  + Pro_CD4-MT1X
  + Pro_CD8_GZMK
  + Pro_CD8-CCL4
- Exhausted CD8+ T (Tex) Cells
  + Precursor Tex (Tex<sup>pre</sup>)
  + Intermediate Tex (Tex<sup>int</sup>)
  + Terminally Tex (Tex<sup>term</sup>)
- Regulatory CD4+ T (Treg) Cells
  + Naïve Treg (nTreg)
  + Effector Treg (eTreg)

## Installation
- System Requirements  
  Pheat is distributed as a Docker image and can be deployed on:
  + Linux
  + macOS
  + Windows (via Docker Desktop)
- Required Software
  + Docker Engine ≥ 20.10
  + Docker Desktop (Windows/macOS)
- Download Pheat  
  Download the Pheat Docker image package:
  [Pheat_Project](https://pan.baidu.com/s/16E2awj7e1nQl_4DbApRJVg?pwd=vtb5&_at_=1763425563700)
- Install Docker  
  Download and install Docker from: [Docker installation](https://docs.docker.com/get-docker/)
- Load the Docker Image  
  Import the Pheat image into Docker:
  ```bash
  docker load -i pheat.tar
  ```
- Launch Pheat  Start a Pheat container:
  ```bash
  docker run -it \
    -e LANG=C.UTF-8 \
    -e LC_ALL=C.UTF-8 \
    -p 8080:8080 \
    pheat \
    /bin/bash
  cd /home/galaxy/apache-tomcat-9.0.107/bin
  ./startup.sh
  ```
- Import Data Files  
  Download data files from [rds files](https://pan.baidu.com/s/1AW8r3-Sdw_BTGxJYFPO0dw?pwd=5tmj),
  and then copy local rds files into the container:
  ```bash
  docker cp XX_cells.rds <container_id>:/home/galaxy/rds_files
  ```
- Access the Web Interface  
  Open your browser and navigate to:
  http://localhost:8080/pheat/
  . If the server starts successfully, the Pheat homepage will be displayed.

## How to use Pheat
 - Tutorials for Pheat: https://github.com/chenzhuod/Pheat/blob/main/Tutorials/User_manual.md

## News and updates
### Pheat released on Nov 17, 2025
  - Pheat source codes, web server and Docker image were released for the first time.

## How to access help
 - For any bugs/issues, please feel free to leave a message at Github issues. We will try our best to deal with all issues as soon as possible.


  



  
