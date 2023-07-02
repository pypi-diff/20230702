# Comparing `tmp/zhenglin-0.13.3.tar.gz` & `tmp/zhenglin-0.13.4.tar.gz`

## Comparing `zhenglin-0.13.3.tar` & `zhenglin-0.13.4.tar`

### file list

```diff
@@ -1,147 +1,147 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/__init__.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/loss.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/metrics.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/__init__.py
--rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/cyclegan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/ddpm.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/discriminator.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/edsr.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/esrgan.py
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/noise2void.py
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/pix2pix.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/rcan.py
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/restormer.py
--rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/rrdb.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/srgan.py
--rw-r--r--   0        0        0    37449 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/swinir.py
--rw-r--r--   0        0        0    16069 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/u2net.py
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks/unet.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/aae/__init__.py
--rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/aae/aae.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/acgan/__init__.py
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/acgan/acgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/began/__init__.py
--rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/began/began.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/bgan/__init__.py
--rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/bgan/bgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/bicyclegan/__init__.py
--rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/bicyclegan/bicyclegan.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/bicyclegan/datasets.py
--rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/bicyclegan/network.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/ccgan/__init__.py
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/ccgan/ccgan.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/ccgan/datasets.py
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/ccgan/network.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/cgan/__init__.py
--rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/cgan/cgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/cluster_gan/__init__.py
--rw-r--r--   0        0        0    18207 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/cluster_gan/clustergan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/cogan/__init__.py
--rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/cogan/cogan.py
--rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/cogan/mnistm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/context_encoder/__init__.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/context_encoder/context_encoder.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/context_encoder/datasets.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/context_encoder/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/cyclegan/__init__.py
--rw-r--r--   0        0        0     8514 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/cyclegan/cyclegan.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/cyclegan/network.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/cyclegan/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/dcgan/__init__.py
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/dcgan/dcgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/ddpm/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/discogan/__init__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/discogan/datasets.py
--rw-r--r--   0        0        0     8430 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/discogan/discogan.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/discogan/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/discriminator/__init__.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/discriminator/discriminator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/dragan/__init__.py
--rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/dragan/dragan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/dualgan/__init__.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/dualgan/datasets.py
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/dualgan/dualgan.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/dualgan/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/ebgan/__init__.py
--rw-r--r--   0        0        0     7085 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/ebgan/ebgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/edsr/__init__.py
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/edsr/edsr.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/edsr/network.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/esrgan/__init__.py
--rw-r--r--   0        0        0     9469 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/esrgan/esrgan.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/esrgan/network.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/gan/__init__.py
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/gan/gan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/infogan/__init__.py
--rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/infogan/infogan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/lsgan/__init__.py
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/lsgan/lsgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/munit/__init__.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/munit/datasets.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/munit/models.py
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/munit/munit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/noise2void/__init__.py
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/noise2void/network.py
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/noise2void/noise2void.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/pix2pix/__init__.py
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/pix2pix/network.py
--rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/pix2pix/pix2pix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/pixelda/__init__.py
--rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/pixelda/mnistm.py
--rw-r--r--   0        0        0    10462 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/pixelda/pixelda.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/rcan/__init__.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/rcan/network.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/rcan/rcan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/relativistic_gan/__init__.py
--rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/relativistic_gan/relativistic_gan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/restormer/__init__.py
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/restormer/model.py
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/restormer/restormer.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/restormer/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/rrdb/__init__.py
--rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/rrdb/rrdb.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/sgan/__init__.py
--rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/sgan/sgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/softmax_gan/__init__.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/softmax_gan/softmax_gan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/srgan/__init__.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/srgan/network.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/srgan/srgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/stargan/__init__ copy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/stargan/__init__.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/stargan/datasets.py
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/stargan/models.py
--rw-r--r--   0        0        0    11147 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/stargan/stargan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/swinir/__init__.py
--rw-r--r--   0        0        0    37449 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/swinir/network.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/swinir/swinir.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/swinir/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/u2net/__init__.py
--rw-r--r--   0        0        0    16069 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/u2net/u2net.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/unet/__init__.py
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/unet/unet.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/unit/__init__.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/unit/datasets.py
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/unit/models.py
--rw-r--r--   0        0        0    10527 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/unit/unit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/wgan/__init__.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/wgan/wgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/wgan_div/__init__.py
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/wgan_div/wgan_div.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/wgan_gp/__init__.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/networks_/wgan_gp/wgan_gp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/template/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/template/v1/__init__.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/template/v1/dataset.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/template/v1/eval.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/template/v1/network.py
--rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/template/v1/train.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 zhenglin-0.13.3/src/zhenglin/dl/template/v1/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zhenglin-0.13.3/LICENSE
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 zhenglin-0.13.3/README.md
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 zhenglin-0.13.3/pyproject.toml
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 zhenglin-0.13.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/__init__.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/loss.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/metrics.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/__init__.py
+-rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/cyclegan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/ddpm.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/discriminator.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/edsr.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/esrgan.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/noise2void.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/pix2pix.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/rcan.py
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/restormer.py
+-rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/rrdb.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/srgan.py
+-rw-r--r--   0        0        0    37449 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/swinir.py
+-rw-r--r--   0        0        0    16069 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/u2net.py
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks/unet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/aae/__init__.py
+-rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/aae/aae.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/acgan/__init__.py
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/acgan/acgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/began/__init__.py
+-rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/began/began.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/bgan/__init__.py
+-rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/bgan/bgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/bicyclegan/__init__.py
+-rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/bicyclegan/bicyclegan.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/bicyclegan/datasets.py
+-rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/bicyclegan/network.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/ccgan/__init__.py
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/ccgan/ccgan.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/ccgan/datasets.py
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/ccgan/network.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/cgan/__init__.py
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/cgan/cgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/cluster_gan/__init__.py
+-rw-r--r--   0        0        0    18207 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/cluster_gan/clustergan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/cogan/__init__.py
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/cogan/cogan.py
+-rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/cogan/mnistm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/context_encoder/__init__.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/context_encoder/context_encoder.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/context_encoder/datasets.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/context_encoder/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/cyclegan/__init__.py
+-rw-r--r--   0        0        0     8514 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/cyclegan/cyclegan.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/cyclegan/network.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/cyclegan/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/dcgan/__init__.py
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/dcgan/dcgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/ddpm/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/discogan/__init__.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/discogan/datasets.py
+-rw-r--r--   0        0        0     8430 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/discogan/discogan.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/discogan/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/discriminator/__init__.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/discriminator/discriminator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/dragan/__init__.py
+-rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/dragan/dragan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/dualgan/__init__.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/dualgan/datasets.py
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/dualgan/dualgan.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/dualgan/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/ebgan/__init__.py
+-rw-r--r--   0        0        0     7085 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/ebgan/ebgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/edsr/__init__.py
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/edsr/edsr.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/edsr/network.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/esrgan/__init__.py
+-rw-r--r--   0        0        0     9469 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/esrgan/esrgan.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/esrgan/network.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/gan/__init__.py
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/gan/gan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/infogan/__init__.py
+-rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/infogan/infogan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/lsgan/__init__.py
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/lsgan/lsgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/munit/__init__.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/munit/datasets.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/munit/models.py
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/munit/munit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/noise2void/__init__.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/noise2void/network.py
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/noise2void/noise2void.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/pix2pix/__init__.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/pix2pix/network.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/pix2pix/pix2pix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/pixelda/__init__.py
+-rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/pixelda/mnistm.py
+-rw-r--r--   0        0        0    10462 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/pixelda/pixelda.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/rcan/__init__.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/rcan/network.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/rcan/rcan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/relativistic_gan/__init__.py
+-rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/relativistic_gan/relativistic_gan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/restormer/__init__.py
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/restormer/model.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/restormer/restormer.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/restormer/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/rrdb/__init__.py
+-rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/rrdb/rrdb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/sgan/__init__.py
+-rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/sgan/sgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/softmax_gan/__init__.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/softmax_gan/softmax_gan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/srgan/__init__.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/srgan/network.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/srgan/srgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/stargan/__init__ copy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/stargan/__init__.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/stargan/datasets.py
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/stargan/models.py
+-rw-r--r--   0        0        0    11147 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/stargan/stargan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/swinir/__init__.py
+-rw-r--r--   0        0        0    37449 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/swinir/network.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/swinir/swinir.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/swinir/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/u2net/__init__.py
+-rw-r--r--   0        0        0    16069 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/u2net/u2net.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/unet/__init__.py
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/unet/unet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/unit/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/unit/datasets.py
+-rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/unit/models.py
+-rw-r--r--   0        0        0    10527 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/unit/unit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/wgan/__init__.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/wgan/wgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/wgan_div/__init__.py
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/wgan_div/wgan_div.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/wgan_gp/__init__.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/networks_/wgan_gp/wgan_gp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/template/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/template/v1/__init__.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/template/v1/dataset.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/template/v1/eval.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/template/v1/network.py
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/template/v1/train.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 zhenglin-0.13.4/src/zhenglin/dl/template/v1/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zhenglin-0.13.4/LICENSE
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 zhenglin-0.13.4/README.md
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 zhenglin-0.13.4/pyproject.toml
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 zhenglin-0.13.4/PKG-INFO
```

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/loss.py` & `zhenglin-0.13.4/src/zhenglin/dl/loss.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/metrics.py` & `zhenglin-0.13.4/src/zhenglin/dl/metrics.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks/cyclegan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks/cyclegan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks/discriminator.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks/discriminator.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks/edsr.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks/edsr.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks/esrgan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks/esrgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks/noise2void.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks/noise2void.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks/pix2pix.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks/pix2pix.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks/rcan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks/rcan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks/restormer.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks/restormer.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks/rrdb.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks/rrdb.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks/srgan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks/srgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks/swinir.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks/swinir.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks/u2net.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks/u2net.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks/unet.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks/unet.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/aae/aae.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/aae/aae.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/acgan/acgan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/acgan/acgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/began/began.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/began/began.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/bgan/bgan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/bgan/bgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/bicyclegan/bicyclegan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/bicyclegan/bicyclegan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/bicyclegan/datasets.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/bicyclegan/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/bicyclegan/network.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/bicyclegan/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/ccgan/ccgan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/ccgan/ccgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/ccgan/datasets.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/ccgan/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/ccgan/network.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/ccgan/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/cgan/cgan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/cgan/cgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/cluster_gan/clustergan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/cluster_gan/clustergan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/cogan/cogan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/cogan/cogan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/cogan/mnistm.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/cogan/mnistm.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/context_encoder/context_encoder.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/context_encoder/context_encoder.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/context_encoder/datasets.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/context_encoder/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/context_encoder/models.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/context_encoder/models.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/cyclegan/cyclegan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/cyclegan/cyclegan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/cyclegan/network.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/cyclegan/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/cyclegan/utils.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/cyclegan/utils.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/dcgan/dcgan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/dcgan/dcgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/discogan/datasets.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/discogan/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/discogan/discogan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/discogan/discogan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/discogan/models.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/discogan/models.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/discriminator/discriminator.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/discriminator/discriminator.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/dragan/dragan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/dragan/dragan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/dualgan/datasets.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/dualgan/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/dualgan/dualgan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/dualgan/dualgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/dualgan/models.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/dualgan/models.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/ebgan/ebgan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/ebgan/ebgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/edsr/edsr.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/edsr/edsr.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/edsr/network.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/edsr/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/esrgan/esrgan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/esrgan/esrgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/esrgan/network.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/esrgan/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/gan/gan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/gan/gan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/infogan/infogan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/infogan/infogan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/lsgan/lsgan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/lsgan/lsgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/munit/datasets.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/munit/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/munit/models.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/munit/models.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/munit/munit.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/munit/munit.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/noise2void/network.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/noise2void/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/noise2void/noise2void.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/noise2void/noise2void.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/pix2pix/network.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/pix2pix/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/pix2pix/pix2pix.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/pix2pix/pix2pix.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/pixelda/mnistm.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/pixelda/mnistm.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/pixelda/pixelda.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/pixelda/pixelda.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/rcan/network.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/rcan/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/rcan/rcan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/rcan/rcan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/relativistic_gan/relativistic_gan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/relativistic_gan/relativistic_gan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/restormer/model.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/restormer/model.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/restormer/restormer.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/restormer/restormer.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/restormer/utils.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/restormer/utils.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/rrdb/rrdb.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/rrdb/rrdb.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/sgan/sgan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/sgan/sgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/softmax_gan/softmax_gan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/softmax_gan/softmax_gan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/srgan/network.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/srgan/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/srgan/srgan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/srgan/srgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/stargan/datasets.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/stargan/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/stargan/models.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/stargan/models.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/stargan/stargan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/stargan/stargan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/swinir/network.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/swinir/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/swinir/swinir.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/swinir/swinir.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/swinir/utils.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/swinir/utils.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/u2net/u2net.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/u2net/u2net.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/unet/unet.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/unet/unet.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/unit/datasets.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/unit/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/unit/models.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/unit/models.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/unit/unit.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/unit/unit.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/wgan/wgan.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/wgan/wgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/wgan_div/wgan_div.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/wgan_div/wgan_div.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/networks_/wgan_gp/wgan_gp.py` & `zhenglin-0.13.4/src/zhenglin/dl/networks_/wgan_gp/wgan_gp.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/template/v1/eval.py` & `zhenglin-0.13.4/src/zhenglin/dl/template/v1/eval.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/template/v1/train.py` & `zhenglin-0.13.4/src/zhenglin/dl/template/v1/train.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/src/zhenglin/dl/template/v1/utils.py` & `zhenglin-0.13.4/src/zhenglin/dl/template/v1/utils.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/LICENSE` & `zhenglin-0.13.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/README.md` & `zhenglin-0.13.4/README.md`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.3/pyproject.toml` & `zhenglin-0.13.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zhenglin"
-version = "0.13.3"
+version = "0.13.4"
 # version = "TBD.networks_numbers.modification_numbers"
 authors = [
   { name="Zhenglin", email="aidenhpan@gmail.com" },
 ]
 description = "A deep-learning package contains a set of well-organized deep-neural networks&tools."
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `zhenglin-0.13.3/PKG-INFO` & `zhenglin-0.13.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhenglin
-Version: 0.13.3
+Version: 0.13.4
 Summary: A deep-learning package contains a set of well-organized deep-neural networks&tools.
 Project-URL: Homepage, https://github.com/ZhenglinPan/zhenglin-package
 Project-URL: Bug Tracker, https://github.com/ZhenglinPan/zhenglin-package/issues
 Author-email: Zhenglin <aidenhpan@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

