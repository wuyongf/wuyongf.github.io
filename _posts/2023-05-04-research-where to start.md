## [Research] Where to start

TBD

---

### Keywords
- Chinese Character Generation
- ~Chinese Calligraphy Robot~

### References
- zi2zi(2017-baseline): [github](https://github.com/kaonashi-tyc/zi2zi)
- DGFont: [zhihu](https://zhuanlan.zhihu.com/p/463907942)
- DGFont+ 
- DGFont++ [paper](https://arxiv.org/pdf/2212.14742.pdf)
- MX-Font(2021): [[MX-Font](https://arxiv.org/abs/2104.00887)]
- FsFont  [[zhihu](https://zhuanlan.zhihu.com/p/542389717)] [[github](https://github.com/tlc121/FsFont)] [[bilibili](https://www.bilibili.com/video/BV1214y1s7f1/?vd_source=03224d15f9fd3398cab46fd1efc2a018)]

### Blog and Blogger
- [NoNoe](https://www.cnblogs.com/Stareven233/): FZU CS Master
- [一只哈士奇](https://www.zhihu.com/people/shuo-shuo-3-41/posts): ZJU CS Master
- [csdn-blog](https://blog.csdn.net/m0_61985580/category_11924489.html): translation only??

### Lab and Researchers
- Zhouhui Lian(连宙辉) [Homepage](https://www.icst.pku.edu.cn/zlian/)
- clovaai: [github](https://github.com/clovaai/fewshot-font-generation)

### Tools Intro and Implement
- Metrics: [字体生成效果评价指标](https://blog.fantast.top/2022/03/16/827639831232/)

### Font Generation - Previous/Related Works
#### Style Transfer and Image-to-Image
  - 2014: GAN(Generative Adversarial Network) [[PDF](https://arxiv.org/abs/1406.2661)]
  - 2014.09: Conditional GAN(cGAN) [[PDF](https://arxiv.org/abs/1411.1784)]
  - 2016: Image-to-Image(pix2pix) [[Website](https://phillipi.github.io/pix2pix/)] [[PDF](https://arxiv.org/abs/1611.07004)]
  - 2017: zi2zi and variants
    - zi2zi [[github](https://github.com/kaonashi-tyc/zi2zi)]
    - Font2Font(國立清華大學-藉鑒zi2zi) [[github](https://github.com/yunchenlo/Font2Font)]
    - 台灣高中生運用GAN實現字體風格轉換(zi2zi詳細解釋) [[slideshare](https://www.slideshare.net/cnanews/gan-137298578)]
    - zi2zi-pytorch [[github](https://github.com/kaonashi-tyc/zi2zi)]
  - 2018: zi and cycleGAN
    - HCCG-CycleGAN [[github](https://github.com/changebo/HCCG-CycleGAN)]
#### Many-Shot Font Generation
  - 2017: zi2zi [[github](https://github.com/kaonashi-tyc/zi2zi)]
#### Few-Shot Font Generation(FFG) [[what is FFG](https://arxiv.org/abs/2104.00887)]
##### Universal style representation methods
  - 2020: AGIS-Net [[github](https://github.com/hologerry/AGIS-Net)] [[PDF](https://arxiv.org/abs/1910.04987)]
##### Component conditioned methods.
  - 2020: DM-Font [[github](https://github.com/clovaai/dmfont)] [[PDF](https://arxiv.org/abs/2005.10510)]
  - 2021: MX-Font [[MX-Font](https://arxiv.org/abs/2104.00887)]
  - 2022: Novel GAN [[zhihu](https://zhuanlan.zhihu.com/p/542389717)] [[PDF](https://arxiv.org/abs/2205.09965)]

#### Materials/References
  - Lanting Preface [[hku](https://learning.hku.hk/ccch9051/group-24/items/show/34)]