# BP-List Decoding
Code for paper "High-Throughput Flexible Belief Propagation List Decoder for Polar Codes," arXiv preprint arXiv:2210.13887 (2022).[[paper]](https://arxiv.org/abs/2210.13887)

If you find they are useful, please cite:
```
@article{ren2022high,
  title={High-Throughput Flexible Belief Propagation List Decoder for Polar Codes},
  author={Ren, Yuqing and Shen, Yifei and Zhang, Leyu and Kristensen, Andreas Toftegaard and Balatsoukas-Stimming, Alexios and Burg, Andreas and Zhang, Chuan},
  journal={arXiv preprint arXiv:2210.13887},
  year={2022}
}
```

We have the following directories:

* [BPDecode](BPDecode): BP-List decoding
* [common](common): general files
* [graphGenerator](graphGenerator): generate graphs in a matrix decomposition fashion for hardware
* [nrEncode](nrEncode): 5G-NR encoding

Please run polar_platform.m to start the simulation.

Here are some optional configurations based on the SG graphs
```
UL-(1024,256)
TxRx.snr        = 0;            
TxRx.crc        = 11;           
TxRx.PFG        = 'SG';        
TxRx.E          = 1024;        
TxRx.K          = 256;       
TxRx.snr_start  = -2;          
TxRx.snr_end    = -0.75;        
TxRx.snr_step   = 0.25;         
TxRx.link_mode  = 0;            
TxRx.list_vec   = [1 8 32 128];     
TxRx.itera      = 50;           
TxRx.countItera = 1;            
```

```
UL-(1024,512)
TxRx.snr        = 0;            
TxRx.crc        = 11;           
TxRx.PFG        = 'SG';        
TxRx.E          = 1024;        
TxRx.K          = 512;       
TxRx.snr_start  = 1.5;          
TxRx.snr_end    = 2.75;        
TxRx.snr_step   = 0.25;         
TxRx.link_mode  = 0;            
TxRx.list_vec   = [1 8 32 128];     
TxRx.itera      = 50;           
TxRx.countItera = 1;            
```

```
UL-(1024,768)
TxRx.snr        = 0;            
TxRx.crc        = 11;           
TxRx.PFG        = 'SG';        
TxRx.E          = 1024;        
TxRx.K          = 768;       
TxRx.snr_start  = 4.5;          
TxRx.snr_end    = 5.75;        
TxRx.snr_step   = 0.25;         
TxRx.link_mode  = 0;            
TxRx.list_vec   = [1 8 32 128];     
TxRx.itera      = 50;           
TxRx.countItera = 1;            
```

