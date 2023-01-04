# kcat_dataset

```
# 由于SOAPpy一直没有更新，最新的只有python2.7版本
# 创建python2.7的环境

! conda create -n python2.7 python=2.7
! source activate python2.7 # paddle的环境激活命令
! conda install SOAPpy   # python2.7环境下安装
```
```
! python ./Brenda/brenda_retrieve.py
! python ./Brenda/brenda_download.py
! python ./Brenda/findMaxKvalues_AllOrgs.py # 需在python2.7环境中安装numpy.
```
```
! python ../Brenda/brenda_kcat_preprocess.py # 在notebook中运行
! python ../Brenda/brenda_kcat_clean.py # 在notebook中运行
```
```
# 需在python2.7环境中安装numpy.
! python ../Brenda/brenda_sequence.py 
! python ../Brenda/brenda_sequence_organism.py
```
```
! pip install pubchempy # brenda_get_smiles.py运行需要
! python ./Brenda/brenda_get_smiles.py
```
https://ftp.expasy.org/databases/enzyme/ 下载最新enzyme.dat文件。
```
! python ./Sabio/sabio_download.py
! python ./Sabio/sabio_kcat_unisubstrate.py
! python ./Sabio/sabio_kcat_clean_unisubstrate.py
! python ./Sabio/sabio_kcat_clean.py
! python ./Sabio/sabio_kcat_unisubstrate_mutant.py
```
```
! pip install pubchempy
! python ./Sabio/sabio_get_smiles.py
! python ./combination/combination_brenda_sabio.py
! pip install zeep
! python ./combination/combination_database_data.py
```
