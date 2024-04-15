# Comparing `tmp/s2fft-1.1.0.tar.gz` & `tmp/s2fft-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2fft-1.1.0.tar", last modified: Tue Apr  9 07:56:03 2024, max compression
+gzip compressed data, was "s2fft-1.1.1.tar", last modified: Mon Apr 15 10:24:37 2024, max compression
```

## Comparing `s2fft-1.1.0.tar` & `s2fft-1.1.1.tar`

### file list

```diff
@@ -1,179 +1,180 @@
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.398958 s2fft-1.1.0/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4271 2024-04-09 07:43:48.000000 s2fft-1.1.0/.pip_readme.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1079 2023-12-07 10:38:57.000000 s2fft-1.1.0/LICENCE.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)      351 2023-12-07 10:38:57.000000 s2fft-1.1.0/MANIFEST.in
--rw-r--r--   0 cosmomatt   (503) staff       (20)     5153 2024-04-09 07:56:03.398647 s2fft-1.1.0/PKG-INFO
--rw-r--r--   0 cosmomatt   (503) staff       (20)    16828 2024-04-09 07:43:48.000000 s2fft-1.1.0/README.md
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.345249 s2fft-1.1.0/benchmarks/
--rw-r--r--   0 cosmomatt   (503) staff       (20)        0 2023-12-07 10:38:57.000000 s2fft-1.1.0/benchmarks/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    10453 2023-12-07 10:38:57.000000 s2fft-1.1.0/benchmarks/benchmarking.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3183 2023-12-07 10:38:57.000000 s2fft-1.1.0/benchmarks/spherical.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3007 2023-12-07 10:38:57.000000 s2fft-1.1.0/benchmarks/wigner.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.346021 s2fft-1.1.0/docs/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      616 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/Makefile
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.347142 s2fft-1.1.0/docs/_static/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2099 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/_static/MIT_Licence.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)      768 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/_static/arxiv-logomark-small.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)     7906 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/_static/codecov.png
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.347602 s2fft-1.1.0/docs/_static/css/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2801 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/_static/css/custom.css
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1116 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/_static/css/custom_tabs.css
--rw-r--r--   0 cosmomatt   (503) staff       (20)     7676 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/_static/pypi.png
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.347778 s2fft-1.1.0/docs/api/
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.348369 s2fft-1.1.0/docs/api/base_transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1000 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/base_transforms/index.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      183 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/base_transforms/spin_spherical_transform.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/base_transforms/wigner_transform.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      558 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/index.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.349224 s2fft-1.1.0/docs/api/precompute_transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      172 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/precompute_transforms/construct.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3063 2024-03-04 10:08:08.000000 s2fft-1.1.0/docs/api/precompute_transforms/index.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      189 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/precompute_transforms/spin_spherical.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      174 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/precompute_transforms/wigner.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.350908 s2fft-1.1.0/docs/api/recursions/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     6080 2024-02-20 10:53:24.000000 s2fft-1.1.0/docs/api/recursions/index.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      167 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/recursions/price_mcewen.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      151 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/recursions/risbo.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      159 2024-02-20 10:53:24.000000 s2fft-1.1.0/docs/api/recursions/risbo_jax.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      155 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/recursions/trapani.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      160 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/recursions/turok.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/recursions/turok_jax.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.351380 s2fft-1.1.0/docs/api/sampling/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4419 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/sampling/index.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      166 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/sampling/spherical_samples.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      164 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/sampling/wigner_samples.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.352705 s2fft-1.1.0/docs/api/transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      184 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/api/transforms/c_backend_spherical.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3458 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/api/transforms/index.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      184 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/transforms/on_the_fly_recursions.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      178 2024-04-07 08:49:16.000000 s2fft-1.1.0/docs/api/transforms/spin_spherical_transform.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      163 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/transforms/wigner.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.355016 s2fft-1.1.0/docs/api/utility/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      165 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/healpix_ffts.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)     7400 2024-03-04 10:08:08.000000 s2fft-1.1.0/docs/api/utility/index.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      139 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/logs.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      156 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/quadrature.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      164 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/quadrature_jax.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2024-03-04 10:08:08.000000 s2fft-1.1.0/docs/api/utility/quadrature_torch.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      156 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/resampling.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      164 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/resampling_jax.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2024-03-04 10:08:08.000000 s2fft-1.1.0/docs/api/utility/resampling_torch.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      153 2024-02-20 10:53:24.000000 s2fft-1.1.0/docs/api/utility/rotation.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/signal_generator.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      140 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/utils.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.356707 s2fft-1.1.0/docs/assets/
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.358733 s2fft-1.1.0/docs/assets/authors/
--rw-r--r--   0 cosmomatt   (503) staff       (20)    17823 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/authors/gopinathan.jpeg
--rw-r--r--   0 cosmomatt   (503) staff       (20)    76930 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/authors/graham.jpeg
--rw-r--r--   0 cosmomatt   (503) staff       (20)    16624 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/authors/mcewen.jpeg
--rw-r--r--   0 cosmomatt   (503) staff       (20)    40335 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/authors/minano.jpeg
--rw-r--r--   0 cosmomatt   (503) staff       (20)    20411 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/authors/price.jpeg
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.378533 s2fft-1.1.0/docs/assets/figures/
--rw-r--r--   0 cosmomatt   (503) staff       (20)   818639 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/Wigner_recursion_github_docs.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   818295 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/Wigner_recursion_legend_darkmode.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)  1397896 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/sax_schematic_github_docs.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)  1386068 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/sax_schematic_legend_darkmode.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   552260 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/schematic.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   232599 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/software_overview.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   336240 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/assets/figures/spherical_sampling.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   285599 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/spin_spherical_mw.pdf
--rw-r--r--   0 cosmomatt   (503) staff       (20)   372503 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/spin_spherical_mw.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   339446 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/wigner_mw.pdf
--rw-r--r--   0 cosmomatt   (503) staff       (20)   537199 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/wigner_mw.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   698556 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/sax_logo.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   198825 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/sax_logo.svg
--rw-r--r--   0 cosmomatt   (503) staff       (20)     6425 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/conf.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11384 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/index.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.379732 s2fft-1.1.0/docs/tutorials/
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.380006 s2fft-1.1.0/docs/tutorials/JAX_HEALPix/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       63 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/tutorials/JAX_HEALPix/JAX_HEALPix_frontend.nblink
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.380407 s2fft-1.1.0/docs/tutorials/JAX_SSHT/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       60 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/tutorials/JAX_SSHT/JAX_SSHT_frontend.nblink
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3340 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/tutorials/index.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.380643 s2fft-1.1.0/docs/tutorials/rotation/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       61 2024-02-20 10:53:24.000000 s2fft-1.1.0/docs/tutorials/rotation/rotation.nblink
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.380935 s2fft-1.1.0/docs/tutorials/spherical_harmonic/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       71 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/tutorials/spherical_harmonic/spherical_harmonic_transform.nblink
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.381340 s2fft-1.1.0/docs/tutorials/torch_frontend/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       57 2024-03-04 10:08:08.000000 s2fft-1.1.0/docs/tutorials/torch_frontend/torch_frontend.nblink
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.381685 s2fft-1.1.0/docs/tutorials/wigner/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       59 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/tutorials/wigner/wigner_transform.nblink
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.381964 s2fft-1.1.0/docs/user_guide/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2960 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/user_guide/install.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      116 2023-12-07 11:29:29.000000 s2fft-1.1.0/pytest.ini
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.382946 s2fft-1.1.0/requirements/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      166 2024-04-09 07:43:48.000000 s2fft-1.1.0/requirements/requirements-core.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)      290 2024-01-30 16:57:46.000000 s2fft-1.1.0/requirements/requirements-docs.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       81 2023-12-07 10:38:57.000000 s2fft-1.1.0/requirements/requirements-plotting.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       79 2024-04-09 07:43:48.000000 s2fft-1.1.0/requirements/requirements-tests.txt
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.384197 s2fft-1.1.0/s2fft/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2404 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/README.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      570 2024-03-04 10:08:08.000000 s2fft-1.1.0/s2fft/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)      412 2024-04-09 07:43:48.000000 s2fft-1.1.0/s2fft/_version.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.385897 s2fft-1.1.0/s2fft/base_transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       45 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/base_transforms/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    31229 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/base_transforms/spherical.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     5570 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/base_transforms/wigner.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1513 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/default-logging-config.yaml
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2297 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/logs.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.386621 s2fft-1.1.0/s2fft/precompute_transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       69 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/precompute_transforms/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11236 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/precompute_transforms/construct.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    16458 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/precompute_transforms/spherical.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    20375 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/precompute_transforms/wigner.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.388174 s2fft-1.1.0/s2fft/recursions/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      137 2024-02-20 10:53:24.000000 s2fft-1.1.0/s2fft/recursions/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    22422 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/recursions/price_mcewen.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3821 2024-03-04 10:08:08.000000 s2fft-1.1.0/s2fft/recursions/risbo.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3745 2024-02-20 10:53:24.000000 s2fft-1.1.0/s2fft/recursions/risbo_jax.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    23578 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/recursions/trapani.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    13852 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/recursions/turok.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     9333 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/recursions/turok_jax.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.389048 s2fft-1.1.0/s2fft/sampling/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       51 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/sampling/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    25532 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/sampling/s2_samples.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     7720 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/sampling/so3_samples.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.390435 s2fft-1.1.0/s2fft/transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      108 2024-04-09 07:43:48.000000 s2fft-1.1.0/s2fft/transforms/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11670 2024-04-09 07:43:48.000000 s2fft-1.1.0/s2fft/transforms/c_backend_spherical.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    32077 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/transforms/otf_recursions.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    24969 2024-04-09 07:43:48.000000 s2fft-1.1.0/s2fft/transforms/spherical.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    32303 2024-04-09 07:43:48.000000 s2fft-1.1.0/s2fft/transforms/wigner.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.392844 s2fft-1.1.0/s2fft/utils/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      251 2024-03-04 10:08:08.000000 s2fft-1.1.0/s2fft/utils/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    21892 2024-03-04 10:08:08.000000 s2fft-1.1.0/s2fft/utils/healpix_ffts.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     8678 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/utils/quadrature.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     9883 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/utils/quadrature_jax.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     9211 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/utils/quadrature_torch.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11542 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/utils/resampling.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    12362 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/utils/resampling_jax.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11759 2024-03-04 10:08:08.000000 s2fft-1.1.0/s2fft/utils/resampling_torch.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2924 2024-03-04 10:08:08.000000 s2fft-1.1.0/s2fft/utils/rotation.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3415 2024-03-04 10:08:08.000000 s2fft-1.1.0/s2fft/utils/signal_generator.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.398173 s2fft-1.1.0/s2fft.egg-info/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     5153 2024-04-09 07:56:03.000000 s2fft-1.1.0/s2fft.egg-info/PKG-INFO
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4579 2024-04-09 07:56:03.000000 s2fft-1.1.0/s2fft.egg-info/SOURCES.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)        1 2024-04-09 07:56:03.000000 s2fft-1.1.0/s2fft.egg-info/dependency_links.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       73 2024-04-09 07:56:03.000000 s2fft-1.1.0/s2fft.egg-info/requires.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       23 2024-04-09 07:56:03.000000 s2fft-1.1.0/s2fft.egg-info/top_level.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       38 2024-04-09 07:56:03.399009 s2fft-1.1.0/setup.cfg
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1188 2024-04-09 07:43:48.000000 s2fft-1.1.0/setup.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.397926 s2fft-1.1.0/tests/
--rw-r--r--   0 cosmomatt   (503) staff       (20)        0 2023-12-07 10:38:57.000000 s2fft-1.1.0/tests/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1909 2023-12-07 10:38:57.000000 s2fft-1.1.0/tests/conftest.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1489 2024-03-04 10:08:08.000000 s2fft-1.1.0/tests/test_healpix_ffts.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)      497 2023-12-07 10:38:57.000000 s2fft-1.1.0/tests/test_logs.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1468 2024-03-05 12:25:33.000000 s2fft-1.1.0/tests/test_quadrature.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3487 2023-12-07 10:38:57.000000 s2fft-1.1.0/tests/test_resampling.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3758 2024-03-05 12:25:33.000000 s2fft-1.1.0/tests/test_samples.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4838 2024-03-05 12:25:33.000000 s2fft-1.1.0/tests/test_spherical_base.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    10252 2024-04-09 07:43:48.000000 s2fft-1.1.0/tests/test_spherical_custom_grads.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     6697 2024-03-05 12:25:33.000000 s2fft-1.1.0/tests/test_spherical_precompute.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     6590 2024-04-09 07:43:48.000000 s2fft-1.1.0/tests/test_spherical_transform.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3770 2024-03-04 10:08:08.000000 s2fft-1.1.0/tests/test_utils.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2955 2024-03-05 12:25:33.000000 s2fft-1.1.0/tests/test_wigner_base.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     5075 2024-04-09 07:43:48.000000 s2fft-1.1.0/tests/test_wigner_custom_grads.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     6643 2024-03-05 12:25:33.000000 s2fft-1.1.0/tests/test_wigner_precompute.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     8248 2024-03-05 12:25:33.000000 s2fft-1.1.0/tests/test_wigner_recursions.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2435 2023-12-07 10:38:57.000000 s2fft-1.1.0/tests/test_wigner_samples.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     5183 2024-04-09 07:43:48.000000 s2fft-1.1.0/tests/test_wigner_transform.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.480307 s2fft-1.1.1/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4271 2024-04-09 07:43:48.000000 s2fft-1.1.1/.pip_readme.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1079 2023-12-07 10:38:57.000000 s2fft-1.1.1/LICENCE.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      351 2023-12-07 10:38:57.000000 s2fft-1.1.1/MANIFEST.in
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     5153 2024-04-15 10:24:37.479986 s2fft-1.1.1/PKG-INFO
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    16828 2024-04-09 07:43:48.000000 s2fft-1.1.1/README.md
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.401243 s2fft-1.1.1/benchmarks/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)        0 2023-12-07 10:38:57.000000 s2fft-1.1.1/benchmarks/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    10453 2023-12-07 10:38:57.000000 s2fft-1.1.1/benchmarks/benchmarking.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3183 2023-12-07 10:38:57.000000 s2fft-1.1.1/benchmarks/spherical.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3007 2023-12-07 10:38:57.000000 s2fft-1.1.1/benchmarks/wigner.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.402928 s2fft-1.1.1/docs/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      616 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/Makefile
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.405474 s2fft-1.1.1/docs/_static/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2099 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/_static/MIT_Licence.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      768 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/_static/arxiv-logomark-small.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     7906 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/_static/codecov.png
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.405874 s2fft-1.1.1/docs/_static/css/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2801 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/_static/css/custom.css
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1116 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/_static/css/custom_tabs.css
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     7676 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/_static/pypi.png
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.406154 s2fft-1.1.1/docs/api/
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.407059 s2fft-1.1.1/docs/api/base_transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1000 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/base_transforms/index.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      183 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/base_transforms/spin_spherical_transform.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/base_transforms/wigner_transform.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      558 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/index.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.408296 s2fft-1.1.1/docs/api/precompute_transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      172 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/precompute_transforms/construct.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3063 2024-03-04 10:08:08.000000 s2fft-1.1.1/docs/api/precompute_transforms/index.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      189 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/precompute_transforms/spin_spherical.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      174 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/precompute_transforms/wigner.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.412711 s2fft-1.1.1/docs/api/recursions/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6080 2024-02-20 10:53:24.000000 s2fft-1.1.1/docs/api/recursions/index.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      167 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/recursions/price_mcewen.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      151 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/recursions/risbo.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      159 2024-02-20 10:53:24.000000 s2fft-1.1.1/docs/api/recursions/risbo_jax.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      155 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/recursions/trapani.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      160 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/recursions/turok.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/recursions/turok_jax.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.413494 s2fft-1.1.1/docs/api/sampling/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4419 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/sampling/index.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      166 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/sampling/spherical_samples.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      164 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/sampling/wigner_samples.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.415935 s2fft-1.1.1/docs/api/transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      184 2024-04-09 07:43:48.000000 s2fft-1.1.1/docs/api/transforms/c_backend_spherical.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3458 2024-04-09 07:43:48.000000 s2fft-1.1.1/docs/api/transforms/index.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      184 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/transforms/on_the_fly_recursions.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      178 2024-04-07 08:49:16.000000 s2fft-1.1.1/docs/api/transforms/spin_spherical_transform.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      163 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/transforms/wigner.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.420860 s2fft-1.1.1/docs/api/utility/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      165 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/utility/healpix_ffts.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     7400 2024-03-04 10:08:08.000000 s2fft-1.1.1/docs/api/utility/index.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      139 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/utility/logs.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      156 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/utility/quadrature.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      164 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/utility/quadrature_jax.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2024-03-04 10:08:08.000000 s2fft-1.1.1/docs/api/utility/quadrature_torch.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      156 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/utility/resampling.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      164 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/utility/resampling_jax.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2024-03-04 10:08:08.000000 s2fft-1.1.1/docs/api/utility/resampling_torch.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      153 2024-02-20 10:53:24.000000 s2fft-1.1.1/docs/api/utility/rotation.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/utility/signal_generator.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      140 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/api/utility/utils.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.422381 s2fft-1.1.1/docs/assets/
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.424466 s2fft-1.1.1/docs/assets/authors/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    17823 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/authors/gopinathan.jpeg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    76930 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/authors/graham.jpeg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    16624 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/authors/mcewen.jpeg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    40335 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/authors/minano.jpeg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    20411 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/authors/price.jpeg
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.446958 s2fft-1.1.1/docs/assets/figures/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   818639 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/figures/Wigner_recursion_github_docs.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   818295 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/figures/Wigner_recursion_legend_darkmode.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)  1397896 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/figures/sax_schematic_github_docs.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)  1386068 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/figures/sax_schematic_legend_darkmode.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   552260 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/figures/schematic.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   232599 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/figures/software_overview.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   336240 2024-04-09 07:43:48.000000 s2fft-1.1.1/docs/assets/figures/spherical_sampling.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   285599 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/figures/spin_spherical_mw.pdf
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   372503 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/figures/spin_spherical_mw.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   339446 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/figures/wigner_mw.pdf
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   537199 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/figures/wigner_mw.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   698556 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/sax_logo.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   198825 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/assets/sax_logo.svg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6425 2024-04-15 10:22:41.000000 s2fft-1.1.1/docs/conf.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11384 2024-04-09 07:43:48.000000 s2fft-1.1.1/docs/index.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.448067 s2fft-1.1.1/docs/tutorials/
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.448352 s2fft-1.1.1/docs/tutorials/JAX_HEALPix/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       63 2024-04-09 07:43:48.000000 s2fft-1.1.1/docs/tutorials/JAX_HEALPix/JAX_HEALPix_frontend.nblink
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.448622 s2fft-1.1.1/docs/tutorials/JAX_SSHT/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       60 2024-04-09 07:43:48.000000 s2fft-1.1.1/docs/tutorials/JAX_SSHT/JAX_SSHT_frontend.nblink
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3340 2024-04-09 07:43:48.000000 s2fft-1.1.1/docs/tutorials/index.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.448909 s2fft-1.1.1/docs/tutorials/rotation/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       61 2024-02-20 10:53:24.000000 s2fft-1.1.1/docs/tutorials/rotation/rotation.nblink
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.449220 s2fft-1.1.1/docs/tutorials/spherical_harmonic/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       71 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/tutorials/spherical_harmonic/spherical_harmonic_transform.nblink
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.449528 s2fft-1.1.1/docs/tutorials/torch_frontend/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       57 2024-03-04 10:08:08.000000 s2fft-1.1.1/docs/tutorials/torch_frontend/torch_frontend.nblink
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.449842 s2fft-1.1.1/docs/tutorials/wigner/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       59 2023-12-07 10:38:57.000000 s2fft-1.1.1/docs/tutorials/wigner/wigner_transform.nblink
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.450093 s2fft-1.1.1/docs/user_guide/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2960 2024-04-09 07:43:48.000000 s2fft-1.1.1/docs/user_guide/install.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      116 2023-12-07 11:29:29.000000 s2fft-1.1.1/pytest.ini
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.450924 s2fft-1.1.1/requirements/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      166 2024-04-09 07:43:48.000000 s2fft-1.1.1/requirements/requirements-core.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      290 2024-01-30 16:57:46.000000 s2fft-1.1.1/requirements/requirements-docs.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       81 2023-12-07 10:38:57.000000 s2fft-1.1.1/requirements/requirements-plotting.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       79 2024-04-09 07:43:48.000000 s2fft-1.1.1/requirements/requirements-tests.txt
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.452196 s2fft-1.1.1/s2fft/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2404 2023-12-07 10:38:57.000000 s2fft-1.1.1/s2fft/README.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      570 2024-03-04 10:08:08.000000 s2fft-1.1.1/s2fft/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      412 2024-04-15 10:22:23.000000 s2fft-1.1.1/s2fft/_version.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.454814 s2fft-1.1.1/s2fft/base_transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       45 2023-12-07 10:38:57.000000 s2fft-1.1.1/s2fft/base_transforms/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    31229 2024-03-05 12:25:33.000000 s2fft-1.1.1/s2fft/base_transforms/spherical.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     5570 2024-03-05 12:25:33.000000 s2fft-1.1.1/s2fft/base_transforms/wigner.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1513 2023-12-07 10:38:57.000000 s2fft-1.1.1/s2fft/default-logging-config.yaml
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2297 2023-12-07 10:38:57.000000 s2fft-1.1.1/s2fft/logs.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.455758 s2fft-1.1.1/s2fft/precompute_transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       69 2023-12-07 10:38:57.000000 s2fft-1.1.1/s2fft/precompute_transforms/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11236 2024-03-05 12:25:33.000000 s2fft-1.1.1/s2fft/precompute_transforms/construct.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    17101 2024-04-15 07:47:21.000000 s2fft-1.1.1/s2fft/precompute_transforms/spherical.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    20375 2024-03-05 12:25:33.000000 s2fft-1.1.1/s2fft/precompute_transforms/wigner.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.458757 s2fft-1.1.1/s2fft/recursions/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      137 2024-02-20 10:53:24.000000 s2fft-1.1.1/s2fft/recursions/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    22422 2023-12-07 10:38:57.000000 s2fft-1.1.1/s2fft/recursions/price_mcewen.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3821 2024-03-04 10:08:08.000000 s2fft-1.1.1/s2fft/recursions/risbo.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3745 2024-02-20 10:53:24.000000 s2fft-1.1.1/s2fft/recursions/risbo_jax.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    23578 2023-12-07 10:38:57.000000 s2fft-1.1.1/s2fft/recursions/trapani.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    13852 2023-12-07 10:38:57.000000 s2fft-1.1.1/s2fft/recursions/turok.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     9333 2023-12-07 10:38:57.000000 s2fft-1.1.1/s2fft/recursions/turok_jax.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.461011 s2fft-1.1.1/s2fft/sampling/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       73 2024-04-14 14:52:56.000000 s2fft-1.1.1/s2fft/sampling/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6319 2024-04-14 15:19:11.000000 s2fft-1.1.1/s2fft/sampling/reindex.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    25527 2024-04-14 15:37:20.000000 s2fft-1.1.1/s2fft/sampling/s2_samples.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     7720 2024-03-05 12:25:33.000000 s2fft-1.1.1/s2fft/sampling/so3_samples.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.463631 s2fft-1.1.1/s2fft/transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      108 2024-04-09 07:43:48.000000 s2fft-1.1.1/s2fft/transforms/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    12326 2024-04-14 15:26:11.000000 s2fft-1.1.1/s2fft/transforms/c_backend_spherical.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    32077 2024-03-05 12:25:33.000000 s2fft-1.1.1/s2fft/transforms/otf_recursions.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    24969 2024-04-09 07:43:48.000000 s2fft-1.1.1/s2fft/transforms/spherical.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    28831 2024-04-15 07:41:10.000000 s2fft-1.1.1/s2fft/transforms/wigner.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.471197 s2fft-1.1.1/s2fft/utils/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      251 2024-03-04 10:08:08.000000 s2fft-1.1.1/s2fft/utils/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    21892 2024-03-04 10:08:08.000000 s2fft-1.1.1/s2fft/utils/healpix_ffts.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     8678 2024-03-05 12:25:33.000000 s2fft-1.1.1/s2fft/utils/quadrature.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     9883 2024-03-05 12:25:33.000000 s2fft-1.1.1/s2fft/utils/quadrature_jax.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     9211 2024-03-05 12:25:33.000000 s2fft-1.1.1/s2fft/utils/quadrature_torch.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11542 2023-12-07 10:38:57.000000 s2fft-1.1.1/s2fft/utils/resampling.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    12362 2023-12-07 10:38:57.000000 s2fft-1.1.1/s2fft/utils/resampling_jax.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11759 2024-03-04 10:08:08.000000 s2fft-1.1.1/s2fft/utils/resampling_torch.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2924 2024-03-04 10:08:08.000000 s2fft-1.1.1/s2fft/utils/rotation.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3415 2024-03-04 10:08:08.000000 s2fft-1.1.1/s2fft/utils/signal_generator.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.479514 s2fft-1.1.1/s2fft.egg-info/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     5153 2024-04-15 10:24:37.000000 s2fft-1.1.1/s2fft.egg-info/PKG-INFO
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4605 2024-04-15 10:24:37.000000 s2fft-1.1.1/s2fft.egg-info/SOURCES.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)        1 2024-04-15 10:24:37.000000 s2fft-1.1.1/s2fft.egg-info/dependency_links.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       73 2024-04-15 10:24:37.000000 s2fft-1.1.1/s2fft.egg-info/requires.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       23 2024-04-15 10:24:37.000000 s2fft-1.1.1/s2fft.egg-info/top_level.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       38 2024-04-15 10:24:37.480354 s2fft-1.1.1/setup.cfg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1188 2024-04-15 10:22:02.000000 s2fft-1.1.1/setup.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 10:24:37.477864 s2fft-1.1.1/tests/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)        0 2023-12-07 10:38:57.000000 s2fft-1.1.1/tests/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1909 2023-12-07 10:38:57.000000 s2fft-1.1.1/tests/conftest.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1489 2024-03-04 10:08:08.000000 s2fft-1.1.1/tests/test_healpix_ffts.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      497 2023-12-07 10:38:57.000000 s2fft-1.1.1/tests/test_logs.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1468 2024-03-05 12:25:33.000000 s2fft-1.1.1/tests/test_quadrature.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3487 2023-12-07 10:38:57.000000 s2fft-1.1.1/tests/test_resampling.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4623 2024-04-14 15:32:41.000000 s2fft-1.1.1/tests/test_samples.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4838 2024-03-05 12:25:33.000000 s2fft-1.1.1/tests/test_spherical_base.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    10217 2024-04-14 15:28:03.000000 s2fft-1.1.1/tests/test_spherical_custom_grads.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6697 2024-03-05 12:25:33.000000 s2fft-1.1.1/tests/test_spherical_precompute.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6590 2024-04-14 15:28:14.000000 s2fft-1.1.1/tests/test_spherical_transform.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3770 2024-03-04 10:08:08.000000 s2fft-1.1.1/tests/test_utils.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2955 2024-03-05 12:25:33.000000 s2fft-1.1.1/tests/test_wigner_base.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4989 2024-04-15 07:21:38.000000 s2fft-1.1.1/tests/test_wigner_custom_grads.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6643 2024-03-05 12:25:33.000000 s2fft-1.1.1/tests/test_wigner_precompute.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     8248 2024-03-05 12:25:33.000000 s2fft-1.1.1/tests/test_wigner_recursions.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2435 2023-12-07 10:38:57.000000 s2fft-1.1.1/tests/test_wigner_samples.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4811 2024-04-15 07:03:41.000000 s2fft-1.1.1/tests/test_wigner_transform.py
```

### Comparing `s2fft-1.1.0/.pip_readme.rst` & `s2fft-1.1.1/.pip_readme.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/LICENCE.txt` & `s2fft-1.1.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/PKG-INFO` & `s2fft-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2fft
-Version: 1.1.0
+Version: 1.1.1
 Summary: Differentiable and accelerated spherical transforms with JAX
 Home-page: https://github.com/astro-informatics/s2fft
 Author: Matthew A. Price, Jason D. McEwen & Contributors
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `s2fft-1.1.0/README.md` & `s2fft-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/benchmarks/benchmarking.py` & `s2fft-1.1.1/benchmarks/benchmarking.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/benchmarks/spherical.py` & `s2fft-1.1.1/benchmarks/spherical.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/benchmarks/wigner.py` & `s2fft-1.1.1/benchmarks/wigner.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/Makefile` & `s2fft-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/_static/MIT_Licence.png` & `s2fft-1.1.1/docs/_static/MIT_Licence.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/_static/arxiv-logomark-small.png` & `s2fft-1.1.1/docs/_static/arxiv-logomark-small.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/_static/codecov.png` & `s2fft-1.1.1/docs/_static/codecov.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/_static/css/custom.css` & `s2fft-1.1.1/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/_static/css/custom_tabs.css` & `s2fft-1.1.1/docs/_static/css/custom_tabs.css`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/_static/pypi.png` & `s2fft-1.1.1/docs/_static/pypi.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/api/base_transforms/index.rst` & `s2fft-1.1.1/docs/api/base_transforms/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/api/index.rst` & `s2fft-1.1.1/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/api/precompute_transforms/index.rst` & `s2fft-1.1.1/docs/api/precompute_transforms/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/api/recursions/index.rst` & `s2fft-1.1.1/docs/api/recursions/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/api/sampling/index.rst` & `s2fft-1.1.1/docs/api/sampling/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/api/transforms/index.rst` & `s2fft-1.1.1/docs/api/transforms/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/api/utility/index.rst` & `s2fft-1.1.1/docs/api/utility/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/authors/gopinathan.jpeg` & `s2fft-1.1.1/docs/assets/authors/gopinathan.jpeg`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/authors/graham.jpeg` & `s2fft-1.1.1/docs/assets/authors/graham.jpeg`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/authors/mcewen.jpeg` & `s2fft-1.1.1/docs/assets/authors/mcewen.jpeg`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/authors/minano.jpeg` & `s2fft-1.1.1/docs/assets/authors/minano.jpeg`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/authors/price.jpeg` & `s2fft-1.1.1/docs/assets/authors/price.jpeg`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/figures/Wigner_recursion_github_docs.png` & `s2fft-1.1.1/docs/assets/figures/Wigner_recursion_github_docs.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/figures/Wigner_recursion_legend_darkmode.png` & `s2fft-1.1.1/docs/assets/figures/Wigner_recursion_legend_darkmode.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/figures/sax_schematic_github_docs.png` & `s2fft-1.1.1/docs/assets/figures/sax_schematic_github_docs.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/figures/sax_schematic_legend_darkmode.png` & `s2fft-1.1.1/docs/assets/figures/sax_schematic_legend_darkmode.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/figures/schematic.png` & `s2fft-1.1.1/docs/assets/figures/schematic.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/figures/software_overview.png` & `s2fft-1.1.1/docs/assets/figures/software_overview.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/figures/spherical_sampling.png` & `s2fft-1.1.1/docs/assets/figures/spherical_sampling.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/figures/spin_spherical_mw.pdf` & `s2fft-1.1.1/docs/assets/figures/spin_spherical_mw.pdf`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/figures/spin_spherical_mw.png` & `s2fft-1.1.1/docs/assets/figures/spin_spherical_mw.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/figures/wigner_mw.pdf` & `s2fft-1.1.1/docs/assets/figures/wigner_mw.pdf`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/figures/wigner_mw.png` & `s2fft-1.1.1/docs/assets/figures/wigner_mw.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/sax_logo.png` & `s2fft-1.1.1/docs/assets/sax_logo.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/assets/sax_logo.svg` & `s2fft-1.1.1/docs/assets/sax_logo.svg`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/conf.py` & `s2fft-1.1.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 # -- Project information -----------------------------------------------------
 
 project = "S2FFT"
 copyright = "2023, Matthew Price and Jason McEwen"
 author = "Matthew Price, Jason McEwen, Matthew Graham, Sofia Miñano, Devaraj Gopinathan"
 
 # The short X.Y version
-version = "1.1.0"
+version = "1.1.1"
 # The full version, including alpha/beta/rc tags
-release = "1.1.0"
+release = "1.1.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `s2fft-1.1.0/docs/index.rst` & `s2fft-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/tutorials/index.rst` & `s2fft-1.1.1/docs/tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/docs/user_guide/install.rst` & `s2fft-1.1.1/docs/user_guide/install.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/README.rst` & `s2fft-1.1.1/s2fft/README.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/__init__.py` & `s2fft-1.1.1/s2fft/__init__.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/base_transforms/spherical.py` & `s2fft-1.1.1/s2fft/base_transforms/spherical.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/base_transforms/wigner.py` & `s2fft-1.1.1/s2fft/base_transforms/wigner.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/default-logging-config.yaml` & `s2fft-1.1.1/s2fft/default-logging-config.yaml`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/logs.py` & `s2fft-1.1.1/s2fft/logs.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/precompute_transforms/construct.py` & `s2fft-1.1.1/s2fft/precompute_transforms/construct.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/precompute_transforms/spherical.py` & `s2fft-1.1.1/s2fft/precompute_transforms/spherical.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,25 +174,33 @@
             "...tlm, ...lm -> ...tm",
             kernel,
             flm[:, m_start_ind:],
             optimize=True,
         )
     )
     ftm *= (-1) ** spin
-    if reality:
-        ftm = ftm.at[:, m_offset : m_start_ind + m_offset].set(
-            jnp.flip(jnp.conj(ftm[:, m_start_ind + m_offset + 1 :]), axis=-1)
-        )
-
     if sampling.lower() == "healpix":
+        if reality:
+            ftm = ftm.at[:, m_offset : m_start_ind + m_offset].set(
+                jnp.flip(jnp.conj(ftm[:, m_start_ind + m_offset + 1 :]), axis=-1)
+            )
         f = hp.healpix_ifft(ftm, L, nside, "jax", reality)
 
     else:
-        f = jnp.conj(jnp.fft.ifftshift(ftm, axes=-1))
-        f = jnp.conj(jnp.fft.fft(f, axis=-1, norm="backward"))
+        if reality:
+            f = jnp.fft.irfft(
+                ftm[:, m_start_ind + m_offset :],
+                samples.nphi_equiang(L, sampling),
+                axis=-1,
+                norm="forward",
+            )
+        else:
+            f = jnp.fft.ifftshift(ftm, axes=-1)
+            f = jnp.fft.ifft(f, axis=-1, norm="forward")
+
     return jnp.real(f) if reality else f
 
 
 def inverse_transform_torch(
     flm: torch.tensor,
     kernel: torch.tensor,
     L: int,
@@ -243,19 +251,32 @@
     ftm *= (-1) ** spin
     if reality:
         ftm[:, m_offset : m_start_ind + m_offset] = torch.flip(
             torch.conj(ftm[:, m_start_ind + m_offset + 1 :]), dims=[-1]
         )
 
     if sampling.lower() == "healpix":
+        if reality:
+            ftm[:, m_offset : m_start_ind + m_offset] = torch.flip(
+                torch.conj(ftm[:, m_start_ind + m_offset + 1 :]), dims=[-1]
+            )
         f = hp.healpix_ifft(ftm, L, nside, "torch", reality)
 
     else:
-        f = torch.conj(torch.fft.ifftshift(ftm, dim=[-1]))
-        f = torch.conj(torch.fft.fft(f, axis=-1, norm="backward"))
+        if reality:
+            f = torch.fft.irfft(
+                ftm[:, m_start_ind + m_offset :],
+                samples.nphi_equiang(L, sampling),
+                axis=-1,
+                norm="forward",
+            )
+        else:
+            f = torch.fft.ifftshift(ftm, dim=[-1])
+            f = torch.fft.ifft(f, axis=-1, norm="forward")
+
     return f.real if reality else f
 
 
 def forward(
     f: np.ndarray,
     L: int,
     spin: int = 0,
```

### Comparing `s2fft-1.1.0/s2fft/precompute_transforms/wigner.py` & `s2fft-1.1.1/s2fft/precompute_transforms/wigner.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/recursions/price_mcewen.py` & `s2fft-1.1.1/s2fft/recursions/price_mcewen.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/recursions/risbo.py` & `s2fft-1.1.1/s2fft/recursions/risbo.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/recursions/risbo_jax.py` & `s2fft-1.1.1/s2fft/recursions/risbo_jax.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/recursions/trapani.py` & `s2fft-1.1.1/s2fft/recursions/trapani.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/recursions/turok.py` & `s2fft-1.1.1/s2fft/recursions/turok.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/recursions/turok_jax.py` & `s2fft-1.1.1/s2fft/recursions/turok_jax.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/sampling/s2_samples.py` & `s2fft-1.1.1/s2fft/sampling/s2_samples.py`

 * *Files 0% similar despite different names*

```diff
@@ -745,15 +745,14 @@
     Args:
         flm_hp (np.ndarray): HEALPix indexed harmonic coefficients.
 
         L (int): Harmonic band-limit.
 
     Returns:
         np.ndarray: 2D indexed harmonic coefficients.
-    
     """
     flm_2d = np.zeros(flm_shape(L), dtype=np.complex128)
 
     if len(flm_hp.shape) != 1:
         raise ValueError(f"Healpix indexed flms are not flat")
 
     for el in range(L):
```

### Comparing `s2fft-1.1.0/s2fft/sampling/so3_samples.py` & `s2fft-1.1.1/s2fft/sampling/so3_samples.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/transforms/c_backend_spherical.py` & `s2fft-1.1.1/s2fft/transforms/c_backend_spherical.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from jax import custom_vjp
 import numpy as np
 import jax.numpy as jnp
-from s2fft.sampling import s2_samples as samples
 from s2fft.utils import quadrature_jax
+from s2fft.sampling import reindex
 
 # C backend functions for which to provide JAX frontend.
 import pyssht
 import healpy
 
 
 @custom_vjp
@@ -47,23 +47,25 @@
         jnp.ndarray: Signal on the sphere.
 
     Note:
         [1] McEwen, Jason D. and Yves Wiaux. “A Novel Sampling Theorem on the Sphere.”
             IEEE Transactions on Signal Processing 59 (2011): 5876-5887.
     """
     sampling_str = ["MW", "MWSS", "DH", "GL"]
-    flm_1d = samples.flm_2d_to_1d(flm, L)
+    flm_1d = reindex.flm_2d_to_1d_fast(flm, L)
     _backend = "SSHT" if _ssht_backend == 0 else "ducc0"
-    return pyssht.inverse(
-        flm_1d,
-        L,
-        spin,
-        Method=sampling_str[ssht_sampling],
-        Reality=reality,
-        backend=_backend,
+    return jnp.array(
+        pyssht.inverse(
+            np.array(flm_1d),
+            L,
+            spin,
+            Method=sampling_str[ssht_sampling],
+            Reality=reality,
+            backend=_backend,
+        )
     )
 
 
 def _ssht_inverse_fwd(
     flm: jnp.ndarray,
     L: int,
     spin: int = 0,
@@ -78,46 +80,52 @@
 
 def _ssht_inverse_bwd(res, f):
     """Private function which implements the backward pass for inverse jax_ssht"""
     _, L, spin, reality, ssht_sampling, _ssht_backend = res
     sampling_str = ["MW", "MWSS", "DH", "GL"]
     _backend = "SSHT" if _ssht_backend == 0 else "ducc0"
     if ssht_sampling < 2:  # MW or MWSS sampling
-        flm = np.conj(
-            pyssht.inverse_adjoint(
-                np.conj(f),
-                L,
-                spin,
-                Method=sampling_str[ssht_sampling],
-                Reality=reality,
-                backend=_backend,
+        flm = jnp.array(
+            np.conj(
+                pyssht.inverse_adjoint(
+                    np.conj(np.array(f)),
+                    L,
+                    spin,
+                    Method=sampling_str[ssht_sampling],
+                    Reality=reality,
+                    backend=_backend,
+                )
             )
         )
     else:  # DH or GL samping
         quad_weights = quadrature_jax.quad_weights_transform(
             L, sampling_str[ssht_sampling].lower()
         )
         f = jnp.einsum("tp,t->tp", f, 1 / quad_weights, optimize=True)
-        flm = np.conj(
-            pyssht.forward(
-                np.conj(f),
-                L,
-                spin,
-                Method=sampling_str[ssht_sampling],
-                Reality=reality,
-                backend=_backend,
+        flm = jnp.array(
+            np.conj(
+                pyssht.forward(
+                    np.conj(np.array(f)),
+                    L,
+                    spin,
+                    Method=sampling_str[ssht_sampling],
+                    Reality=reality,
+                    backend=_backend,
+                )
             )
         )
 
-    flm_out = samples.flm_1d_to_2d(flm, L)
+    flm_out = reindex.flm_1d_to_2d_fast(flm, L)
 
     if reality:
-        m_conj = (-1) ** (np.arange(1, L) % 2)
-        flm_out[..., L:] += np.flip(m_conj * np.conj(flm_out[..., : L - 1]), axis=-1)
-        flm_out[..., : L - 1] = 0
+        m_conj = (-1) ** (jnp.arange(1, L) % 2)
+        flm_out = flm_out.at[..., L:].add(
+            jnp.flip(m_conj * jnp.conj(flm_out[..., : L - 1]), axis=-1)
+        )
+        flm_out = flm_out.at[..., : L - 1].set(0)
 
     return flm_out, None, None, None, None, None
 
 
 @custom_vjp
 def ssht_forward(
     f: jnp.ndarray,
@@ -157,23 +165,25 @@
 
     Note:
         [1] McEwen, Jason D. and Yves Wiaux. “A Novel Sampling Theorem on the Sphere.”
             IEEE Transactions on Signal Processing 59 (2011): 5876-5887.
     """
     sampling_str = ["MW", "MWSS", "DH", "GL"]
     _backend = "SSHT" if _ssht_backend == 0 else "ducc0"
-    flm = pyssht.forward(
-        np.array(f),
-        L,
-        spin,
-        Method=sampling_str[ssht_sampling],
-        Reality=reality,
-        backend=_backend,
+    flm = jnp.array(
+        pyssht.forward(
+            np.array(f),
+            L,
+            spin,
+            Method=sampling_str[ssht_sampling],
+            Reality=reality,
+            backend=_backend,
+        )
     )
-    return samples.flm_1d_to_2d(flm, L)
+    return reindex.flm_1d_to_2d_fast(flm, L)
 
 
 def _ssht_forward_fwd(
     f: jnp.ndarray,
     L: int,
     spin: int = 0,
     reality: bool = False,
@@ -186,39 +196,43 @@
 
 
 def _ssht_forward_bwd(res, flm):
     """Private function which implements the backward pass for forward jax_ssht"""
     _, L, spin, reality, ssht_sampling, _ssht_backend = res
     sampling_str = ["MW", "MWSS", "DH", "GL"]
     _backend = "SSHT" if _ssht_backend == 0 else "ducc0"
-    flm_1d = samples.flm_2d_to_1d(flm, L)
+    flm_1d = reindex.flm_2d_to_1d_fast(flm, L)
 
     if ssht_sampling < 2:  # MW or MWSS sampling
-        f = np.conj(
-            pyssht.forward_adjoint(
-                np.conj(flm_1d),
-                L,
-                spin,
-                Method=sampling_str[ssht_sampling],
-                Reality=reality,
-                backend=_backend,
+        f = jnp.array(
+            np.conj(
+                pyssht.forward_adjoint(
+                    np.conj(np.array(flm_1d)),
+                    L,
+                    spin,
+                    Method=sampling_str[ssht_sampling],
+                    Reality=reality,
+                    backend=_backend,
+                )
             )
         )
     else:  # DH or GL sampling
         quad_weights = quadrature_jax.quad_weights_transform(
             L, sampling_str[ssht_sampling].lower()
         )
-        f = np.conj(
-            pyssht.inverse(
-                np.conj(flm_1d),
-                L,
-                spin,
-                Method=sampling_str[ssht_sampling],
-                Reality=reality,
-                backend=_backend,
+        f = jnp.array(
+            np.conj(
+                pyssht.inverse(
+                    np.conj(np.array(flm_1d)),
+                    L,
+                    spin,
+                    Method=sampling_str[ssht_sampling],
+                    Reality=reality,
+                    backend=_backend,
+                )
             )
         )
         f = jnp.einsum("tp,t->tp", f, quad_weights, optimize=True)
 
     return f, None, None, None, None, None
 
 
@@ -243,35 +257,39 @@
         jnp.ndarray: Signal on the sphere.
 
     Note:
         [1] Gorski, Krzysztof M., et al. "HEALPix: A framework for high-resolution
         discretization and fast analysis of data distributed on the sphere." The
         Astrophysical Journal 622.2 (2005): 759
     """
-    flm = samples.flm_2d_to_hp(flm, L)
-    f = healpy.alm2map(flm, lmax=L - 1, nside=nside)
+    flm = reindex.flm_2d_to_hp_fast(flm, L)
+    f = jnp.array(healpy.alm2map(np.array(flm), lmax=L - 1, nside=nside))
     return f
 
 
 def _healpy_inverse_fwd(flm: jnp.ndarray, L: int, nside: int):
     """Private function which implements the forward pass for inverse jax_healpy"""
     res = ([], L, nside)
     return healpy_inverse(flm, L, nside), res
 
 
 def _healpy_inverse_bwd(res, f):
     """Private function which implements the backward pass for inverse jax_healpy"""
     _, L, nside = res
-    f_new = f * (12 * nside**2) / (4 * np.pi)
-    flm_out = np.conj(healpy.map2alm(np.conj(f_new), lmax=L - 1, iter=0))
+    f_new = f * (12 * nside**2) / (4 * jnp.pi)
+    flm_out = jnp.array(
+        np.conj(healpy.map2alm(np.conj(np.array(f_new)), lmax=L - 1, iter=0))
+    )
     # iter MUST be zero otherwise gradient propagation is incorrect (JDM).
-    flm_out = samples.flm_hp_to_2d(flm_out, L)
-    m_conj = (-1) ** (np.arange(1, L) % 2)
-    flm_out[..., L:] += np.flip(m_conj * np.conj(flm_out[..., : L - 1]), axis=-1)
-    flm_out[..., : L - 1] = 0
+    flm_out = reindex.flm_hp_to_2d_fast(flm_out, L)
+    m_conj = (-1) ** (jnp.arange(1, L) % 2)
+    flm_out = flm_out.at[..., L:].add(
+        jnp.flip(m_conj * jnp.conj(flm_out[..., : L - 1]), axis=-1)
+    )
+    flm_out = flm_out.at[..., : L - 1].set(0)
 
     return flm_out, None, None
 
 
 @custom_vjp
 def healpy_forward(f: jnp.ndarray, L: int, nside: int, iter: int = 3) -> jnp.ndarray:
     r"""Compute the forward scalar spherical harmonic transform (healpy JAX).
@@ -297,30 +315,32 @@
         jnp.ndarray: Harmonic coefficients of signal f.
 
     Note:
         [1] Gorski, Krzysztof M., et al. "HEALPix: A framework for high-resolution
         discretization and fast analysis of data distributed on the sphere." The
         Astrophysical Journal 622.2 (2005): 759
     """
-    flm = healpy.map2alm(np.array(f), lmax=L - 1, iter=iter)
-    return samples.flm_hp_to_2d(flm, L)
+    flm = jnp.array(healpy.map2alm(np.array(f), lmax=L - 1, iter=iter))
+    return reindex.flm_hp_to_2d_fast(flm, L)
 
 
 def _healpy_forward_fwd(f: jnp.ndarray, L: int, nside: int, iter: int = 3):
     """Private function which implements the forward pass for forward jax_healpy"""
     res = ([], L, nside, iter)
     return healpy_forward(f, L, nside, iter), res
 
 
 def _healpy_forward_bwd(res, flm):
     """Private function which implements the backward pass for forward jax_healpy"""
     _, L, nside, _ = res
-    flm_new = samples.flm_2d_to_hp(np.array(flm), L)
-    f = np.conj(healpy.alm2map(np.conj(flm_new), lmax=L - 1, nside=nside))
-    return f * (4 * np.pi) / (12 * nside**2), None, None, None
+    flm_new = reindex.flm_2d_to_hp_fast(flm, L)
+    f = jnp.array(
+        np.conj(healpy.alm2map(np.conj(np.array(flm_new)), lmax=L - 1, nside=nside))
+    )
+    return f * (4 * jnp.pi) / (12 * nside**2), None, None, None
 
 
 # Link JAX gradients for C backend functions
 ssht_inverse.defvjp(_ssht_inverse_fwd, _ssht_inverse_bwd)
 ssht_forward.defvjp(_ssht_forward_fwd, _ssht_forward_bwd)
 healpy_inverse.defvjp(_healpy_inverse_fwd, _healpy_inverse_bwd)
 healpy_forward.defvjp(_healpy_forward_fwd, _healpy_forward_bwd)
```

### Comparing `s2fft-1.1.0/s2fft/transforms/otf_recursions.py` & `s2fft-1.1.1/s2fft/transforms/otf_recursions.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/transforms/spherical.py` & `s2fft-1.1.1/s2fft/transforms/spherical.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/transforms/wigner.py` & `s2fft-1.1.1/s2fft/transforms/wigner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from jax import jit, pmap, local_device_count
-
+from jax import jit, vmap
 
 import numpy as np
 import jax.numpy as jnp
-import jax.lax as lax
 from functools import partial
 from typing import List
 import s2fft
 from s2fft.sampling import so3_samples as samples
 from s2fft.transforms import c_backend_spherical as c_sph
 
 
@@ -16,15 +14,14 @@
     L: int,
     N: int,
     nside: int = None,
     sampling: str = "mw",
     method: str = "numpy",
     reality: bool = False,
     precomps: List = None,
-    spmd: bool = False,
     L_lower: int = 0,
     _ssht_backend: int = 1,
 ) -> np.ndarray:
     r"""Wrapper for the inverse Wigner transform, i.e. inverse Fourier transform on
     :math:`SO(3)`.
 
     Importantly, the convention adopted for storage of f is :math:`[\gamma, \beta,
@@ -57,18 +54,14 @@
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[np.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
 
-        spmd (bool, optional): Whether to map compute over multiple devices. Currently this
-            only maps over all available devices, and is only valid for JAX implementations.
-            Defaults to False.
-
         L_lower (int, optional): Harmonic lower-bound. Transform will only be computed
             for :math:`\texttt{L_lower} \leq \ell < \texttt{L}`. Defaults to 0.
 
         _ssht_backend (int, optional, experimental): Whether to default to SSHT core
             (set to 0) recursions or pick up ducc0 (set to 1) accelerated experimental
             backend. Use with caution.
 
@@ -77,33 +70,25 @@
 
     Returns:
         np.ndarray:  Signal on the on :math:`SO(3)` with shape :math:`[n_{\gamma},
         n_{\beta}, n_{\alpha}]`, where :math:`n_\xi` denotes the number of samples for
         angle :math:`\xi`.
 
     Note:
-        The single-program multiple-data (SPMD) optional variable determines whether
-        the transform is run over a single device or all available devices. For very low
-        harmonic bandlimits L this is inefficient as the I/O overhead for communication
-        between devices is noticable, however as L increases one will asymptotically
-        recover acceleration by the number of devices.
-
         [1] McEwen, Jason D. and Yves Wiaux. “A Novel Sampling Theorem on the Sphere.”
             IEEE Transactions on Signal Processing 59 (2011): 5876-5887.
     """
 
     if N >= 8 and method in ["numpy", "jax"]:
         raise Warning("Recursive transform may provide lower precision beyond N ~ 8")
 
     if method == "numpy":
         return inverse_numpy(flmn, L, N, nside, sampling, reality, precomps, L_lower)
     elif method == "jax":
-        return inverse_jax(
-            flmn, L, N, nside, sampling, reality, precomps, spmd, L_lower
-        )
+        return inverse_jax(flmn, L, N, nside, sampling, reality, precomps, L_lower)
     elif method == "jax_ssht":
         if sampling.lower() == "healpix":
             raise ValueError("SSHT does not support healpix sampling.")
         return inverse_jax_ssht(flmn, L, N, L_lower, sampling, reality, _ssht_backend)
     else:
         raise ValueError(
             f"Implementation {method} not recognised. Should be either numpy or jax."
@@ -189,24 +174,23 @@
         f = np.fft.irfft(fban[N - 1 :], 2 * N - 1, axis=ax, norm="forward")
     else:
         f = np.fft.ifft(np.fft.ifftshift(fban, axes=ax), axis=ax, norm="forward")
 
     return f
 
 
-@partial(jit, static_argnums=(1, 2, 3, 4, 5, 7, 8))
+@partial(jit, static_argnums=(1, 2, 3, 4, 5, 7))
 def inverse_jax(
     flmn: jnp.ndarray,
     L: int,
     N: int,
     nside: int = None,
     sampling: str = "mw",
     reality: bool = False,
     precomps: List = None,
-    spmd: bool = False,
     L_lower: int = 0,
 ) -> jnp.ndarray:
     r"""Compute the inverse Wigner transform (JAX).
 
     Uses separation of variables and exploits the Price & McEwen recursion for accelerated
     and numerically stable Wiger-d on-the-fly recursions. The memory overhead for this
     function is theoretically :math:`\mathcal{O}(NL^2)`.
@@ -234,119 +218,55 @@
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[jnp.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
 
-        spmd (bool, optional): Whether to map compute over multiple devices. Currently this
-            only maps over all available devices. Defaults to False.
-
         L_lower (int, optional): Harmonic lower-bound. Transform will only be computed
             for :math:`\texttt{L_lower} \leq \ell < \texttt{L}`. Defaults to 0.
 
     Returns:
         jnp.ndarray: Signal on the sphere.
-
-    Note:
-        The single-program multiple-data (SPMD) optional variable determines whether
-        the transform is run over a single device or all available devices. For very low
-        harmonic bandlimits L this is inefficient as the I/O overhead for communication
-        between devices is noticable, however as L increases one will asymptotically
-        recover acceleration by the number of devices.
     """
     if precomps is None:
         precomps = s2fft.generate_precomputes_wigner_jax(
             L, N, sampling, nside, False, reality, L_lower
         )
+
     fban = jnp.zeros(samples.f_shape(L, N, sampling, nside), dtype=jnp.complex128)
 
     flmn = flmn.at[:, L_lower:].set(
         jnp.einsum(
             "...nlm,...l->...nlm",
             flmn[:, L_lower:],
             jnp.sqrt((2 * jnp.arange(L_lower, L) + 1) / (16 * jnp.pi**3)),
             optimize=True,
         )
     )
 
     n_start_ind = 0 if reality else -N + 1
     spins = jnp.arange(n_start_ind, N)
 
-    def spherical_loop(n, args):
-        fban, flmn, lrenorm, vsign, spins = args
-        fban = fban.at[n].add(
-            (-1) ** jnp.abs(spins[n])
-            * s2fft.inverse_jax(
-                flmn[n],
-                L,
-                -spins[n],
-                nside,
-                sampling,
-                False,
-                [
-                    lrenorm[n],
-                    vsign[n],
-                    precomps[2][0],
-                    precomps[3][0],
-                    precomps[4][0],
-                ],
-                False,
-                L_lower,
-            )
-        )
-        return fban, flmn, lrenorm, vsign, spins
-
-    if spmd:
-        # TODO: Generalise this to optional device counts.
-        ndevices = local_device_count()
-        opsdevice = int(N / ndevices) if reality else int((2 * N - 1) / ndevices)
-
-        def eval_spherical_loop(fban, flmn, lrenorm, vsign, spins):
-            return lax.fori_loop(
-                0,
-                opsdevice,
-                spherical_loop,
-                (fban, flmn, lrenorm, vsign, spins),
-            )[0]
-
-        # Reshape inputs
-        spmd_shape = (ndevices, opsdevice)
-        lrenorm = precomps[0].reshape(spmd_shape + precomps[0].shape[1:])
-        vsign = precomps[1].reshape(spmd_shape + precomps[1].shape[1:])
-        vin = flmn[N - 1 + n_start_ind :].reshape(spmd_shape + flmn.shape[1:])
-        vout = fban[N - 1 + n_start_ind :].reshape(spmd_shape + fban.shape[1:])
-        spins = spins.reshape(spmd_shape)
-
-        fban = fban.at[N - 1 + n_start_ind :].add(
-            pmap(eval_spherical_loop, in_axes=(0, 0, 0, 0, 0))(
-                vout, vin, lrenorm, vsign, spins
-            ).reshape((ndevices * opsdevice,) + fban.shape[1:])
-        )
-    else:
-        opsdevice = N if reality else 2 * N - 1
-        fban = fban.at[N - 1 + n_start_ind :].add(
-            lax.fori_loop(
-                0,
-                opsdevice,
-                spherical_loop,
-                (
-                    fban[N - 1 + n_start_ind :],
-                    flmn[N - 1 + n_start_ind :],
-                    precomps[0],
-                    precomps[1],
-                    spins,
-                ),
-            )[0]
+    def func(flm, spin, p0, p1, p2, p3, p4):
+        precomps = [p0, p1, p2, p3, p4]
+        return (-1) ** jnp.abs(spin) * s2fft.inverse_jax(
+            flm, L, -spin, nside, sampling, False, precomps, False, L_lower
         )
 
+    fban = fban.at[N - 1 + n_start_ind :].set(
+        vmap(
+            partial(func, p2=precomps[2][0], p3=precomps[3][0], p4=precomps[4][0]),
+            in_axes=(0, 0, 0, 0),
+        )(flmn[N - 1 + n_start_ind :], spins, precomps[0], precomps[1])
+    )
     if reality:
-        fban = fban.at[: N - 1].set(jnp.flip(jnp.conj(fban[N:]), axis=0))
-    fban = jnp.conj(jnp.fft.ifftshift(fban, axes=0))
-    f = jnp.conj(jnp.fft.fft(fban, axis=0, norm="backward"))
+        f = jnp.fft.irfft(fban[N - 1 :], 2 * N - 1, axis=0, norm="forward")
+    else:
+        f = jnp.fft.ifft(jnp.fft.ifftshift(fban, axes=0), axis=0, norm="forward")
 
     return f
 
 
 def inverse_jax_ssht(
     flmn: jnp.ndarray,
     L: int,
@@ -388,58 +308,28 @@
     Returns:
         np.ndarray: Signal on the sphere.
 
     Note:
         [1] McEwen, Jason D. and Yves Wiaux. “A Novel Sampling Theorem on the Sphere.”
             IEEE Transactions on Signal Processing 59 (2011): 5876-5887.
     """
-    ssht_sampling = ["mw", "mwss", "dh", "gl"].index(sampling.lower())
-    fban = jnp.zeros(samples.f_shape(L, N, sampling), dtype=jnp.complex128)
-
-    flmn = flmn.at[:, L_lower:].set(
-        jnp.einsum(
-            "...nlm,...l->...nlm",
-            flmn[:, L_lower:],
-            jnp.sqrt((2 * jnp.arange(L_lower, L) + 1) / (16 * jnp.pi**3)),
-            optimize=True,
-        )
-    )
-
-    n_start_ind = 0 if reality else -N + 1
-    for n in range(n_start_ind, N):
-        fban = fban.at[N - 1 + n].add(
-            (-1) ** jnp.abs(n)
-            * c_sph.ssht_inverse(
-                flmn[N - 1 + n],
-                L,
-                -n,
-                reality if n == 0 else False,
-                ssht_sampling,
-                _ssht_backend,
-            )
-        )
-
-    if reality:
-        f = jnp.fft.irfft(fban[N - 1 :], 2 * N - 1, axis=-3, norm="forward")
-    else:
-        f = jnp.fft.ifft(jnp.fft.ifftshift(fban, axes=-3), axis=-3, norm="forward")
-
-    return f
+    flmn, fban = _inverse_norm(flmn, L, N, L_lower, sampling)
+    fban = _flmn_to_fban(flmn, fban, L, N, sampling, reality, _ssht_backend)
+    return _fban_to_f(fban, L, N, reality)
 
 
 def forward(
     f: np.ndarray,
     L: int,
     N: int,
     nside: int = None,
     sampling: str = "mw",
     method: str = "numpy",
     reality: bool = False,
     precomps: List = None,
-    spmd: bool = False,
     L_lower: int = 0,
     _ssht_backend: int = 1,
 ) -> np.ndarray:
     r"""Wrapper for the forward Wigner transform, i.e. Fourier transform on
     :math:`SO(3)`.
 
     Importantly, the convention adopted for storage of f is :math:`[\gamma, \beta,
@@ -474,49 +364,39 @@
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[np.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
 
-        spmd (bool, optional): Whether to map compute over multiple devices. Currently this
-            only maps over all available devices, and is only valid for JAX implementations.
-            Defaults to False.
-
         L_lower (int, optional): Harmonic lower-bound. Transform will only be computed
             for :math:`\texttt{L_lower} \leq \ell < \texttt{L}`. Defaults to 0.
 
         _ssht_backend (int, optional, experimental): Whether to default to SSHT core
             (set to 0) recursions or pick up ducc0 (set to 1) accelerated experimental
             backend. Use with caution.
 
     Raises:
         ValueError: Transform method not recognised.
 
     Returns:
         np.ndarray: Wigner coefficients `flmn` with shape :math:`[2N-1, L, 2L-1]`.
 
     Note:
-        The single-program multiple-data (SPMD) optional variable determines whether
-        the transform is run over a single device or all available devices. For very low
-        harmonic bandlimits L this is inefficient as the I/O overhead for communication
-        between devices is noticable, however as L increases one will asymptotically
-        recover acceleration by the number of devices.
-
         [1] McEwen, Jason D. and Yves Wiaux. “A Novel Sampling Theorem on the Sphere.”
             IEEE Transactions on Signal Processing 59 (2011): 5876-5887.
     """
 
     if N >= 8 and method in ["numpy", "jax"]:
         raise Warning("Recursive transform may provide lower precision beyond N ~ 8")
 
     if method == "numpy":
         return forward_numpy(f, L, N, nside, sampling, reality, precomps, L_lower)
     elif method == "jax":
-        return forward_jax(f, L, N, nside, sampling, reality, precomps, spmd, L_lower)
+        return forward_jax(f, L, N, nside, sampling, reality, precomps, L_lower)
     elif method == "jax_ssht":
         if sampling.lower() == "healpix":
             raise ValueError("SSHT does not support healpix sampling.")
         return forward_jax_ssht(f, L, N, L_lower, sampling, reality, _ssht_backend)
     else:
         raise ValueError(
             f"Implementation {method} not recognised. Should be either numpy or jax."
@@ -611,24 +491,23 @@
         "...nlm,...l->...nlm",
         flmn[:, L_lower:],
         np.sqrt(4 * np.pi / (2 * np.arange(L_lower, L) + 1)),
     )
     return flmn
 
 
-@partial(jit, static_argnums=(1, 2, 3, 4, 5, 7, 8))
+@partial(jit, static_argnums=(1, 2, 3, 4, 5, 7))
 def forward_jax(
     f: jnp.ndarray,
     L: int,
     N: int,
     nside: int = None,
     sampling: str = "mw",
     reality: bool = False,
     precomps: List = None,
-    spmd: bool = False,
     L_lower: int = 0,
 ) -> jnp.ndarray:
     r"""Compute the forward Wigner transform (JAX).
 
     Uses separation of variables and exploits the Price & McEwen recursion for accelerated
     and numerically stable Wiger-d on-the-fly recursions. The memory overhead for this
     function is theoretically :math:`\mathcal{O}(NL^2)`.
@@ -658,116 +537,66 @@
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[jnp.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
 
-        spmd (bool, optional): Whether to map compute over multiple devices. Currently this
-            only maps over all available devices, and is only valid for JAX implementations.
-            Defaults to False.
-
         L_lower (int, optional): Harmonic lower-bound. Transform will only be computed
             for :math:`\texttt{L_lower} \leq \ell < \texttt{L}`. Defaults to 0.
 
     Returns:
         jnp.ndarray: Wigner coefficients `flmn` with shape :math:`[2N-1, L, 2L-1]`.
     """
     if precomps is None:
         precomps = s2fft.generate_precomputes_wigner_jax(
             L, N, sampling, nside, True, reality, L_lower
         )
+
     flmn = jnp.zeros(samples.flmn_shape(L, N), dtype=jnp.complex128)
 
     if reality:
         fban = jnp.fft.rfft(jnp.real(f), axis=0, norm="backward")
     else:
         fban = jnp.fft.fftshift(jnp.fft.fft(f, axis=0, norm="backward"), axes=0)
 
     fban *= 2 * jnp.pi / (2 * N - 1)
-
-    if reality:
-        sgn = (-1) ** abs(jnp.arange(-L + 1, L))
-
     n_start_ind = 0 if reality else -N + 1
     spins = jnp.arange(n_start_ind, N)
 
-    def spherical_loop(n, args):
-        flmn, fban, lrenorm, vsign, spins = args
-        flmn = flmn.at[n].add(
-            (-1) ** spins[n]
-            * s2fft.forward_jax(
-                fban[n],
-                L,
-                -spins[n],
-                nside,
-                sampling,
-                False,
-                [
-                    lrenorm[n],
-                    vsign[n],
-                    precomps[2][0],
-                    precomps[3][0],
-                    precomps[4][0],
-                ],
-                False,
-                L_lower,
-            )
+    def func(fba, spin, p0, p1, p2, p3, p4):
+        precomps = [p0, p1, p2, p3, p4]
+        return (-1) ** jnp.abs(spin) * s2fft.forward_jax(
+            fba, L, -spin, nside, sampling, False, precomps, False, L_lower
         )
-        return flmn, fban, lrenorm, vsign, spins
 
-    if spmd:
-        # TODO: Generalise this to optional device counts.
-        ndevices = local_device_count()
-        opsdevice = int(N / ndevices) if reality else int((2 * N - 1) / ndevices)
-
-        def eval_spherical_loop(fban, flmn, lrenorm, vsign, spins):
-            return lax.fori_loop(
-                0,
-                opsdevice,
-                spherical_loop,
-                (fban, flmn, lrenorm, vsign, spins),
-            )[0]
-
-        # Reshape inputs
-        spmd_shape = (ndevices, opsdevice)
-        lrenorm = precomps[0].reshape(spmd_shape + precomps[0].shape[1:])
-        vsign = precomps[1].reshape(spmd_shape + precomps[1].shape[1:])
-        fban = fban.reshape(spmd_shape + fban.shape[1:])
-        vout = flmn[N - 1 + n_start_ind :].reshape(spmd_shape + flmn.shape[1:])
-        spins = spins.reshape(spmd_shape)
-
-        flmn = flmn.at[N - 1 + n_start_ind :].add(
-            pmap(eval_spherical_loop, in_axes=(0, 0, 0, 0, 0))(
-                vout, fban, lrenorm, vsign, spins
-            ).reshape((ndevices * opsdevice,) + flmn.shape[1:])
-        )
-    else:
-        opsdevice = N if reality else 2 * N - 1
-        flmn = flmn.at[N - 1 + n_start_ind :].add(
-            lax.fori_loop(
-                0,
-                opsdevice,
-                spherical_loop,
-                (
-                    flmn[N - 1 + n_start_ind :],
-                    fban,
-                    precomps[0],
-                    precomps[1],
-                    spins,
-                ),
-            )[0]
-        )
+    flmn = flmn.at[N - 1 + n_start_ind :].set(
+        vmap(
+            partial(func, p2=precomps[2][0], p3=precomps[3][0], p4=precomps[4][0]),
+            in_axes=(0, 0, 0, 0),
+        )(fban, spins, precomps[0], precomps[1])
+    )
 
-    # Fill out Wigner coefficients steerability of real signals
-    for n in range(n_start_ind, N):
-        if reality and n != 0:
-            flmn = flmn.at[N - 1 - n].set(
-                jnp.conj(jnp.flip(flmn[N - 1 + n] * sgn * (-1) ** n, axis=-1))
+    if reality:
+        nidx = jnp.arange(1, N)
+        sgn = (-1) ** abs(jnp.arange(-L + 1, L))
+        flmn = flmn.at[N - 1 - nidx].set(
+            jnp.conj(
+                jnp.flip(
+                    jnp.einsum(
+                        "nlm,m,n->nlm",
+                        flmn[N - 1 + nidx],
+                        sgn,
+                        (-1) ** nidx,
+                        optimize=True,
+                    ),
+                    axis=-1,
+                )
             )
+        )
 
     flmn = flmn.at[:, L_lower:].set(
         jnp.einsum(
             "...nlm,...l->...nlm",
             flmn[:, L_lower:],
             jnp.sqrt(4 * jnp.pi / (2 * jnp.arange(L_lower, L) + 1)),
             optimize=True,
@@ -819,45 +648,139 @@
     Returns:
         jnp.ndarray: Wigner coefficients `flmn` with shape :math:`[2N-1, L, 2L-1]`.
 
     Note:
         [1] McEwen, Jason D. and Yves Wiaux. “A Novel Sampling Theorem on the Sphere.”
             IEEE Transactions on Signal Processing 59 (2011): 5876-5887.
     """
-    ssht_sampling = ["mw", "mwss", "dh", "gl"].index(sampling.lower())
+    flmn, fban = _f_to_fban(f, L, N, reality)
+    flmn = _fban_to_flmn(flmn, fban, L, N, sampling, reality, _ssht_backend)
+    return _reality_and_norm(flmn, L, N, L_lower, reality)
+
+
+@partial(jit, static_argnums=(1, 2, 3))
+def _f_to_fban(f: jnp.ndarray, L: int, N: int, reality: bool = False) -> jnp.ndarray:
+    """Private function which maps from f to fban (C backend)"""
     flmn = jnp.zeros(samples.flmn_shape(L, N), dtype=jnp.complex128)
 
     if reality:
         fban = jnp.fft.rfft(jnp.real(f), axis=0, norm="backward")
     else:
         fban = jnp.fft.fftshift(jnp.fft.fft(f, axis=0, norm="backward"), axes=0)
 
     fban *= 2 * jnp.pi / (2 * N - 1)
 
+    return flmn, fban
+
+
+def _fban_to_flmn(
+    flmn: jnp.ndarray,
+    fban: jnp.ndarray,
+    L: int,
+    N: int,
+    sampling: str = "mw",
+    reality: bool = False,
+    _ssht_backend: int = 1,
+) -> jnp.ndarray:
+    """Private function which maps from fban to flmn (C backend)"""
+    ssht_sampling = ["mw", "mwss", "dh", "gl"].index(sampling.lower())
     n_start_ind = 0 if reality else -N + 1
+    func = partial(
+        c_sph.ssht_forward,
+        L=L,
+        reality=False,
+        ssht_sampling=ssht_sampling,
+        _ssht_backend=_ssht_backend,
+    )
     for n in range(n_start_ind, N):
-        flmn = flmn.at[N - 1 + n].set(
-            (-1) ** jnp.abs(n)
-            * c_sph.ssht_forward(
-                fban[jnp.int64(n - n_start_ind)],
-                L,
-                -n,
-                False,
-                ssht_sampling,
-                _ssht_backend,
-            )
+        flmn = flmn.at[N - 1 + n].add(
+            (-1) ** jnp.abs(n) * func(fban[int(n - n_start_ind)], spin=-n)
         )
-        if reality and n != 0:
-            sgn = (-1) ** abs(jnp.arange(-L + 1, L))
-            flmn = flmn.at[N - 1 - n].set(
-                jnp.conj(jnp.flip(flmn[N - 1 + n] * sgn * (-1) ** n, axis=-1))
+    return flmn
+
+
+@partial(jit, static_argnums=(1, 2, 3, 4))
+def _reality_and_norm(
+    flmn: jnp.ndarray, L: int, N: int, L_lower: int = 0, reality: bool = False
+) -> jnp.ndarray:
+    """Private function which maps from f to fban (C backend)"""
+    if reality:
+        nidx = jnp.arange(1, N)
+        sgn = (-1) ** abs(jnp.arange(-L + 1, L))
+        flmn = flmn.at[N - 1 - nidx].set(
+            jnp.conj(
+                jnp.flip(
+                    jnp.einsum(
+                        "nlm,m,n->nlm",
+                        flmn[N - 1 + nidx],
+                        sgn,
+                        (-1) ** nidx,
+                        optimize=True,
+                    ),
+                    axis=-1,
+                )
             )
+        )
 
     flmn = flmn.at[:, L_lower:].set(
         jnp.einsum(
             "...nlm,...l->...nlm",
             flmn[:, L_lower:],
             jnp.sqrt(4 * jnp.pi / (2 * jnp.arange(L_lower, L) + 1)),
             optimize=True,
         )
     )
     return flmn
+
+
+@partial(jit, static_argnums=(1, 2, 3, 4))
+def _inverse_norm(
+    flmn: jnp.ndarray, L: int, N: int, L_lower: int = 0, sampling: str = "mw"
+):
+    """Private function which normalised flmn for inverse Wigner (C backend)"""
+    fban = jnp.zeros(samples.f_shape(L, N, sampling), dtype=jnp.complex128)
+
+    flmn = flmn.at[:, L_lower:].set(
+        jnp.einsum(
+            "...nlm,...l->...nlm",
+            flmn[:, L_lower:],
+            jnp.sqrt((2 * jnp.arange(L_lower, L) + 1) / (16 * jnp.pi**3)),
+            optimize=True,
+        )
+    )
+    return flmn, fban
+
+
+def _flmn_to_fban(
+    flmn: jnp.ndarray,
+    fban: jnp.ndarray,
+    L: int,
+    N: int,
+    sampling: str = "mw",
+    reality: bool = False,
+    _ssht_backend: int = 1,
+) -> jnp.ndarray:
+    """Private function which maps from flmn to fban (C backend)"""
+    ssht_sampling = ["mw", "mwss", "dh", "gl"].index(sampling.lower())
+    n_start_ind = 0 if reality else -N + 1
+    func = partial(
+        c_sph.ssht_inverse,
+        L=L,
+        reality=False,
+        ssht_sampling=ssht_sampling,
+        _ssht_backend=_ssht_backend,
+    )
+    for n in range(n_start_ind, N):
+        fban = fban.at[N - 1 + n].add(
+            (-1) ** jnp.abs(n) * func(flmn[N - 1 + n], spin=-n)
+        )
+    return fban
+
+
+@partial(jit, static_argnums=(1, 2, 3))
+def _fban_to_f(fban: jnp.ndarray, L: int, N: int, reality: bool = False) -> jnp.ndarray:
+    """Private function which maps from fban to f (C backend)"""
+    if reality:
+        f = jnp.fft.irfft(fban[N - 1 :], 2 * N - 1, axis=-3, norm="forward")
+    else:
+        f = jnp.fft.ifft(jnp.fft.ifftshift(fban, axes=-3), axis=-3, norm="forward")
+    return f
```

### Comparing `s2fft-1.1.0/s2fft/utils/healpix_ffts.py` & `s2fft-1.1.1/s2fft/utils/healpix_ffts.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/utils/quadrature.py` & `s2fft-1.1.1/s2fft/utils/quadrature.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/utils/quadrature_jax.py` & `s2fft-1.1.1/s2fft/utils/quadrature_jax.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/utils/quadrature_torch.py` & `s2fft-1.1.1/s2fft/utils/quadrature_torch.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/utils/resampling.py` & `s2fft-1.1.1/s2fft/utils/resampling.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/utils/resampling_jax.py` & `s2fft-1.1.1/s2fft/utils/resampling_jax.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/utils/resampling_torch.py` & `s2fft-1.1.1/s2fft/utils/resampling_torch.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/utils/rotation.py` & `s2fft-1.1.1/s2fft/utils/rotation.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft/utils/signal_generator.py` & `s2fft-1.1.1/s2fft/utils/signal_generator.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/s2fft.egg-info/PKG-INFO` & `s2fft-1.1.1/s2fft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2fft
-Version: 1.1.0
+Version: 1.1.1
 Summary: Differentiable and accelerated spherical transforms with JAX
 Home-page: https://github.com/astro-informatics/s2fft
 Author: Matthew A. Price, Jason D. McEwen & Contributors
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `s2fft-1.1.0/s2fft.egg-info/SOURCES.txt` & `s2fft-1.1.1/s2fft.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 s2fft/recursions/price_mcewen.py
 s2fft/recursions/risbo.py
 s2fft/recursions/risbo_jax.py
 s2fft/recursions/trapani.py
 s2fft/recursions/turok.py
 s2fft/recursions/turok_jax.py
 s2fft/sampling/__init__.py
+s2fft/sampling/reindex.py
 s2fft/sampling/s2_samples.py
 s2fft/sampling/so3_samples.py
 s2fft/transforms/__init__.py
 s2fft/transforms/c_backend_spherical.py
 s2fft/transforms/otf_recursions.py
 s2fft/transforms/spherical.py
 s2fft/transforms/wigner.py
```

### Comparing `s2fft-1.1.0/setup.py` & `s2fft-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
     ],
     name="s2fft",
-    version="1.1.0",
+    version="1.1.1",
     url="https://github.com/astro-informatics/s2fft",
     author="Matthew A. Price, Jason D. McEwen & Contributors",
     license="MIT",
     python_requires=">=3.8",
     install_requires=requirements,
     description=("Differentiable and accelerated spherical transforms with JAX"),
     long_description_content_type="text/x-rst",
```

### Comparing `s2fft-1.1.0/tests/conftest.py` & `s2fft-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/tests/test_healpix_ffts.py` & `s2fft-1.1.1/tests/test_healpix_ffts.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/tests/test_quadrature.py` & `s2fft-1.1.1/tests/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/tests/test_resampling.py` & `s2fft-1.1.1/tests/test_resampling.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/tests/test_samples.py` & `s2fft-1.1.1/tests/test_samples.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,42 @@
 import pytest
 import numpy as np
+import jax.numpy as jnp
 import pyssht as ssht
 import healpy as hp
 from s2fft.sampling import s2_samples as samples
+from s2fft.sampling import reindex
 
 
 nside_to_test = [16, 32]
 
 
 @pytest.mark.parametrize("L", [15, 16])
+def test_fast_reindexing_functions(L: int):
+    flm = np.random.randn(L, 2 * L - 1) + 1j * np.random.randn(L, 2 * L - 1)
+    flm_jax = jnp.array(flm)
+
+    flm_1d = samples.flm_2d_to_1d(flm, L)
+    flm_1d_jax = reindex.flm_2d_to_1d_fast(flm_jax, L)
+    np.testing.assert_allclose(flm_1d, flm_1d_jax)
+
+    flm_2d = samples.flm_1d_to_2d(flm_1d, L)
+    flm_2d_jax = reindex.flm_1d_to_2d_fast(flm_1d_jax, L)
+    np.testing.assert_allclose(flm_2d, flm_2d_jax)
+
+    flm_hp = samples.flm_2d_to_hp(flm_2d, L)
+    flm_hp_jax = reindex.flm_2d_to_hp_fast(flm_2d_jax, L)
+    np.testing.assert_allclose(flm_hp, flm_hp_jax)
+
+    flm_2d = samples.flm_hp_to_2d(flm_hp, L)
+    flm_2d_jax = reindex.flm_hp_to_2d_fast(flm_hp_jax, L)
+    np.testing.assert_allclose(flm_2d, flm_2d_jax)
+
+
+@pytest.mark.parametrize("L", [15, 16])
 @pytest.mark.parametrize("sampling", ["mw", "mwss", "dh", "gl"])
 def test_samples_n_and_angles(L: int, sampling: str):
     # Test ntheta and nphi
     ntheta = samples.ntheta(L, sampling)
     nphi = samples.nphi_equiang(L, sampling)
     (ntheta_ssht, nphi_ssht) = ssht.sample_shape(L, sampling.upper())
     assert (ntheta, nphi) == pytest.approx((ntheta_ssht, nphi_ssht))
```

### Comparing `s2fft-1.1.0/tests/test_spherical_base.py` & `s2fft-1.1.1/tests/test_spherical_base.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/tests/test_spherical_custom_grads.py` & `s2fft-1.1.1/tests/test_spherical_custom_grads.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from s2fft.recursions.price_mcewen import generate_precomputes_jax
 
 L_to_test = [16]
 L_lower_to_test = [2]
 spin_to_test = [-2, 0, 1]
 nside_to_test = [8]
 sampling_to_test = ["mw", "mwss", "dh", "gl"]
-legacy_mode_to_test = ["jax_ssht"]
 reality_to_test = [False, True]
 
 
 @pytest.mark.parametrize("L", L_to_test)
 @pytest.mark.parametrize("L_lower", L_lower_to_test)
 @pytest.mark.parametrize("spin", spin_to_test)
 @pytest.mark.parametrize("sampling", sampling_to_test)
```

### Comparing `s2fft-1.1.0/tests/test_spherical_precompute.py` & `s2fft-1.1.1/tests/test_spherical_precompute.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/tests/test_spherical_transform.py` & `s2fft-1.1.1/tests/test_spherical_transform.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/tests/test_utils.py` & `s2fft-1.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/tests/test_wigner_base.py` & `s2fft-1.1.1/tests/test_wigner_base.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/tests/test_wigner_custom_grads.py` & `s2fft-1.1.1/tests/test_wigner_custom_grads.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,21 +32,19 @@
     precomps = generate_precomputes_wigner_jax(
         L, N, sampling, None, False, reality, L_lower
     )
 
     flmn = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
     flmn_target = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
     f_target = wigner.inverse_jax(
-        flmn_target, L, N, None, sampling, reality, precomps, False, L_lower
+        flmn_target, L, N, None, sampling, reality, precomps, L_lower
     )
 
     def func(flmn):
-        f = wigner.inverse_jax(
-            flmn, L, N, None, sampling, reality, precomps, False, L_lower
-        )
+        f = wigner.inverse_jax(flmn, L, N, None, sampling, reality, precomps, L_lower)
         return jnp.sum(jnp.abs(f - f_target) ** 2)
 
     check_grads(func, (flmn,), order=1, modes=("rev"))
 
 
 @pytest.mark.parametrize("L", L_to_test)
 @pytest.mark.parametrize("N", N_to_test)
@@ -64,20 +62,18 @@
 ):
     precomps = generate_precomputes_wigner_jax(
         L, N, sampling, None, True, reality, L_lower
     )
 
     flmn_target = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
     flmn = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
-    f = wigner.inverse_jax(flmn, L, N, None, sampling, reality, None, False, L_lower)
+    f = wigner.inverse_jax(flmn, L, N, None, sampling, reality, None, L_lower)
 
     def func(f):
-        flmn = wigner.forward_jax(
-            f, L, N, None, sampling, reality, precomps, False, L_lower
-        )
+        flmn = wigner.forward_jax(f, L, N, None, sampling, reality, precomps, L_lower)
         return jnp.sum(jnp.abs(flmn - flmn_target) ** 2)
 
     check_grads(func, (f,), order=1, modes=("rev"))
 
 
 @pytest.mark.parametrize("L", L_to_test)
 @pytest.mark.parametrize("N", N_to_test)
@@ -98,15 +94,15 @@
 
     if sampling.lower() == "dh" and _ssht_backend == 1:
         pytest.skip("Driscoll Healy ducc0 backend gradient calculation tempremental.")
 
     flmn = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
     flmn_target = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
     f_target = wigner.inverse_jax(
-        flmn_target, L, N, None, sampling, reality, None, False, L_lower
+        flmn_target, L, N, None, sampling, reality, None, L_lower
     )
 
     def func(flmn):
         f = wigner.inverse(
             jnp.array(flmn),
             L,
             N,
@@ -140,15 +136,15 @@
 ):
 
     if sampling.lower() == "dh" and _ssht_backend == 1:
         pytest.skip("Driscoll Healy ducc0 backend gradient calculation tempremental.")
 
     flmn_target = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
     flmn = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
-    f = wigner.inverse_jax(flmn, L, N, None, sampling, reality, None, False, L_lower)
+    f = wigner.inverse_jax(flmn, L, N, None, sampling, reality, None, L_lower)
 
     def func(f):
         flmn = wigner.forward(
             f,
             L,
             N,
             None,
```

### Comparing `s2fft-1.1.0/tests/test_wigner_precompute.py` & `s2fft-1.1.1/tests/test_wigner_precompute.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/tests/test_wigner_recursions.py` & `s2fft-1.1.1/tests/test_wigner_recursions.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/tests/test_wigner_samples.py` & `s2fft-1.1.1/tests/test_wigner_samples.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.1.0/tests/test_wigner_transform.py` & `s2fft-1.1.1/tests/test_wigner_transform.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,89 +14,76 @@
 
 L_to_test = [6, 7]
 N_to_test = [2]
 L_lower_to_test = [0, 2]
 sampling_to_test = ["mw", "mwss", "dh", "gl"]
 method_to_test = ["numpy", "jax"]
 reality_to_test = [False, True]
-multiple_gpus = [False, True]
 
 
 @pytest.mark.parametrize("L", L_to_test)
 @pytest.mark.parametrize("N", N_to_test)
 @pytest.mark.parametrize("L_lower", L_lower_to_test)
 @pytest.mark.parametrize("sampling", sampling_to_test)
 @pytest.mark.parametrize("method", method_to_test)
 @pytest.mark.parametrize("reality", reality_to_test)
-@pytest.mark.parametrize("spmd", multiple_gpus)
 @pytest.mark.filterwarnings("ignore::RuntimeWarning")
 def test_inverse_wigner_transform(
     flmn_generator,
     L: int,
     N: int,
     L_lower: int,
     sampling: str,
     method: str,
     reality: bool,
-    spmd: bool,
 ):
-    if spmd and method != "jax":
-        pytest.skip("GPU distribution only valid for JAX.")
-
     flmn = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
     f_check = base_wigner.inverse(flmn, L, N, L_lower, sampling, reality)
 
     if method.lower() == "jax":
         precomps = generate_precomputes_wigner_jax(
             L, N, sampling, None, False, reality, L_lower
         )
     else:
         precomps = generate_precomputes_wigner(
             L, N, sampling, None, False, reality, L_lower
         )
-    f = wigner.inverse(
-        flmn, L, N, None, sampling, method, reality, precomps, spmd, L_lower
-    )
+    f = wigner.inverse(flmn, L, N, None, sampling, method, reality, precomps, L_lower)
     np.testing.assert_allclose(f, f_check, atol=1e-14)
 
 
 @pytest.mark.parametrize("L", L_to_test)
 @pytest.mark.parametrize("N", N_to_test)
 @pytest.mark.parametrize("L_lower", L_lower_to_test)
 @pytest.mark.parametrize("sampling", sampling_to_test)
 @pytest.mark.parametrize("method", method_to_test)
 @pytest.mark.parametrize("reality", reality_to_test)
-@pytest.mark.parametrize("spmd", multiple_gpus)
 @pytest.mark.filterwarnings("ignore::RuntimeWarning")
 def test_forward_wigner_transform(
     flmn_generator,
     L: int,
     N: int,
     L_lower: int,
     sampling: str,
     method: str,
     reality: bool,
-    spmd: bool,
 ):
-    if spmd and method != "jax":
-        pytest.skip("GPU distribution only valid for JAX.")
-
     flmn = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
     f = base_wigner.inverse(flmn, L, N, L_lower, sampling, reality)
 
     if method.lower() == "jax":
         precomps = generate_precomputes_wigner_jax(
             L, N, sampling, None, True, reality, L_lower
         )
     else:
         precomps = generate_precomputes_wigner(
             L, N, sampling, None, True, reality, L_lower
         )
     flmn_check = wigner.forward(
-        f, L, N, None, sampling, method, reality, precomps, spmd, L_lower
+        f, L, N, None, sampling, method, reality, precomps, L_lower
     )
     np.testing.assert_allclose(flmn, flmn_check, atol=1e-14)
 
 
 @pytest.mark.parametrize("L", L_to_test)
 @pytest.mark.parametrize("N", N_to_test)
 @pytest.mark.parametrize("L_lower", L_lower_to_test)
```

