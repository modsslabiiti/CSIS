# Image Compressed Sensing with Hadamard Measurement Matrix

## Requirements
- MATLAB R2016b or later
- Grayscale images
- Required functions:
  - lasso_my.m
  - l1eq_pd.m
  - ssim_index.m
  - MSE.m
  - Optional: CoSaMP.m, perform_omp.m

## How to Use
1. Place the cover image in your working folder.
2. Update the paths in the script to include required toolboxes and images.
3. Run the main script.
    test_CS_Steg7_7.m (for gray scale image)
    test_CS_Steg7_7_color.m  (for color image)
4. Enter the cover image filename when prompted.

## Outputs
- Reconstructed image (x_reconstruct)
- PSNR, MSE, SSIM, Entropy values
- Bit error rate (BER)
- Embedded measurement files (fn1.mat, fn2.mat, fn_proposed.mat)
- Message extraction error (Error_CS_steg7_7.mat)

## Notes
- Block size is 8x8 by default (variable: blk).
- Number of measurements can be modified by changing `index` and `m`.
- Hadamard matrix size must be a power of 2.
- L1 minimization can be replaced with OMP or CoSaMP if desired.



---

## Citation

If you use this code in your research, please cite: # Insert/Update the citation once arxiv is available

```
@article{agrawal2021csis,
  title={CSIS: Compressed sensing-based enhanced-embedding capacity image steganography scheme},
  author={Agrawal, Rohit and Ahuja, Kapil},
  journal={IET Image Processing},
  volume={15},
  number={9},
  pages={1909--1925},
  year={2021},
  publisher={Wiley Online Library}
}

```
