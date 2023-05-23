# Comparing `tmp/fslpy-3.9.4.tar.gz` & `tmp/fslpy-3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fslpy-3.9.4.tar", last modified: Sat May 28 19:36:53 2022, max compression
+gzip compressed data, was "dist/fslpy-3.9.5.tar", last modified: Thu Jun  2 22:44:23 2022, max compression
```

## Comparing `fslpy-3.9.4.tar` & `fslpy-3.9.5.tar`

### file list

```diff
@@ -1,1172 +1,1172 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/
--rw-rw-rw-   0 root         (0) root         (0)      365 2022-05-28 08:30:56.000000 fslpy-3.9.4/AUTHOR
--rw-rw-rw-   0 root         (0) root         (0)    47681 2022-05-28 08:30:56.000000 fslpy-3.9.4/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)       53 2022-05-28 08:30:56.000000 fslpy-3.9.4/COPYRIGHT
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-05-28 08:30:56.000000 fslpy-3.9.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      370 2022-05-28 08:30:56.000000 fslpy-3.9.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4584 2022-05-28 19:36:53.000000 fslpy-3.9.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3863 2022-05-28 08:30:56.000000 fslpy-3.9.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/doc/_static/
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/_static/theme_overrides.css
--rw-rw-rw-   0 root         (0) root         (0)       83 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)    11175 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     7022 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.atlases.rst
--rw-rw-rw-   0 root         (0) root         (0)      130 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.bitmap.rst
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.cifti.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.constants.rst
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.dicom.rst
--rw-rw-rw-   0 root         (0) root         (0)      130 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.dtifit.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.featanalysis.rst
--rw-rw-rw-   0 root         (0) root         (0)      142 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.featdesign.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.featimage.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.fixlabels.rst
--rw-rw-rw-   0 root         (0) root         (0)      142 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.freesurfer.rst
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.gifti.rst
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.image.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.imagewrapper.rst
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.melodicanalysis.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.melodicimage.rst
--rw-rw-rw-   0 root         (0) root         (0)      124 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.mesh.rst
--rw-rw-rw-   0 root         (0) root         (0)      136 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.mghimage.rst
--rw-rw-rw-   0 root         (0) root         (0)      595 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.rst
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.utils.rst
--rw-rw-rw-   0 root         (0) root         (0)      124 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.vest.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.volumelabels.rst
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.data.vtk.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.Text2Vest.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.Vest2Text.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.atlasq.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.fsl_abspath.rst
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.fsl_apply_x5.rst
--rw-rw-rw-   0 root         (0) root         (0)      163 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.fsl_convert_x5.rst
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.fsl_ents.rst
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.imcp.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.imglob.rst
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.imln.rst
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.immv.rst
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.imrm.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.imtest.rst
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.remove_ext.rst
--rw-rw-rw-   0 root         (0) root         (0)      163 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.resample_image.rst
--rw-rw-rw-   0 root         (0) root         (0)      740 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.scripts.rst
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.transform.affine.rst
--rw-rw-rw-   0 root         (0) root         (0)      142 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.transform.flirt.rst
--rw-rw-rw-   0 root         (0) root         (0)      142 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.transform.fnirt.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.transform.nonlinear.rst
--rw-rw-rw-   0 root         (0) root         (0)      268 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.transform.rst
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.transform.x5.rst
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.assertions.rst
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.bids.rst
--rw-rw-rw-   0 root         (0) root         (0)      130 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.cache.rst
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.deprecated.rst
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.ensure.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.filetree.filetree.rst
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.filetree.parse.rst
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.filetree.query.rst
--rw-rw-rw-   0 root         (0) root         (0)      281 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.filetree.rst
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.filetree.utils.rst
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.fslsub.rst
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.idle.rst
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.image.resample.rst
--rw-rw-rw-   0 root         (0) root         (0)      142 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.image.roi.rst
--rw-rw-rw-   0 root         (0) root         (0)      208 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.image.rst
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.imcp.rst
--rw-rw-rw-   0 root         (0) root         (0)      136 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.memoize.rst
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.meta.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.naninfrange.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.notifier.rst
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.parse_data.rst
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.path.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.platform.rst
--rw-rw-rw-   0 root         (0) root         (0)      576 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.rst
--rw-rw-rw-   0 root         (0) root         (0)      124 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.run.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.settings.rst
--rw-rw-rw-   0 root         (0) root         (0)      136 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.tempdir.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.utils.weakfuncref.rst
--rw-rw-rw-   0 root         (0) root         (0)      118 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.version.rst
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.bet.rst
--rw-rw-rw-   0 root         (0) root         (0)      136 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.eddy.rst
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.epi_reg.rst
--rw-rw-rw-   0 root         (0) root         (0)      136 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.fast.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.flirt.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.fnirt.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.fsl_anat.rst
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.fsl_sub.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.fslmaths.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.fslstats.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.fugue.rst
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.melodic.rst
--rw-rw-rw-   0 root         (0) root         (0)      136 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.misc.rst
--rw-rw-rw-   0 root         (0) root         (0)      494 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.rst
--rw-rw-rw-   0 root         (0) root         (0)      136 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.tbss.rst
--rw-rw-rw-   0 root         (0) root         (0)      160 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/fsl.wrappers.wrapperutils.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/doc/images/
--rw-rw-rw-   0 root         (0) root         (0)    99363 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/images/fnirt_coefficient_field.png
--rw-rw-rw-   0 root         (0) root         (0)   368845 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/images/fnirt_coefficient_field.xcf
--rw-rw-rw-   0 root         (0) root         (0)    83903 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/images/fnirt_warp_field.png
--rw-rw-rw-   0 root         (0) root         (0)   209568 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/images/fnirt_warp_field.xcf
--rw-rw-rw-   0 root         (0) root         (0)    67938 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/images/nonlinear_registration_process.png
--rw-rw-rw-   0 root         (0) root         (0)   300073 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/images/nonlinear_registration_process.xcf
--rw-rw-rw-   0 root         (0) root         (0)     2655 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-05-28 08:30:56.000000 fslpy-3.9.4/doc/mock_modules.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/fsl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/fsl/data/
--rw-rw-rw-   0 root         (0) root         (0)      337 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39304 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/atlases.py
--rw-rw-rw-   0 root         (0) root         (0)     5113 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/bitmap.py
--rw-rw-rw-   0 root         (0) root         (0)    20171 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/cifti.py
--rw-rw-rw-   0 root         (0) root         (0)     4720 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     8870 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/dicom.py
--rw-rw-rw-   0 root         (0) root         (0)    10079 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/dtifit.py
--rw-rw-rw-   0 root         (0) root         (0)    18029 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/featanalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    25901 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/featdesign.py
--rw-rw-rw-   0 root         (0) root         (0)    12212 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/featimage.py
--rw-rw-rw-   0 root         (0) root         (0)    10913 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/fixlabels.py
--rw-rw-rw-   0 root         (0) root         (0)    13044 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/freesurfer.py
--rw-rw-rw-   0 root         (0) root         (0)    13511 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/gifti.py
--rw-rw-rw-   0 root         (0) root         (0)    71521 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/image.py
--rw-rw-rw-   0 root         (0) root         (0)    42105 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/imagewrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     5611 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/melodicanalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4804 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/melodicimage.py
--rw-rw-rw-   0 root         (0) root         (0)    24326 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     5483 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/mghimage.py
--rw-rw-rw-   0 root         (0) root         (0)     3540 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4105 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/vest.py
--rw-rw-rw-   0 root         (0) root         (0)     9686 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/volumelabels.py
--rw-rw-rw-   0 root         (0) root         (0)     5156 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/data/vtk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/fsl/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      789 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/Text2Vest.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/Vest2Text.py
--rw-rw-rw-   0 root         (0) root         (0)    24552 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/atlasq.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/fsl_abspath.py
--rw-rw-rw-   0 root         (0) root         (0)     4403 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/fsl_apply_x5.py
--rw-rw-rw-   0 root         (0) root         (0)     7014 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/fsl_convert_x5.py
--rw-rw-rw-   0 root         (0) root         (0)     6846 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/fsl_ents.py
--rwxrwxrwx   0 root         (0) root         (0)     1822 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/imcp.py
--rw-rw-rw-   0 root         (0) root         (0)     4008 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/imglob.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/imln.py
--rwxrwxrwx   0 root         (0) root         (0)     1815 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/immv.py
--rw-rw-rw-   0 root         (0) root         (0)     1233 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/imrm.py
--rw-rw-rw-   0 root         (0) root         (0)     1634 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/imtest.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/remove_ext.py
--rw-rw-rw-   0 root         (0) root         (0)     6495 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/scripts/resample_image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/fsl/transform/
--rw-rw-rw-   0 root         (0) root         (0)      490 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/transform/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19369 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/transform/affine.py
--rw-rw-rw-   0 root         (0) root         (0)     5792 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/transform/flirt.py
--rw-rw-rw-   0 root         (0) root         (0)    15024 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/transform/fnirt.py
--rw-rw-rw-   0 root         (0) root         (0)    31907 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/transform/nonlinear.py
--rw-rw-rw-   0 root         (0) root         (0)    22936 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/transform/x5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/fsl/utils/
--rw-rw-rw-   0 root         (0) root         (0)      232 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4072 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/assertions.py
--rw-rw-rw-   0 root         (0) root         (0)     7187 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/bids.py
--rw-rw-rw-   0 root         (0) root         (0)     5114 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3952 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/deprecated.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/ensure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/fsl/utils/filetree/
--rw-rw-rw-   0 root         (0) root         (0)    11925 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22770 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/filetree.py
--rw-rw-rw-   0 root         (0) root         (0)     4227 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/parse.py
--rw-rw-rw-   0 root         (0) root         (0)    13571 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/fsl/utils/filetree/trees/
--rw-rw-rw-   0 root         (0) root         (0)      925 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/BedpostX.tree
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/Diffusion.tree
--rw-rw-rw-   0 root         (0) root         (0)     1825 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/HCP_Surface.tree
--rw-rw-rw-   0 root         (0) root         (0)     2096 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/HCP_directory.tree
--rw-rw-rw-   0 root         (0) root         (0)     1591 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/ProbtrackX.tree
--rw-rw-rw-   0 root         (0) root         (0)       82 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/bet.tree
--rw-rw-rw-   0 root         (0) root         (0)     3307 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/bids_raw.tree
--rw-rw-rw-   0 root         (0) root         (0)      498 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/dti.tree
--rw-rw-rw-   0 root         (0) root         (0)      760 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/eddy.tree
--rw-rw-rw-   0 root         (0) root         (0)      188 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/epi_reg.tree
--rw-rw-rw-   0 root         (0) root         (0)      332 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/fast.tree
--rw-rw-rw-   0 root         (0) root         (0)      446 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/feat.tree
--rw-rw-rw-   0 root         (0) root         (0)      155 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/feat_reg.tree
--rw-rw-rw-   0 root         (0) root         (0)      223 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/feat_stats.tree
--rw-rw-rw-   0 root         (0) root         (0)     2199 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/freesurfer.tree
--rw-rw-rw-   0 root         (0) root         (0)     1653 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/fsl_anat.tree
--rw-rw-rw-   0 root         (0) root         (0)       52 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/gfeat.tree
--rw-rw-rw-   0 root         (0) root         (0)      618 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/tbss.tree
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/topup.tree
--rw-rw-rw-   0 root         (0) root         (0)      457 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/trees/vbm.tree
--rw-rw-rw-   0 root         (0) root         (0)    14258 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/filetree/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    19508 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/fslsub.py
--rw-rw-rw-   0 root         (0) root         (0)    36831 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/idle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/fsl/utils/image/
--rw-rw-rw-   0 root         (0) root         (0)      365 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/image/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10627 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/image/resample.py
--rw-rw-rw-   0 root         (0) root         (0)     3216 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/image/roi.py
--rw-rw-rw-   0 root         (0) root         (0)     7087 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/imcp.py
--rw-rw-rw-   0 root         (0) root         (0)     9155 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/memoize.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     2518 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/naninfrange.py
--rw-rw-rw-   0 root         (0) root         (0)    11960 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/notifier.py
--rw-rw-rw-   0 root         (0) root         (0)     2375 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/parse_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19065 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/path.py
--rw-rw-rw-   0 root         (0) root         (0)    13866 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/platform.py
--rw-rw-rw-   0 root         (0) root         (0)    16109 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/run.py
--rw-rw-rw-   0 root         (0) root         (0)    12280 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/tempdir.py
--rw-rw-rw-   0 root         (0) root         (0)     3718 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/utils/weakfuncref.py
--rw-rw-rw-   0 root         (0) root         (0)     4060 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/fsl/wrappers/
--rwxrwxrwx   0 root         (0) root         (0)     4496 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2549 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/bet.py
--rw-rw-rw-   0 root         (0) root         (0)     3387 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/eddy.py
--rwxrwxrwx   0 root         (0) root         (0)     1255 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/epi_reg.py
--rw-rw-rw-   0 root         (0) root         (0)     1652 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/fast.py
--rw-rw-rw-   0 root         (0) root         (0)     3871 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/flirt.py
--rw-rw-rw-   0 root         (0) root         (0)     2917 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/fnirt.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/fsl_anat.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/fsl_sub.py
--rw-rw-rw-   0 root         (0) root         (0)     5966 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/fslmaths.py
--rw-rw-rw-   0 root         (0) root         (0)     8052 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/fslstats.py
--rw-rw-rw-   0 root         (0) root         (0)     3169 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/fugue.py
--rw-rw-rw-   0 root         (0) root         (0)     2426 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/melodic.py
--rw-rw-rw-   0 root         (0) root         (0)     3847 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/misc.py
--rwxrwxrwx   0 root         (0) root         (0)     2265 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/tbss.py
--rw-rw-rw-   0 root         (0) root         (0)    44495 2022-05-28 08:30:56.000000 fslpy-3.9.4/fsl/wrappers/wrapperutils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/fslpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4584 2022-05-28 19:36:53.000000 fslpy-3.9.4/fslpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    64868 2022-05-28 19:36:53.000000 fslpy-3.9.4/fslpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-28 19:36:53.000000 fslpy-3.9.4/fslpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      629 2022-05-28 19:36:53.000000 fslpy-3.9.4/fslpy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      137 2022-05-28 19:36:53.000000 fslpy-3.9.4/fslpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-05-28 19:36:53.000000 fslpy-3.9.4/fslpy.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-05-28 08:30:56.000000 fslpy-3.9.4/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       78 2022-05-28 08:30:56.000000 fslpy-3.9.4/requirements-extra.txt
--rw-rw-rw-   0 root         (0) root         (0)       49 2022-05-28 08:30:56.000000 fslpy-3.9.4/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      596 2022-05-28 19:36:53.000000 fslpy-3.9.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4316 2022-05-28 08:30:56.000000 fslpy-3.9.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)    11639 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     5691 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_assertions.py
--rw-rw-rw-   0 root         (0) root         (0)    11195 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_atlases.py
--rw-rw-rw-   0 root         (0) root         (0)    10695 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_atlases_query.py
--rw-rw-rw-   0 root         (0) root         (0)     5271 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_bids.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_bitmap.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    11995 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_cifti.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_deprecated.py
--rw-rw-rw-   0 root         (0) root         (0)     6675 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_dicom.py
--rw-rw-rw-   0 root         (0) root         (0)     6946 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_dtifit.py
--rw-rw-rw-   0 root         (0) root         (0)      725 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_ensure.py
--rw-rw-rw-   0 root         (0) root         (0)    17244 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_featanalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    15156 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_featdesign.py
--rw-rw-rw-   0 root         (0) root         (0)    10294 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_featimage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/test_filetree/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       93 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/custom.tree
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/extract_vars.tree
--rw-rw-rw-   0 root         (0) root         (0)       46 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/format.tree
--rw-rw-rw-   0 root         (0) root         (0)       17 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/local_parent.tree
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/test_filetree/parent/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/parent/opt_file_test.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/test_filetree/parent/opt_layer_test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/parent/opt_layer_test/opt_file_test.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/parent/opt_layer_test/opt_file_test2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/parent/opt_layer_test/sub_file.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/parent/sub_file.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      173 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/parent.tree
--rw-rw-rw-   0 root         (0) root         (0)    25854 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/test_query.py
--rw-rw-rw-   0 root         (0) root         (0)     9369 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/test_read.py
--rw-rw-rw-   0 root         (0) root         (0)     2403 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/test_registration.py
--rw-rw-rw-   0 root         (0) root         (0)     1977 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_filetree/test_template.py
--rw-rw-rw-   0 root         (0) root         (0)     8340 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_fixlabels.py
--rw-rw-rw-   0 root         (0) root         (0)     8404 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_freesurfer.py
--rw-rw-rw-   0 root         (0) root         (0)     3863 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_fsl_data_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    54167 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_fsl_utils_path.py
--rw-rw-rw-   0 root         (0) root         (0)     9325 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_fslsub.py
--rw-rw-rw-   0 root         (0) root         (0)    13918 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_gifti.py
--rw-rw-rw-   0 root         (0) root         (0)    14892 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_idle.py
--rw-rw-rw-   0 root         (0) root         (0)    49822 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_image.py
--rw-rw-rw-   0 root         (0) root         (0)    11414 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_image_data_access.py
--rw-rw-rw-   0 root         (0) root         (0)    10257 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_image_resample.py
--rw-rw-rw-   0 root         (0) root         (0)     3974 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_image_roi.py
--rw-rw-rw-   0 root         (0) root         (0)     9663 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_immv_imcp.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_importall.py
--rw-rw-rw-   0 root         (0) root         (0)    11761 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_melodicanalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5805 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_melodicimage.py
--rw-rw-rw-   0 root         (0) root         (0)    10319 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_memoize.py
--rw-rw-rw-   0 root         (0) root         (0)    14428 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_mesh.py
--rw-rw-rw-   0 root         (0) root         (0)      616 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_meta.py
--rw-rw-rw-   0 root         (0) root         (0)     2072 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_mghimage.py
--rw-rw-rw-   0 root         (0) root         (0)     2715 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_naninfrange.py
--rw-rw-rw-   0 root         (0) root         (0)     4979 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_notifier.py
--rw-rw-rw-   0 root         (0) root         (0)     4542 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_parse_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5853 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_platform.py
--rw-rw-rw-   0 root         (0) root         (0)    12426 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/test_scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1909 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_atlasq_list_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     5805 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_atlasq_ohi.py
--rw-rw-rw-   0 root         (0) root         (0)    13942 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_atlasq_query.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_fsl_abspath.py
--rw-rw-rw-   0 root         (0) root         (0)     8569 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_fsl_apply_x5.py
--rw-rw-rw-   0 root         (0) root         (0)     6569 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_fsl_convert_x5.py
--rw-rw-rw-   0 root         (0) root         (0)     4619 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_fsl_ents.py
--rw-rw-rw-   0 root         (0) root         (0)     5806 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_imglob.py
--rw-rw-rw-   0 root         (0) root         (0)     3795 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_imln.py
--rw-rw-rw-   0 root         (0) root         (0)    17332 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_immv_imcp.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_imrm.py
--rw-rw-rw-   0 root         (0) root         (0)     2223 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_imtest.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_remove_ext.py
--rw-rw-rw-   0 root         (0) root         (0)     5265 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_resample_image.py
--rw-rw-rw-   0 root         (0) root         (0)     1009 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_scripts/test_vest2text.py
--rw-rw-rw-   0 root         (0) root         (0)    14756 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_tempdir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/test_transform/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18588 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/test_affine.py
--rw-rw-rw-   0 root         (0) root         (0)     4414 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/test_flirt.py
--rw-rw-rw-   0 root         (0) root         (0)     4932 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/test_fnirt.py
--rw-rw-rw-   0 root         (0) root         (0)    20930 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/test_nonlinear.py
--rw-rw-rw-   0 root         (0) root         (0)     3555 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/test_x5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/test_transform/testdata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/test_transform/testdata/nonlinear/
--rw-rw-rw-   0 root         (0) root         (0)     6321 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/nonlinear/coefficientfield.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)   238865 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/nonlinear/displacementfield.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)   248846 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/nonlinear/displacementfield_no_premat.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)    38498 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/nonlinear/ref.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)   286064 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/nonlinear/src.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      189 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/nonlinear/src2ref.mat
--rw-rw-rw-   0 root         (0) root         (0)    58055 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_axisBounds.txt
--rw-rw-rw-   0 root         (0) root         (0)     3734 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_compose.txt
--rw-rw-rw-   0 root         (0) root         (0)     3028 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_concat.txt
--rw-rw-rw-   0 root         (0) root         (0)     2272 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_flirtMatrixToSform.txt
--rw-rw-rw-   0 root         (0) root         (0)     3514 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_invert.txt
--rw-rw-rw-   0 root         (0) root         (0)      527 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_scaleoffsetxform.txt
--rw-rw-rw-   0 root         (0) root         (0)   226337 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_00.txt
--rw-rw-rw-   0 root         (0) root         (0)   226376 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_01.txt
--rw-rw-rw-   0 root         (0) root         (0)   226406 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_02.txt
--rw-rw-rw-   0 root         (0) root         (0)   226264 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_03.txt
--rw-rw-rw-   0 root         (0) root         (0)   226215 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_04.txt
--rw-rw-rw-   0 root         (0) root         (0)   225778 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_05.txt
--rw-rw-rw-   0 root         (0) root         (0)   225869 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_06.txt
--rw-rw-rw-   0 root         (0) root         (0)   225742 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_07.txt
--rw-rw-rw-   0 root         (0) root         (0)   225386 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_08.txt
--rw-rw-rw-   0 root         (0) root         (0)   227019 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_09.txt
--rw-rw-rw-   0 root         (0) root         (0)   229117 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_10.txt
--rw-rw-rw-   0 root         (0) root         (0)   226378 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_11.txt
--rw-rw-rw-   0 root         (0) root         (0)   226339 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_12.txt
--rw-rw-rw-   0 root         (0) root         (0)   230281 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_13.txt
--rw-rw-rw-   0 root         (0) root         (0)   227417 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_14.txt
--rw-rw-rw-   0 root         (0) root         (0)   226350 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_15.txt
--rw-rw-rw-   0 root         (0) root         (0)   228249 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_16.txt
--rw-rw-rw-   0 root         (0) root         (0)   228498 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_17.txt
--rw-rw-rw-   0 root         (0) root         (0)   226585 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_18.txt
--rw-rw-rw-   0 root         (0) root         (0)   228523 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_19.txt
--rw-rw-rw-   0 root         (0) root         (0)   229073 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_20.txt
--rw-rw-rw-   0 root         (0) root         (0)   234060 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_coords.txt
--rw-rw-rw-   0 root         (0) root         (0)     3593 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_version.py
--rw-rw-rw-   0 root         (0) root         (0)     6954 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_vest.py
--rw-rw-rw-   0 root         (0) root         (0)     9624 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_volumelabels.py
--rw-rw-rw-   0 root         (0) root         (0)     2499 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_vtk.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_weakfuncref.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/test_wrappers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_wrappers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3161 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_wrappers/test_fslstats.py
--rwxrwxrwx   0 root         (0) root         (0)    18503 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_wrappers/test_wrappers.py
--rw-rw-rw-   0 root         (0) root         (0)    32958 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/test_wrappers/test_wrapperutils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/
--rw-rw-rw-   0 root         (0) root         (0)      680 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/example.mgz
--rw-rw-rw-   0 root         (0) root         (0)     1746 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/example.shape.gii
--rw-rw-rw-   0 root         (0) root         (0)    16934 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/example.surf.gii
--rw-rw-rw-   0 root         (0) root         (0)     6941 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/example4D.shape.gii
--rw-rw-rw-   0 root         (0) root         (0)    13720 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/example4D_multiple_darrays.shape.gii
--rw-rw-rw-   0 root         (0) root         (0)    26416 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/example_bad1.surf.gii
--rw-rw-rw-   0 root         (0) root         (0)    24184 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/example_bad2.surf.gii
--rw-rw-rw-   0 root         (0) root         (0)    14703 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/example_bad3.surf.gii
--rw-rw-rw-   0 root         (0) root         (0)    18478 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/example_bad4.surf.gii
--rw-rw-rw-   0 root         (0) root         (0)    14703 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/example_bad5.surf.gii
--rw-rw-rw-   0 root         (0) root         (0)     7453 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/example_bad6.surf.gii
--rw-rw-rw-   0 root         (0) root         (0)   386730 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/example_dicom.tbz2
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/absbrainthresh.txt
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/cluster_mask_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/cluster_mask_zstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      257 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/cluster_zstat1.txt
--rw-rw-rw-   0 root         (0) root         (0)      269 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/cluster_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)      505 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/cluster_zstat2.txt
--rw-rw-rw-   0 root         (0) root         (0)      581 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/cluster_zstat2_std.txt
--rw-rw-rw-   0 root         (0) root         (0)     3313 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/confoundevs.txt
--rw-rw-rw-   0 root         (0) root         (0)      415 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/design.con
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/design.frf
--rw-rw-rw-   0 root         (0) root         (0)    10740 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/design.fsf
--rw-rw-rw-   0 root         (0) root         (0)     6283 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/design.mat
--rw-rw-rw-   0 root         (0) root         (0)        2 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/design.min
--rw-rw-rw-   0 root         (0) root         (0)      186 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/design.trg
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       28 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      110 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/lmax_zstat1.txt
--rw-rw-rw-   0 root         (0) root         (0)      166 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/lmax_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)      335 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/lmax_zstat2.txt
--rw-rw-rw-   0 root         (0) root         (0)      491 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/lmax_zstat2_std.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mask.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0000
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0001
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0002
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0003
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0004
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0005
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0006
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0007
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0008
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0009
--rw-rw-rw-   0 root         (0) root         (0)      150 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0010
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0011
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0012
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0013
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0014
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0015
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0016
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0017
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0018
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0019
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0020
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0021
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0022
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0023
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0024
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0025
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0026
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0027
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0028
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0029
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0030
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0031
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0032
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0033
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0034
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0035
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0036
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0037
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0038
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0039
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0040
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0041
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0042
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0043
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0044
--rw-rw-rw-   0 root         (0) root         (0)     3313 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.par
--rw-rw-rw-   0 root         (0) root         (0)      448 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf_abs.rms
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf_abs_mean.rms
--rw-rw-rw-   0 root         (0) root         (0)     3313 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf_final.par
--rw-rw-rw-   0 root         (0) root         (0)      436 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf_rel.rms
--rw-rw-rw-   0 root         (0) root         (0)       10 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf_rel_mean.rms
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mean_func.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      195 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/example_func2highres.mat
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/example_func2highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       87 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/example_func2initial_highres.mat
--rw-rw-rw-   0 root         (0) root         (0)       42 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/example_func2initial_highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      190 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/example_func2standard.mat
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/example_func2standard.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      193 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/highres2example_func.mat
--rw-rw-rw-   0 root         (0) root         (0)      194 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/highres2initial_highres.mat
--rw-rw-rw-   0 root         (0) root         (0)      185 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/highres2standard.mat
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/highres2standard.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/highres_head.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/initial_highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       88 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/initial_highres2example_func.mat
--rw-rw-rw-   0 root         (0) root         (0)      195 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/initial_highres2highres.mat
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/initial_highres2highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       49 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/initial_highres2highres_fast_wmedge.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/initial_highres2highres_fast_wmseg.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      181 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/initial_highres2highres_init.mat
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/standard.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      191 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/standard2example_func.mat
--rw-rw-rw-   0 root         (0) root         (0)      189 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg/standard2highres.mat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       27 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/mask.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/mean_func.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/reg/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/reg/highres.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/stats/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/stats/cope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/stats/cope2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/stats/varcope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/stats/varcope2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/rendered_thresh_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/rendered_thresh_zstat2.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/cope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/cope2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/dof
--rw-rw-rw-   0 root         (0) root         (0)      189 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/logfile
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/pe1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/pe10.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/pe2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/pe3.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/pe4.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/pe5.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/pe6.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/pe7.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/pe8.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/pe9.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/res4d.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/sigmasquareds.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/smoothness
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/threshac1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/tstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/tstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/varcope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/varcope2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/stats/zstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/thresh_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/thresh_zstat1.vol
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/thresh_zstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/thresh_zstat2.vol
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/absbrainthresh.txt
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/cluster_mask_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/cluster_mask_zstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      319 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/cluster_zstat1.txt
--rw-rw-rw-   0 root         (0) root         (0)      344 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/cluster_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)      313 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/cluster_zstat2.txt
--rw-rw-rw-   0 root         (0) root         (0)      338 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/cluster_zstat2_std.txt
--rw-rw-rw-   0 root         (0) root         (0)     3299 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/confoundevs.txt
--rw-rw-rw-   0 root         (0) root         (0)      441 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/design.con
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/design.frf
--rw-rw-rw-   0 root         (0) root         (0)    11227 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/design.fsf
--rw-rw-rw-   0 root         (0) root         (0)     6904 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/design.mat
--rw-rw-rw-   0 root         (0) root         (0)        2 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/design.min
--rw-rw-rw-   0 root         (0) root         (0)      188 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/design.trg
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/designInputVoxelwiseEV3.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       28 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/designVoxelwiseEV3.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       28 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      186 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/lmax_zstat1.txt
--rw-rw-rw-   0 root         (0) root         (0)      279 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/lmax_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)      186 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/lmax_zstat2.txt
--rw-rw-rw-   0 root         (0) root         (0)      269 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/lmax_zstat2_std.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mask.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0000
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0001
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0002
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0003
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0004
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0005
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0006
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0007
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0008
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0009
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0010
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0011
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0012
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0013
--rw-rw-rw-   0 root         (0) root         (0)      150 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0014
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0015
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0016
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0017
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0018
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0019
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0020
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0021
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0022
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0023
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0024
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0025
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0026
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0027
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0028
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0029
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0030
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0031
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0032
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0033
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0034
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0035
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0036
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0037
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0038
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0039
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0040
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0041
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0042
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0043
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0044
--rw-rw-rw-   0 root         (0) root         (0)     3299 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.par
--rw-rw-rw-   0 root         (0) root         (0)      442 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf_abs.rms
--rw-rw-rw-   0 root         (0) root         (0)       10 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf_abs_mean.rms
--rw-rw-rw-   0 root         (0) root         (0)     3299 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf_final.par
--rw-rw-rw-   0 root         (0) root         (0)      434 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf_rel.rms
--rw-rw-rw-   0 root         (0) root         (0)       10 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf_rel_mean.rms
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mean_func.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      195 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/example_func2highres.mat
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/example_func2highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       87 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/example_func2initial_highres.mat
--rw-rw-rw-   0 root         (0) root         (0)       42 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/example_func2initial_highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      188 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/example_func2standard.mat
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/example_func2standard.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      194 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/highres2example_func.mat
--rw-rw-rw-   0 root         (0) root         (0)      194 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/highres2initial_highres.mat
--rw-rw-rw-   0 root         (0) root         (0)      185 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/highres2standard.mat
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/highres2standard.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/highres_head.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/initial_highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       88 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/initial_highres2example_func.mat
--rw-rw-rw-   0 root         (0) root         (0)      195 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/initial_highres2highres.mat
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/initial_highres2highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       49 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/initial_highres2highres_fast_wmedge.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/initial_highres2highres_fast_wmseg.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      181 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/initial_highres2highres_init.mat
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/standard.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      191 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/standard2example_func.mat
--rw-rw-rw-   0 root         (0) root         (0)      189 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/reg/standard2highres.mat
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/rendered_thresh_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/rendered_thresh_zstat2.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/cope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/cope2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/dof
--rw-rw-rw-   0 root         (0) root         (0)      222 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/logfile
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/pe1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/pe10.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/pe11.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/pe2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/pe3.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/pe4.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/pe5.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/pe6.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/pe7.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/pe8.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/pe9.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/res4d.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/sigmasquareds.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       39 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/smoothness
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/threshac1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/tstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/tstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/varcope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/varcope2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/stats/zstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/thresh_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/thresh_zstat1.vol
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/thresh_zstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/thresh_zstat2.vol
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/InputconfoundEV1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/absbrainthresh.txt
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/cluster_mask_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/cluster_mask_zstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      369 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/cluster_zstat1.txt
--rw-rw-rw-   0 root         (0) root         (0)      507 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/cluster_zstat2.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/confoundEV1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)    18118 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/confoundevs.txt
--rw-rw-rw-   0 root         (0) root         (0)      987 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/design.con
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/design.frf
--rw-rw-rw-   0 root         (0) root         (0)    10095 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/design.fsf
--rw-rw-rw-   0 root         (0) root         (0)    20020 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/design.mat
--rw-rw-rw-   0 root         (0) root         (0)        2 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/design.min
--rw-rw-rw-   0 root         (0) root         (0)      265 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/design.trg
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       28 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      108 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/lmax_zstat1.txt
--rw-rw-rw-   0 root         (0) root         (0)      304 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/lmax_zstat2.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mask.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0000
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0001
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0002
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0003
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0004
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0005
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0006
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0007
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0008
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0009
--rw-rw-rw-   0 root         (0) root         (0)      150 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0010
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0011
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0012
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0013
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0014
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0015
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0016
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0017
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0018
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0019
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0020
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0021
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0022
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0023
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0024
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0025
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0026
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0027
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0028
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0029
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0030
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0031
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0032
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0033
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0034
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0035
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0036
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0037
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0038
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0039
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0040
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0041
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0042
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0043
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0044
--rw-rw-rw-   0 root         (0) root         (0)     3313 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.par
--rw-rw-rw-   0 root         (0) root         (0)      448 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_abs.rms
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_abs_mean.rms
--rw-rw-rw-   0 root         (0) root         (0)    13185 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_diff.dat
--rw-rw-rw-   0 root         (0) root         (0)    16498 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_final.par
--rw-rw-rw-   0 root         (0) root         (0)      436 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_rel.rms
--rw-rw-rw-   0 root         (0) root         (0)       10 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_rel_mean.rms
--rw-rw-rw-   0 root         (0) root         (0)      450 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/meanConfounds.dat
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mean_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/rendered_thresh_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/rendered_thresh_zstat2.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/cope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/cope2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/dof
--rw-rw-rw-   0 root         (0) root         (0)      215 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/logfile
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe10.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe11.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe12.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe13.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe14.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe15.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe16.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe17.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe18.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe19.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe20.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe21.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe22.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe23.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe24.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe25.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe26.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe27.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe28.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe29.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe3.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe30.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe31.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe32.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe4.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe5.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe6.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe7.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe8.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/pe9.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/res4d.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/sigmasquareds.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       39 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/smoothness
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/threshac1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/tstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/tstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/varcope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/varcope2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/stats/zstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/thresh_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/thresh_zstat1.vol
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/thresh_zstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/thresh_zstat2.vol
--rw-rw-rw-   0 root         (0) root         (0)       11 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/vef.dat
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/ven.dat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/absbrainthresh.txt
--rw-rw-rw-   0 root         (0) root         (0)      258 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/design.con
--rw-rw-rw-   0 root         (0) root         (0)        8 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/design.frf
--rw-rw-rw-   0 root         (0) root         (0)     9916 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/design.fsf
--rw-rw-rw-   0 root         (0) root         (0)     2561 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/design.mat
--rw-rw-rw-   0 root         (0) root         (0)        2 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/design.min
--rw-rw-rw-   0 root         (0) root         (0)      174 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/design.trg
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       28 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       14 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mask.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0000
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0001
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0002
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0003
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0004
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0005
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0006
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0007
--rw-rw-rw-   0 root         (0) root         (0)      151 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0008
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0009
--rw-rw-rw-   0 root         (0) root         (0)      150 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0010
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0011
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0012
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0013
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0014
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0015
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0016
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0017
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0018
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0019
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0020
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0021
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0022
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0023
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0024
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0025
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0026
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0027
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0028
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0029
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0030
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0031
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0032
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0033
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0034
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0035
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0036
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0037
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0038
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0039
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0040
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0041
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0042
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0043
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0044
--rw-rw-rw-   0 root         (0) root         (0)     3313 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.par
--rw-rw-rw-   0 root         (0) root         (0)      448 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf_abs.rms
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf_abs_mean.rms
--rw-rw-rw-   0 root         (0) root         (0)      436 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf_rel.rms
--rw-rw-rw-   0 root         (0) root         (0)       10 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf_rel_mean.rms
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mean_func.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      195 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/example_func2highres.mat
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/example_func2highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       87 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/example_func2initial_highres.mat
--rw-rw-rw-   0 root         (0) root         (0)       42 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/example_func2initial_highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      190 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/example_func2standard.mat
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/example_func2standard.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      193 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/highres2example_func.mat
--rw-rw-rw-   0 root         (0) root         (0)      194 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/highres2initial_highres.mat
--rw-rw-rw-   0 root         (0) root         (0)      185 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/highres2standard.mat
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/highres2standard.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/highres_head.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/initial_highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       88 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/initial_highres2example_func.mat
--rw-rw-rw-   0 root         (0) root         (0)      195 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/initial_highres2highres.mat
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/initial_highres2highres.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       49 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/initial_highres2highres_fast_wmedge.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/initial_highres2highres_fast_wmseg.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      181 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/initial_highres2highres_init.mat
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/standard.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      191 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/standard2example_func.mat
--rw-rw-rw-   0 root         (0) root         (0)      189 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/reg/standard2highres.mat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/absbrainthresh.txt
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/cluster_mask_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/cluster_mask_zstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      252 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/cluster_zstat1.txt
--rw-rw-rw-   0 root         (0) root         (0)      247 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/cluster_zstat2.txt
--rw-rw-rw-   0 root         (0) root         (0)      258 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/design.con
--rw-rw-rw-   0 root         (0) root         (0)        8 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/design.frf
--rw-rw-rw-   0 root         (0) root         (0)     9670 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/design.fsf
--rw-rw-rw-   0 root         (0) root         (0)     2574 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/design.mat
--rw-rw-rw-   0 root         (0) root         (0)        2 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/design.min
--rw-rw-rw-   0 root         (0) root         (0)      174 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/design.trg
--rw-rw-rw-   0 root         (0) root         (0)      391 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)    12354 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       62 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/lmax_zstat1.txt
--rw-rw-rw-   0 root         (0) root         (0)       49 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/lmax_zstat2.txt
--rw-rw-rw-   0 root         (0) root         (0)      112 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/mask.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      435 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/mean_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      451 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/rendered_thresh_zstat1.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/
--rw-rw-rw-   0 root         (0) root         (0)      448 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/cope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      451 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/cope2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/dof
--rw-rw-rw-   0 root         (0) root         (0)      189 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/logfile
--rw-rw-rw-   0 root         (0) root         (0)      448 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/pe1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      450 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/pe2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      451 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/pe3.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      452 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/pe4.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)    13580 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/res4d.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      442 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/sigmasquareds.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/smoothness
--rw-rw-rw-   0 root         (0) root         (0)     1442 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/threshac1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      448 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/tstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      447 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/tstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      444 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/varcope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      444 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/varcope2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      446 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/zstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      179 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/thresh_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        3 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/thresh_zstat1.vol
--rw-rw-rw-   0 root         (0) root         (0)      170 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/thresh_zstat2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        3 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/thresh_zstat2.vol
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/bg_image.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/
--rwxrwxrwx   0 root         (0) root         (0)      187 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/.flame
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/cluster_mask_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      663 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/cluster_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)      129 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/design.con
--rw-rw-rw-   0 root         (0) root         (0)     7861 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/design.fsf
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/design.grp
--rw-rw-rw-   0 root         (0) root         (0)       14 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/design.lcon
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/design.lev
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/design.mat
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       39 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      707 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/lmax_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/mask.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/mean_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/rendered_thresh_zstat1.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/cope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        2 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/dof
--rw-rw-rw-   0 root         (0) root         (0)      233 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/logfile
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/mean_random_effects_var1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/pe1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/res4d.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       41 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/smoothness
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/tdof_t1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/tstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/varcope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/weights1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/zflame1lowertstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/zflame1uppertstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/thresh_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/thresh_zstat1.vol
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/var_filtered_func_data.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/
--rwxrwxrwx   0 root         (0) root         (0)      187 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/.flame
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/cluster_mask_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      251 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/cluster_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)      129 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/design.con
--rw-rw-rw-   0 root         (0) root         (0)     7861 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/design.fsf
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/design.grp
--rw-rw-rw-   0 root         (0) root         (0)       14 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/design.lcon
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/design.lev
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/design.mat
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       39 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      124 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/lmax_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/mask.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/mean_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/rendered_thresh_zstat1.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/cope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        2 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/dof
--rw-rw-rw-   0 root         (0) root         (0)      233 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/logfile
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/mean_random_effects_var1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/pe1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/res4d.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/smoothness
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/tdof_t1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/tstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/varcope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/weights1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/zflame1lowertstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/zflame1uppertstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/thresh_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/thresh_zstat1.vol
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/var_filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      129 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/design.con
--rw-rw-rw-   0 root         (0) root         (0)     7861 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/design.fsf
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/design.grp
--rw-rw-rw-   0 root         (0) root         (0)       28 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/design.lcon
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/design.mat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/inputreg/
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/inputreg/masksum.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/inputreg/masksum_overlay.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/inputreg/maskunique.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/inputreg/maskunique_overlay.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       14 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/mask.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/mean_func.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/bg_image.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/
--rwxrwxrwx   0 root         (0) root         (0)      327 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/.flame
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/cluster_mask_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      831 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/cluster_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/design.con
--rw-rw-rw-   0 root         (0) root         (0)     8071 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/design.fsf
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/design.grp
--rw-rw-rw-   0 root         (0) root         (0)       14 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/design.lcon
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/design.lev
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/design.mat
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       39 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      766 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/lmax_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/mask.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/mean_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/rendered_thresh_zstat1.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/cope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        2 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/dof
--rw-rw-rw-   0 root         (0) root         (0)      373 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/logfile
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/mean_random_effects_var1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/pe1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/pe2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/res4d.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/smoothness
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/tdof_t1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/tstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/varcope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/weights1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/zflame1lowertstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/zflame1uppertstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/thresh_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/thresh_zstat1.vol
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/var_filtered_func_data.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/
--rwxrwxrwx   0 root         (0) root         (0)      327 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/.flame
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/cluster_mask_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     2030 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/cluster_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/design.con
--rw-rw-rw-   0 root         (0) root         (0)     8071 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/design.fsf
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/design.grp
--rw-rw-rw-   0 root         (0) root         (0)       14 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/design.lcon
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/design.lev
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/design.mat
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       39 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     2340 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/lmax_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/mask.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/mean_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/rendered_thresh_zstat1.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/cope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        2 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/dof
--rw-rw-rw-   0 root         (0) root         (0)      373 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/logfile
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/mean_random_effects_var1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/pe1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/pe2.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/res4d.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/smoothness
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/tdof_t1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/tstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/varcope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/weights1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/zflame1lowertstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/zflame1uppertstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/thresh_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/thresh_zstat1.vol
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/var_filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/design.con
--rw-rw-rw-   0 root         (0) root         (0)     8071 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/design.fsf
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/design.grp
--rw-rw-rw-   0 root         (0) root         (0)       28 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/design.lcon
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/design.mat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/inputreg/
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/inputreg/masksum.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/inputreg/masksum_overlay.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/inputreg/maskunique.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/inputreg/maskunique_overlay.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       14 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/mask.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/mean_func.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/
--rw-rw-rw-   0 root         (0) root         (0)     3663 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/bg_image.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/
--rwxrwxrwx   0 root         (0) root         (0)      215 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/.flame
--rw-rw-rw-   0 root         (0) root         (0)      253 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/cluster_mask_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      522 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/cluster_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)      129 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/design.con
--rw-rw-rw-   0 root         (0) root         (0)     7891 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/design.fsf
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/design.grp
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/design.lcon
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/design.lev
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/design.mat
--rw-rw-rw-   0 root         (0) root         (0)     3663 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)    11136 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      527 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/lmax_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/mask.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     3644 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/mean_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     3726 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/rendered_thresh_zstat1.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/
--rw-rw-rw-   0 root         (0) root         (0)     3839 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/cope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        2 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/dof
--rw-rw-rw-   0 root         (0) root         (0)      262 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/logfile
--rw-rw-rw-   0 root         (0) root         (0)      138 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/mean_random_effects_var1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     3839 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/pe1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)    10615 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/res4d.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       41 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/smoothness
--rw-rw-rw-   0 root         (0) root         (0)      142 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/tdof_t1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     3839 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/tstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     3748 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/varcope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      160 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/weights1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      138 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/zflame1lowertstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      138 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/zflame1uppertstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     3832 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      159 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/tdof_filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     2886 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/thresh_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/thresh_zstat1.vol
--rw-rw-rw-   0 root         (0) root         (0)    10862 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/var_filtered_func_data.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/
--rwxrwxrwx   0 root         (0) root         (0)      215 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/.flame
--rw-rw-rw-   0 root         (0) root         (0)      138 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/cluster_mask_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      457 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/cluster_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)      129 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/design.con
--rw-rw-rw-   0 root         (0) root         (0)     7891 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/design.fsf
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/design.grp
--rw-rw-rw-   0 root         (0) root         (0)        8 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/design.lcon
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/design.lev
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/design.mat
--rw-rw-rw-   0 root         (0) root         (0)     3663 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/example_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)    11247 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      335 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/lmax_zstat1_std.txt
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/mask.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     3644 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/mean_func.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     3760 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/rendered_thresh_zstat1.nii.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 19:36:53.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/
--rw-rw-rw-   0 root         (0) root         (0)     3890 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/cope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        2 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/dof
--rw-rw-rw-   0 root         (0) root         (0)      262 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/logfile
--rw-rw-rw-   0 root         (0) root         (0)      138 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/mean_random_effects_var1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     3890 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/pe1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)    10802 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/res4d.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)       41 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/smoothness
--rw-rw-rw-   0 root         (0) root         (0)      142 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/tdof_t1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     3889 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/tstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     3755 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/varcope1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      160 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/weights1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      138 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/zflame1lowertstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      138 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/zflame1uppertstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     3893 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      159 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/tdof_filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      301 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/thresh_zstat1.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/thresh_zstat1.vol
--rw-rw-rw-   0 root         (0) root         (0)    10871 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/var_filtered_func_data.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)      129 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/design.con
--rw-rw-rw-   0 root         (0) root         (0)     7891 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/design.fsf
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/design.grp
--rw-rw-rw-   0 root         (0) root         (0)       17 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/design.lcon
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/design.mat
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/mask.nii.gz
--rw-rw-rw-   0 root         (0) root         (0)     3644 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/mean_func.nii.gz
--rwxrwxrwx   0 root         (0) root         (0)    32615 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_mesh.vtk
--rw-rw-rw-   0 root         (0) root         (0)     1870 2022-05-28 08:30:56.000000 fslpy-3.9.4/tests/testdata/test_mesh_data.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/
+-rw-rw-rw-   0 root         (0) root         (0)      365 2022-06-02 20:10:03.000000 fslpy-3.9.5/AUTHOR
+-rw-rw-rw-   0 root         (0) root         (0)    47960 2022-06-02 20:10:03.000000 fslpy-3.9.5/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)       53 2022-06-02 20:10:03.000000 fslpy-3.9.5/COPYRIGHT
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-06-02 20:10:03.000000 fslpy-3.9.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      370 2022-06-02 20:10:03.000000 fslpy-3.9.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4584 2022-06-02 22:44:23.000000 fslpy-3.9.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3863 2022-06-02 20:10:03.000000 fslpy-3.9.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/doc/_static/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/_static/theme_overrides.css
+-rw-rw-rw-   0 root         (0) root         (0)       83 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11175 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     7022 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)      133 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.atlases.rst
+-rw-rw-rw-   0 root         (0) root         (0)      130 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.bitmap.rst
+-rw-rw-rw-   0 root         (0) root         (0)      127 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.cifti.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.constants.rst
+-rw-rw-rw-   0 root         (0) root         (0)      127 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.dicom.rst
+-rw-rw-rw-   0 root         (0) root         (0)      130 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.dtifit.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.featanalysis.rst
+-rw-rw-rw-   0 root         (0) root         (0)      142 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.featdesign.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.featimage.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.fixlabels.rst
+-rw-rw-rw-   0 root         (0) root         (0)      142 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.freesurfer.rst
+-rw-rw-rw-   0 root         (0) root         (0)      127 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.gifti.rst
+-rw-rw-rw-   0 root         (0) root         (0)      127 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.image.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.imagewrapper.rst
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.melodicanalysis.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.melodicimage.rst
+-rw-rw-rw-   0 root         (0) root         (0)      124 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.mesh.rst
+-rw-rw-rw-   0 root         (0) root         (0)      136 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.mghimage.rst
+-rw-rw-rw-   0 root         (0) root         (0)      595 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.rst
+-rw-rw-rw-   0 root         (0) root         (0)      127 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.utils.rst
+-rw-rw-rw-   0 root         (0) root         (0)      124 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.vest.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.volumelabels.rst
+-rw-rw-rw-   0 root         (0) root         (0)      121 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.data.vtk.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.Text2Vest.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.Vest2Text.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.atlasq.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.fsl_abspath.rst
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.fsl_apply_x5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      163 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.fsl_convert_x5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      145 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.fsl_ents.rst
+-rw-rw-rw-   0 root         (0) root         (0)      133 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.imcp.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.imglob.rst
+-rw-rw-rw-   0 root         (0) root         (0)      133 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.imln.rst
+-rw-rw-rw-   0 root         (0) root         (0)      133 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.immv.rst
+-rw-rw-rw-   0 root         (0) root         (0)      133 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.imrm.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.imtest.rst
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.remove_ext.rst
+-rw-rw-rw-   0 root         (0) root         (0)      163 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.resample_image.rst
+-rw-rw-rw-   0 root         (0) root         (0)      740 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.scripts.rst
+-rw-rw-rw-   0 root         (0) root         (0)      145 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.transform.affine.rst
+-rw-rw-rw-   0 root         (0) root         (0)      142 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.transform.flirt.rst
+-rw-rw-rw-   0 root         (0) root         (0)      142 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.transform.fnirt.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.transform.nonlinear.rst
+-rw-rw-rw-   0 root         (0) root         (0)      268 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.transform.rst
+-rw-rw-rw-   0 root         (0) root         (0)      133 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.transform.x5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      145 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.assertions.rst
+-rw-rw-rw-   0 root         (0) root         (0)      127 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.bids.rst
+-rw-rw-rw-   0 root         (0) root         (0)      130 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.cache.rst
+-rw-rw-rw-   0 root         (0) root         (0)      145 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.deprecated.rst
+-rw-rw-rw-   0 root         (0) root         (0)      133 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.ensure.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.filetree.filetree.rst
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.filetree.parse.rst
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.filetree.query.rst
+-rw-rw-rw-   0 root         (0) root         (0)      281 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.filetree.rst
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.filetree.utils.rst
+-rw-rw-rw-   0 root         (0) root         (0)      133 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.fslsub.rst
+-rw-rw-rw-   0 root         (0) root         (0)      127 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.idle.rst
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.image.resample.rst
+-rw-rw-rw-   0 root         (0) root         (0)      142 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.image.roi.rst
+-rw-rw-rw-   0 root         (0) root         (0)      208 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.image.rst
+-rw-rw-rw-   0 root         (0) root         (0)      127 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.imcp.rst
+-rw-rw-rw-   0 root         (0) root         (0)      136 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.memoize.rst
+-rw-rw-rw-   0 root         (0) root         (0)      127 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.meta.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.naninfrange.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.notifier.rst
+-rw-rw-rw-   0 root         (0) root         (0)      145 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.parse_data.rst
+-rw-rw-rw-   0 root         (0) root         (0)      127 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.path.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.platform.rst
+-rw-rw-rw-   0 root         (0) root         (0)      576 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.rst
+-rw-rw-rw-   0 root         (0) root         (0)      124 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.run.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.settings.rst
+-rw-rw-rw-   0 root         (0) root         (0)      136 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.tempdir.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.utils.weakfuncref.rst
+-rw-rw-rw-   0 root         (0) root         (0)      118 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.version.rst
+-rw-rw-rw-   0 root         (0) root         (0)      133 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.bet.rst
+-rw-rw-rw-   0 root         (0) root         (0)      136 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.eddy.rst
+-rw-rw-rw-   0 root         (0) root         (0)      145 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.epi_reg.rst
+-rw-rw-rw-   0 root         (0) root         (0)      136 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.fast.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.flirt.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.fnirt.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.fsl_anat.rst
+-rw-rw-rw-   0 root         (0) root         (0)      145 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.fsl_sub.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.fslmaths.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.fslstats.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.fugue.rst
+-rw-rw-rw-   0 root         (0) root         (0)      145 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.melodic.rst
+-rw-rw-rw-   0 root         (0) root         (0)      136 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.misc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      494 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.rst
+-rw-rw-rw-   0 root         (0) root         (0)      136 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.tbss.rst
+-rw-rw-rw-   0 root         (0) root         (0)      160 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/fsl.wrappers.wrapperutils.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/doc/images/
+-rw-rw-rw-   0 root         (0) root         (0)    99363 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/images/fnirt_coefficient_field.png
+-rw-rw-rw-   0 root         (0) root         (0)   368845 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/images/fnirt_coefficient_field.xcf
+-rw-rw-rw-   0 root         (0) root         (0)    83903 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/images/fnirt_warp_field.png
+-rw-rw-rw-   0 root         (0) root         (0)   209568 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/images/fnirt_warp_field.xcf
+-rw-rw-rw-   0 root         (0) root         (0)    67938 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/images/nonlinear_registration_process.png
+-rw-rw-rw-   0 root         (0) root         (0)   300073 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/images/nonlinear_registration_process.xcf
+-rw-rw-rw-   0 root         (0) root         (0)     2655 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-06-02 20:10:03.000000 fslpy-3.9.5/doc/mock_modules.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/fsl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/fsl/data/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39304 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/atlases.py
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/bitmap.py
+-rw-rw-rw-   0 root         (0) root         (0)    20171 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/cifti.py
+-rw-rw-rw-   0 root         (0) root         (0)     4720 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     8870 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/dicom.py
+-rw-rw-rw-   0 root         (0) root         (0)    10079 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/dtifit.py
+-rw-rw-rw-   0 root         (0) root         (0)    18029 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/featanalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    25901 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/featdesign.py
+-rw-rw-rw-   0 root         (0) root         (0)    12212 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/featimage.py
+-rw-rw-rw-   0 root         (0) root         (0)    10913 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/fixlabels.py
+-rw-rw-rw-   0 root         (0) root         (0)    13044 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/freesurfer.py
+-rw-rw-rw-   0 root         (0) root         (0)    13511 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/gifti.py
+-rw-rw-rw-   0 root         (0) root         (0)    71521 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/image.py
+-rw-rw-rw-   0 root         (0) root         (0)    42105 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/imagewrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     5611 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/melodicanalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4804 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/melodicimage.py
+-rw-rw-rw-   0 root         (0) root         (0)    24326 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     5483 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/mghimage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3540 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4105 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/vest.py
+-rw-rw-rw-   0 root         (0) root         (0)     9686 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/volumelabels.py
+-rw-rw-rw-   0 root         (0) root         (0)     5156 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/data/vtk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/fsl/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      789 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/Text2Vest.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/Vest2Text.py
+-rw-rw-rw-   0 root         (0) root         (0)    24552 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/atlasq.py
+-rw-rw-rw-   0 root         (0) root         (0)      564 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/fsl_abspath.py
+-rw-rw-rw-   0 root         (0) root         (0)     4403 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/fsl_apply_x5.py
+-rw-rw-rw-   0 root         (0) root         (0)     7014 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/fsl_convert_x5.py
+-rw-rw-rw-   0 root         (0) root         (0)     6846 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/fsl_ents.py
+-rwxrwxrwx   0 root         (0) root         (0)     1822 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/imcp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4008 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/imglob.py
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/imln.py
+-rwxrwxrwx   0 root         (0) root         (0)     1815 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/immv.py
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/imrm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1634 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/imtest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/remove_ext.py
+-rw-rw-rw-   0 root         (0) root         (0)     6495 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/scripts/resample_image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/fsl/transform/
+-rw-rw-rw-   0 root         (0) root         (0)      490 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/transform/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19369 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/transform/affine.py
+-rw-rw-rw-   0 root         (0) root         (0)     5792 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/transform/flirt.py
+-rw-rw-rw-   0 root         (0) root         (0)    15024 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/transform/fnirt.py
+-rw-rw-rw-   0 root         (0) root         (0)    31907 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/transform/nonlinear.py
+-rw-rw-rw-   0 root         (0) root         (0)    22936 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/transform/x5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/fsl/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4072 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/assertions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7187 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/bids.py
+-rw-rw-rw-   0 root         (0) root         (0)     5114 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/deprecated.py
+-rw-rw-rw-   0 root         (0) root         (0)      593 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/ensure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/fsl/utils/filetree/
+-rw-rw-rw-   0 root         (0) root         (0)    11925 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22770 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/filetree.py
+-rw-rw-rw-   0 root         (0) root         (0)     4227 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)    13571 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/fsl/utils/filetree/trees/
+-rw-rw-rw-   0 root         (0) root         (0)      925 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/BedpostX.tree
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/Diffusion.tree
+-rw-rw-rw-   0 root         (0) root         (0)     1825 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/HCP_Surface.tree
+-rw-rw-rw-   0 root         (0) root         (0)     2096 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/HCP_directory.tree
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/ProbtrackX.tree
+-rw-rw-rw-   0 root         (0) root         (0)       82 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/bet.tree
+-rw-rw-rw-   0 root         (0) root         (0)     3307 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/bids_raw.tree
+-rw-rw-rw-   0 root         (0) root         (0)      498 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/dti.tree
+-rw-rw-rw-   0 root         (0) root         (0)      760 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/eddy.tree
+-rw-rw-rw-   0 root         (0) root         (0)      188 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/epi_reg.tree
+-rw-rw-rw-   0 root         (0) root         (0)      332 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/fast.tree
+-rw-rw-rw-   0 root         (0) root         (0)      446 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/feat.tree
+-rw-rw-rw-   0 root         (0) root         (0)      155 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/feat_reg.tree
+-rw-rw-rw-   0 root         (0) root         (0)      223 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/feat_stats.tree
+-rw-rw-rw-   0 root         (0) root         (0)     2199 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/freesurfer.tree
+-rw-rw-rw-   0 root         (0) root         (0)     1653 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/fsl_anat.tree
+-rw-rw-rw-   0 root         (0) root         (0)       52 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/gfeat.tree
+-rw-rw-rw-   0 root         (0) root         (0)      618 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/tbss.tree
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/topup.tree
+-rw-rw-rw-   0 root         (0) root         (0)      457 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/trees/vbm.tree
+-rw-rw-rw-   0 root         (0) root         (0)    14258 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/filetree/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    19508 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/fslsub.py
+-rw-rw-rw-   0 root         (0) root         (0)    36831 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/idle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/fsl/utils/image/
+-rw-rw-rw-   0 root         (0) root         (0)      365 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/image/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10627 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/image/resample.py
+-rw-rw-rw-   0 root         (0) root         (0)     3216 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/image/roi.py
+-rw-rw-rw-   0 root         (0) root         (0)     7087 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/imcp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9155 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/memoize.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     2518 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/naninfrange.py
+-rw-rw-rw-   0 root         (0) root         (0)    11960 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/notifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     2375 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/parse_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    19065 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/path.py
+-rw-rw-rw-   0 root         (0) root         (0)    13866 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)    16109 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/run.py
+-rw-rw-rw-   0 root         (0) root         (0)    12280 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/tempdir.py
+-rw-rw-rw-   0 root         (0) root         (0)     3718 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/utils/weakfuncref.py
+-rw-rw-rw-   0 root         (0) root         (0)     4060 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/fsl/wrappers/
+-rwxrwxrwx   0 root         (0) root         (0)     5052 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/bet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3387 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/eddy.py
+-rwxrwxrwx   0 root         (0) root         (0)     1255 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/epi_reg.py
+-rw-rw-rw-   0 root         (0) root         (0)     1652 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/fast.py
+-rw-rw-rw-   0 root         (0) root         (0)     3871 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/flirt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2917 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/fnirt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/fsl_anat.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/fsl_sub.py
+-rw-rw-rw-   0 root         (0) root         (0)     5966 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/fslmaths.py
+-rw-rw-rw-   0 root         (0) root         (0)     8052 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/fslstats.py
+-rw-rw-rw-   0 root         (0) root         (0)     3169 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/fugue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2426 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/melodic.py
+-rw-rw-rw-   0 root         (0) root         (0)     3847 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/misc.py
+-rwxrwxrwx   0 root         (0) root         (0)     2265 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/tbss.py
+-rw-rw-rw-   0 root         (0) root         (0)    44934 2022-06-02 20:10:03.000000 fslpy-3.9.5/fsl/wrappers/wrapperutils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/fslpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4584 2022-06-02 22:44:23.000000 fslpy-3.9.5/fslpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    64868 2022-06-02 22:44:23.000000 fslpy-3.9.5/fslpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-02 22:44:23.000000 fslpy-3.9.5/fslpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      629 2022-06-02 22:44:23.000000 fslpy-3.9.5/fslpy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      137 2022-06-02 22:44:23.000000 fslpy-3.9.5/fslpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2022-06-02 22:44:23.000000 fslpy-3.9.5/fslpy.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-06-02 20:10:03.000000 fslpy-3.9.5/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       78 2022-06-02 20:10:03.000000 fslpy-3.9.5/requirements-extra.txt
+-rw-rw-rw-   0 root         (0) root         (0)       49 2022-06-02 20:10:03.000000 fslpy-3.9.5/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      596 2022-06-02 22:44:23.000000 fslpy-3.9.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4316 2022-06-02 20:10:03.000000 fslpy-3.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    11639 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      729 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5691 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_assertions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11195 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_atlases.py
+-rw-rw-rw-   0 root         (0) root         (0)    10695 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_atlases_query.py
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_bids.py
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_bitmap.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    11995 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_cifti.py
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_deprecated.py
+-rw-rw-rw-   0 root         (0) root         (0)     6675 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_dicom.py
+-rw-rw-rw-   0 root         (0) root         (0)     6946 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_dtifit.py
+-rw-rw-rw-   0 root         (0) root         (0)      896 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_ensure.py
+-rw-rw-rw-   0 root         (0) root         (0)    17244 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_featanalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    15156 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_featdesign.py
+-rw-rw-rw-   0 root         (0) root         (0)    10294 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_featimage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/test_filetree/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       93 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/custom.tree
+-rw-rw-rw-   0 root         (0) root         (0)       57 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/extract_vars.tree
+-rw-rw-rw-   0 root         (0) root         (0)       46 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/format.tree
+-rw-rw-rw-   0 root         (0) root         (0)       17 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/local_parent.tree
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/test_filetree/parent/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/parent/opt_file_test.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/test_filetree/parent/opt_layer_test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/parent/opt_layer_test/opt_file_test.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/parent/opt_layer_test/opt_file_test2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/parent/opt_layer_test/sub_file.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/parent/sub_file.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      173 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/parent.tree
+-rw-rw-rw-   0 root         (0) root         (0)    25854 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/test_query.py
+-rw-rw-rw-   0 root         (0) root         (0)     9369 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/test_read.py
+-rw-rw-rw-   0 root         (0) root         (0)     2403 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/test_registration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1977 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_filetree/test_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     8340 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_fixlabels.py
+-rw-rw-rw-   0 root         (0) root         (0)     8404 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_freesurfer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3863 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_fsl_data_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    54167 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_fsl_utils_path.py
+-rw-rw-rw-   0 root         (0) root         (0)     9325 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_fslsub.py
+-rw-rw-rw-   0 root         (0) root         (0)    13918 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_gifti.py
+-rw-rw-rw-   0 root         (0) root         (0)    14892 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_idle.py
+-rw-rw-rw-   0 root         (0) root         (0)    49822 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_image.py
+-rw-rw-rw-   0 root         (0) root         (0)    11414 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_image_data_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    10257 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_image_resample.py
+-rw-rw-rw-   0 root         (0) root         (0)     3974 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_image_roi.py
+-rw-rw-rw-   0 root         (0) root         (0)     9663 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_immv_imcp.py
+-rw-rw-rw-   0 root         (0) root         (0)      530 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_importall.py
+-rw-rw-rw-   0 root         (0) root         (0)    11761 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_melodicanalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5805 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_melodicimage.py
+-rw-rw-rw-   0 root         (0) root         (0)    10319 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_memoize.py
+-rw-rw-rw-   0 root         (0) root         (0)    14428 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)      616 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     2072 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_mghimage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2715 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_naninfrange.py
+-rw-rw-rw-   0 root         (0) root         (0)     4979 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_notifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     4542 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_parse_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5853 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_platform.py
+-rw-rw-rw-   0 root         (0) root         (0)    12426 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/test_scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1909 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_atlasq_list_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5805 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_atlasq_ohi.py
+-rw-rw-rw-   0 root         (0) root         (0)    13942 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_atlasq_query.py
+-rw-rw-rw-   0 root         (0) root         (0)      892 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_fsl_abspath.py
+-rw-rw-rw-   0 root         (0) root         (0)     8569 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_fsl_apply_x5.py
+-rw-rw-rw-   0 root         (0) root         (0)     6569 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_fsl_convert_x5.py
+-rw-rw-rw-   0 root         (0) root         (0)     4619 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_fsl_ents.py
+-rw-rw-rw-   0 root         (0) root         (0)     5806 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_imglob.py
+-rw-rw-rw-   0 root         (0) root         (0)     3795 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_imln.py
+-rw-rw-rw-   0 root         (0) root         (0)    17332 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_immv_imcp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_imrm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2223 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_imtest.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_remove_ext.py
+-rw-rw-rw-   0 root         (0) root         (0)     5265 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_resample_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_scripts/test_vest2text.py
+-rw-rw-rw-   0 root         (0) root         (0)    14756 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_tempdir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/test_transform/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18588 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/test_affine.py
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/test_flirt.py
+-rw-rw-rw-   0 root         (0) root         (0)     4932 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/test_fnirt.py
+-rw-rw-rw-   0 root         (0) root         (0)    20930 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/test_nonlinear.py
+-rw-rw-rw-   0 root         (0) root         (0)     3555 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/test_x5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/test_transform/testdata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/test_transform/testdata/nonlinear/
+-rw-rw-rw-   0 root         (0) root         (0)     6321 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/nonlinear/coefficientfield.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)   238865 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/nonlinear/displacementfield.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)   248846 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/nonlinear/displacementfield_no_premat.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)    38498 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/nonlinear/ref.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)   286064 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/nonlinear/src.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      189 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/nonlinear/src2ref.mat
+-rw-rw-rw-   0 root         (0) root         (0)    58055 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_axisBounds.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3734 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_compose.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3028 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_concat.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_flirtMatrixToSform.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_invert.txt
+-rw-rw-rw-   0 root         (0) root         (0)      527 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_scaleoffsetxform.txt
+-rw-rw-rw-   0 root         (0) root         (0)   226337 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_00.txt
+-rw-rw-rw-   0 root         (0) root         (0)   226376 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_01.txt
+-rw-rw-rw-   0 root         (0) root         (0)   226406 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_02.txt
+-rw-rw-rw-   0 root         (0) root         (0)   226264 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_03.txt
+-rw-rw-rw-   0 root         (0) root         (0)   226215 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_04.txt
+-rw-rw-rw-   0 root         (0) root         (0)   225778 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_05.txt
+-rw-rw-rw-   0 root         (0) root         (0)   225869 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_06.txt
+-rw-rw-rw-   0 root         (0) root         (0)   225742 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_07.txt
+-rw-rw-rw-   0 root         (0) root         (0)   225386 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_08.txt
+-rw-rw-rw-   0 root         (0) root         (0)   227019 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_09.txt
+-rw-rw-rw-   0 root         (0) root         (0)   229117 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_10.txt
+-rw-rw-rw-   0 root         (0) root         (0)   226378 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_11.txt
+-rw-rw-rw-   0 root         (0) root         (0)   226339 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_12.txt
+-rw-rw-rw-   0 root         (0) root         (0)   230281 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_13.txt
+-rw-rw-rw-   0 root         (0) root         (0)   227417 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_14.txt
+-rw-rw-rw-   0 root         (0) root         (0)   226350 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_15.txt
+-rw-rw-rw-   0 root         (0) root         (0)   228249 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_16.txt
+-rw-rw-rw-   0 root         (0) root         (0)   228498 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_17.txt
+-rw-rw-rw-   0 root         (0) root         (0)   226585 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_18.txt
+-rw-rw-rw-   0 root         (0) root         (0)   228523 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_19.txt
+-rw-rw-rw-   0 root         (0) root         (0)   229073 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_20.txt
+-rw-rw-rw-   0 root         (0) root         (0)   234060 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_coords.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3593 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6954 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_vest.py
+-rw-rw-rw-   0 root         (0) root         (0)     9624 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_volumelabels.py
+-rw-rw-rw-   0 root         (0) root         (0)     2499 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_vtk.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_weakfuncref.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/test_wrappers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_wrappers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3161 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_wrappers/test_fslstats.py
+-rwxrwxrwx   0 root         (0) root         (0)    18503 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_wrappers/test_wrappers.py
+-rw-rw-rw-   0 root         (0) root         (0)    34453 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/test_wrappers/test_wrapperutils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/
+-rw-rw-rw-   0 root         (0) root         (0)      680 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/example.mgz
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/example.shape.gii
+-rw-rw-rw-   0 root         (0) root         (0)    16934 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/example.surf.gii
+-rw-rw-rw-   0 root         (0) root         (0)     6941 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/example4D.shape.gii
+-rw-rw-rw-   0 root         (0) root         (0)    13720 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/example4D_multiple_darrays.shape.gii
+-rw-rw-rw-   0 root         (0) root         (0)    26416 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/example_bad1.surf.gii
+-rw-rw-rw-   0 root         (0) root         (0)    24184 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/example_bad2.surf.gii
+-rw-rw-rw-   0 root         (0) root         (0)    14703 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/example_bad3.surf.gii
+-rw-rw-rw-   0 root         (0) root         (0)    18478 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/example_bad4.surf.gii
+-rw-rw-rw-   0 root         (0) root         (0)    14703 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/example_bad5.surf.gii
+-rw-rw-rw-   0 root         (0) root         (0)     7453 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/example_bad6.surf.gii
+-rw-rw-rw-   0 root         (0) root         (0)   386730 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/example_dicom.tbz2
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/absbrainthresh.txt
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/cluster_mask_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/cluster_mask_zstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      257 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/cluster_zstat1.txt
+-rw-rw-rw-   0 root         (0) root         (0)      269 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/cluster_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)      505 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/cluster_zstat2.txt
+-rw-rw-rw-   0 root         (0) root         (0)      581 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/cluster_zstat2_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3313 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/confoundevs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      415 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/design.con
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/design.frf
+-rw-rw-rw-   0 root         (0) root         (0)    10740 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/design.fsf
+-rw-rw-rw-   0 root         (0) root         (0)     6283 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/design.mat
+-rw-rw-rw-   0 root         (0) root         (0)        2 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/design.min
+-rw-rw-rw-   0 root         (0) root         (0)      186 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/design.trg
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      110 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/lmax_zstat1.txt
+-rw-rw-rw-   0 root         (0) root         (0)      166 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/lmax_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)      335 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/lmax_zstat2.txt
+-rw-rw-rw-   0 root         (0) root         (0)      491 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/lmax_zstat2_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mask.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0000
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0001
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0002
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0003
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0004
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0005
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0006
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0007
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0008
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0009
+-rw-rw-rw-   0 root         (0) root         (0)      150 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0010
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0011
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0012
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0013
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0014
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0015
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0016
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0017
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0018
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0019
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0020
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0021
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0022
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0023
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0024
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0025
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0026
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0027
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0028
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0029
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0030
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0031
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0032
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0033
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0034
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0035
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0036
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0037
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0038
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0039
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0040
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0041
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0042
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0043
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.mat/MAT_0044
+-rw-rw-rw-   0 root         (0) root         (0)     3313 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.par
+-rw-rw-rw-   0 root         (0) root         (0)      448 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf_abs.rms
+-rw-rw-rw-   0 root         (0) root         (0)        9 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf_abs_mean.rms
+-rw-rw-rw-   0 root         (0) root         (0)     3313 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf_final.par
+-rw-rw-rw-   0 root         (0) root         (0)      436 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf_rel.rms
+-rw-rw-rw-   0 root         (0) root         (0)       10 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf_rel_mean.rms
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mean_func.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      195 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/example_func2highres.mat
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/example_func2highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       87 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/example_func2initial_highres.mat
+-rw-rw-rw-   0 root         (0) root         (0)       42 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/example_func2initial_highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      190 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/example_func2standard.mat
+-rw-rw-rw-   0 root         (0) root         (0)       35 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/example_func2standard.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      193 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/highres2example_func.mat
+-rw-rw-rw-   0 root         (0) root         (0)      194 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/highres2initial_highres.mat
+-rw-rw-rw-   0 root         (0) root         (0)      185 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/highres2standard.mat
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/highres2standard.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       26 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/highres_head.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/initial_highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       88 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/initial_highres2example_func.mat
+-rw-rw-rw-   0 root         (0) root         (0)      195 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/initial_highres2highres.mat
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/initial_highres2highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       49 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/initial_highres2highres_fast_wmedge.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/initial_highres2highres_fast_wmseg.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      181 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/initial_highres2highres_init.mat
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/standard.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      191 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/standard2example_func.mat
+-rw-rw-rw-   0 root         (0) root         (0)      189 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg/standard2highres.mat
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       27 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/mask.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/mean_func.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/reg/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/reg/highres.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/stats/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/stats/cope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/stats/cope2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/stats/varcope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/reg_standard/stats/varcope2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/rendered_thresh_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/rendered_thresh_zstat2.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/cope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/cope2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        5 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/dof
+-rw-rw-rw-   0 root         (0) root         (0)      189 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/logfile
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/pe1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/pe10.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/pe2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/pe3.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/pe4.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/pe5.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/pe6.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/pe7.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/pe8.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/pe9.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/res4d.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/sigmasquareds.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/smoothness
+-rw-rw-rw-   0 root         (0) root         (0)       25 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/threshac1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/tstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/tstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       24 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/varcope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       24 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/varcope2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/stats/zstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       23 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/thresh_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        5 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/thresh_zstat1.vol
+-rw-rw-rw-   0 root         (0) root         (0)       23 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/thresh_zstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        5 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/thresh_zstat2.vol
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/absbrainthresh.txt
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/cluster_mask_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/cluster_mask_zstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      319 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/cluster_zstat1.txt
+-rw-rw-rw-   0 root         (0) root         (0)      344 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/cluster_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)      313 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/cluster_zstat2.txt
+-rw-rw-rw-   0 root         (0) root         (0)      338 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/cluster_zstat2_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3299 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/confoundevs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      441 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/design.con
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/design.frf
+-rw-rw-rw-   0 root         (0) root         (0)    11227 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/design.fsf
+-rw-rw-rw-   0 root         (0) root         (0)     6904 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/design.mat
+-rw-rw-rw-   0 root         (0) root         (0)        2 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/design.min
+-rw-rw-rw-   0 root         (0) root         (0)      188 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/design.trg
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/designInputVoxelwiseEV3.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/designVoxelwiseEV3.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      186 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/lmax_zstat1.txt
+-rw-rw-rw-   0 root         (0) root         (0)      279 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/lmax_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)      186 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/lmax_zstat2.txt
+-rw-rw-rw-   0 root         (0) root         (0)      269 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/lmax_zstat2_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mask.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0000
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0001
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0002
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0003
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0004
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0005
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0006
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0007
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0008
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0009
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0010
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0011
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0012
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0013
+-rw-rw-rw-   0 root         (0) root         (0)      150 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0014
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0015
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0016
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0017
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0018
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0019
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0020
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0021
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0022
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0023
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0024
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0025
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0026
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0027
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0028
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0029
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0030
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0031
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0032
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0033
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0034
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0035
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0036
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0037
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0038
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0039
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0040
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0041
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0042
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0043
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.mat/MAT_0044
+-rw-rw-rw-   0 root         (0) root         (0)     3299 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.par
+-rw-rw-rw-   0 root         (0) root         (0)      442 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf_abs.rms
+-rw-rw-rw-   0 root         (0) root         (0)       10 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf_abs_mean.rms
+-rw-rw-rw-   0 root         (0) root         (0)     3299 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf_final.par
+-rw-rw-rw-   0 root         (0) root         (0)      434 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf_rel.rms
+-rw-rw-rw-   0 root         (0) root         (0)       10 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf_rel_mean.rms
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mean_func.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      195 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/example_func2highres.mat
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/example_func2highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       87 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/example_func2initial_highres.mat
+-rw-rw-rw-   0 root         (0) root         (0)       42 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/example_func2initial_highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      188 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/example_func2standard.mat
+-rw-rw-rw-   0 root         (0) root         (0)       35 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/example_func2standard.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      194 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/highres2example_func.mat
+-rw-rw-rw-   0 root         (0) root         (0)      194 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/highres2initial_highres.mat
+-rw-rw-rw-   0 root         (0) root         (0)      185 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/highres2standard.mat
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/highres2standard.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       26 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/highres_head.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/initial_highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       88 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/initial_highres2example_func.mat
+-rw-rw-rw-   0 root         (0) root         (0)      195 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/initial_highres2highres.mat
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/initial_highres2highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       49 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/initial_highres2highres_fast_wmedge.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/initial_highres2highres_fast_wmseg.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      181 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/initial_highres2highres_init.mat
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/standard.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      191 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/standard2example_func.mat
+-rw-rw-rw-   0 root         (0) root         (0)      189 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/reg/standard2highres.mat
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/rendered_thresh_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/rendered_thresh_zstat2.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/cope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/cope2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        5 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/dof
+-rw-rw-rw-   0 root         (0) root         (0)      222 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/logfile
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/pe1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/pe10.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/pe11.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/pe2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/pe3.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/pe4.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/pe5.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/pe6.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/pe7.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/pe8.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/pe9.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/res4d.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/sigmasquareds.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       39 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/smoothness
+-rw-rw-rw-   0 root         (0) root         (0)       25 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/threshac1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/tstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/tstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       24 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/varcope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       24 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/varcope2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/stats/zstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       23 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/thresh_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        5 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/thresh_zstat1.vol
+-rw-rw-rw-   0 root         (0) root         (0)       23 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/thresh_zstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        5 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/thresh_zstat2.vol
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/InputconfoundEV1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        7 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/absbrainthresh.txt
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/cluster_mask_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/cluster_mask_zstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      369 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/cluster_zstat1.txt
+-rw-rw-rw-   0 root         (0) root         (0)      507 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/cluster_zstat2.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/confoundEV1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)    18118 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/confoundevs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      987 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/design.con
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/design.frf
+-rw-rw-rw-   0 root         (0) root         (0)    10095 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/design.fsf
+-rw-rw-rw-   0 root         (0) root         (0)    20020 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/design.mat
+-rw-rw-rw-   0 root         (0) root         (0)        2 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/design.min
+-rw-rw-rw-   0 root         (0) root         (0)      265 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/design.trg
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      108 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/lmax_zstat1.txt
+-rw-rw-rw-   0 root         (0) root         (0)      304 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/lmax_zstat2.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mask.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0000
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0001
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0002
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0003
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0004
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0005
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0006
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0007
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0008
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0009
+-rw-rw-rw-   0 root         (0) root         (0)      150 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0010
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0011
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0012
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0013
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0014
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0015
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0016
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0017
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0018
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0019
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0020
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0021
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0022
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0023
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0024
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0025
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0026
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0027
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0028
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0029
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0030
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0031
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0032
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0033
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0034
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0035
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0036
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0037
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0038
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0039
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0040
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0041
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0042
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0043
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.mat/MAT_0044
+-rw-rw-rw-   0 root         (0) root         (0)     3313 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.par
+-rw-rw-rw-   0 root         (0) root         (0)      448 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_abs.rms
+-rw-rw-rw-   0 root         (0) root         (0)        9 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_abs_mean.rms
+-rw-rw-rw-   0 root         (0) root         (0)    13185 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_diff.dat
+-rw-rw-rw-   0 root         (0) root         (0)    16498 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_final.par
+-rw-rw-rw-   0 root         (0) root         (0)      436 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_rel.rms
+-rw-rw-rw-   0 root         (0) root         (0)       10 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_rel_mean.rms
+-rw-rw-rw-   0 root         (0) root         (0)      450 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/meanConfounds.dat
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mean_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/rendered_thresh_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/rendered_thresh_zstat2.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/cope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/cope2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        5 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/dof
+-rw-rw-rw-   0 root         (0) root         (0)      215 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/logfile
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe10.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe11.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe12.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe13.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe14.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe15.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe16.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe17.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe18.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe19.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe20.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe21.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe22.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe23.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe24.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe25.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe26.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe27.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe28.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe29.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe3.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe30.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe31.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe32.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe4.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe5.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe6.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe7.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe8.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/pe9.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/res4d.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/sigmasquareds.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       39 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/smoothness
+-rw-rw-rw-   0 root         (0) root         (0)       25 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/threshac1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/tstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/tstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       24 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/varcope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       24 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/varcope2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/stats/zstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       23 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/thresh_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        5 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/thresh_zstat1.vol
+-rw-rw-rw-   0 root         (0) root         (0)       23 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/thresh_zstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        5 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/thresh_zstat2.vol
+-rw-rw-rw-   0 root         (0) root         (0)       11 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/vef.dat
+-rw-rw-rw-   0 root         (0) root         (0)        1 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/ven.dat
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/absbrainthresh.txt
+-rw-rw-rw-   0 root         (0) root         (0)      258 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/design.con
+-rw-rw-rw-   0 root         (0) root         (0)        8 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/design.frf
+-rw-rw-rw-   0 root         (0) root         (0)     9916 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/design.fsf
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/design.mat
+-rw-rw-rw-   0 root         (0) root         (0)        2 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/design.min
+-rw-rw-rw-   0 root         (0) root         (0)      174 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/design.trg
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       14 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mask.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0000
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0001
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0002
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0003
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0004
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0005
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0006
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0007
+-rw-rw-rw-   0 root         (0) root         (0)      151 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0008
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0009
+-rw-rw-rw-   0 root         (0) root         (0)      150 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0010
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0011
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0012
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0013
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0014
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0015
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0016
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0017
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0018
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0019
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0020
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0021
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0022
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0023
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0024
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0025
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0026
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0027
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0028
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0029
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0030
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0031
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0032
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0033
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0034
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0035
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0036
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0037
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0038
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0039
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0040
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0041
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0042
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0043
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.mat/MAT_0044
+-rw-rw-rw-   0 root         (0) root         (0)     3313 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.par
+-rw-rw-rw-   0 root         (0) root         (0)      448 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf_abs.rms
+-rw-rw-rw-   0 root         (0) root         (0)        9 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf_abs_mean.rms
+-rw-rw-rw-   0 root         (0) root         (0)      436 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf_rel.rms
+-rw-rw-rw-   0 root         (0) root         (0)       10 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf_rel_mean.rms
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mean_func.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      195 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/example_func2highres.mat
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/example_func2highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       87 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/example_func2initial_highres.mat
+-rw-rw-rw-   0 root         (0) root         (0)       42 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/example_func2initial_highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      190 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/example_func2standard.mat
+-rw-rw-rw-   0 root         (0) root         (0)       35 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/example_func2standard.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      193 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/highres2example_func.mat
+-rw-rw-rw-   0 root         (0) root         (0)      194 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/highres2initial_highres.mat
+-rw-rw-rw-   0 root         (0) root         (0)      185 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/highres2standard.mat
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/highres2standard.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       26 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/highres_head.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/initial_highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       88 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/initial_highres2example_func.mat
+-rw-rw-rw-   0 root         (0) root         (0)      195 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/initial_highres2highres.mat
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/initial_highres2highres.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       49 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/initial_highres2highres_fast_wmedge.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/initial_highres2highres_fast_wmseg.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      181 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/initial_highres2highres_init.mat
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/standard.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      191 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/standard2example_func.mat
+-rw-rw-rw-   0 root         (0) root         (0)      189 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/reg/standard2highres.mat
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/absbrainthresh.txt
+-rw-rw-rw-   0 root         (0) root         (0)      122 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/cluster_mask_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      122 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/cluster_mask_zstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      252 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/cluster_zstat1.txt
+-rw-rw-rw-   0 root         (0) root         (0)      247 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/cluster_zstat2.txt
+-rw-rw-rw-   0 root         (0) root         (0)      258 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/design.con
+-rw-rw-rw-   0 root         (0) root         (0)        8 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/design.frf
+-rw-rw-rw-   0 root         (0) root         (0)     9670 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/design.fsf
+-rw-rw-rw-   0 root         (0) root         (0)     2574 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/design.mat
+-rw-rw-rw-   0 root         (0) root         (0)        2 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/design.min
+-rw-rw-rw-   0 root         (0) root         (0)      174 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/design.trg
+-rw-rw-rw-   0 root         (0) root         (0)      391 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)    12354 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       62 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/lmax_zstat1.txt
+-rw-rw-rw-   0 root         (0) root         (0)       49 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/lmax_zstat2.txt
+-rw-rw-rw-   0 root         (0) root         (0)      112 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/mask.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      435 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/mean_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      451 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/rendered_thresh_zstat1.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/
+-rw-rw-rw-   0 root         (0) root         (0)      448 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/cope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      451 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/cope2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        5 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/dof
+-rw-rw-rw-   0 root         (0) root         (0)      189 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/logfile
+-rw-rw-rw-   0 root         (0) root         (0)      448 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/pe1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      450 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/pe2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      451 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/pe3.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      452 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/pe4.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)    13580 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/res4d.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      442 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/sigmasquareds.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/smoothness
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/threshac1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      448 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/tstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      447 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/tstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      444 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/varcope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      444 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/varcope2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      446 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/zstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      179 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/thresh_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        3 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/thresh_zstat1.vol
+-rw-rw-rw-   0 root         (0) root         (0)      170 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/thresh_zstat2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        3 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/thresh_zstat2.vol
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/bg_image.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/
+-rwxrwxrwx   0 root         (0) root         (0)      187 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/.flame
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/cluster_mask_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      663 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/cluster_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)      129 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/design.con
+-rw-rw-rw-   0 root         (0) root         (0)     7861 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/design.fsf
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/design.grp
+-rw-rw-rw-   0 root         (0) root         (0)       14 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/design.lcon
+-rw-rw-rw-   0 root         (0) root         (0)        9 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/design.lev
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/design.mat
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       39 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      707 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/lmax_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)       25 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/mask.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/mean_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       43 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/rendered_thresh_zstat1.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/cope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        2 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/dof
+-rw-rw-rw-   0 root         (0) root         (0)      233 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/logfile
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/mean_random_effects_var1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/pe1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/res4d.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       41 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/smoothness
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/tdof_t1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/tstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       35 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/varcope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       35 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/weights1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       45 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/zflame1lowertstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       45 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/zflame1uppertstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/stats/zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/thresh_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        6 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/thresh_zstat1.vol
+-rw-rw-rw-   0 root         (0) root         (0)       43 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/var_filtered_func_data.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/
+-rwxrwxrwx   0 root         (0) root         (0)      187 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/.flame
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/cluster_mask_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      251 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/cluster_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)      129 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/design.con
+-rw-rw-rw-   0 root         (0) root         (0)     7861 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/design.fsf
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/design.grp
+-rw-rw-rw-   0 root         (0) root         (0)       14 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/design.lcon
+-rw-rw-rw-   0 root         (0) root         (0)        7 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/design.lev
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/design.mat
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       39 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      124 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/lmax_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)       25 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/mask.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/mean_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       43 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/rendered_thresh_zstat1.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/cope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        2 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/dof
+-rw-rw-rw-   0 root         (0) root         (0)      233 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/logfile
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/mean_random_effects_var1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/pe1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/res4d.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/smoothness
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/tdof_t1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/tstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       35 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/varcope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       35 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/weights1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       45 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/zflame1lowertstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       45 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/zflame1uppertstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/stats/zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/thresh_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        6 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/thresh_zstat1.vol
+-rw-rw-rw-   0 root         (0) root         (0)       43 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/var_filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      129 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/design.con
+-rw-rw-rw-   0 root         (0) root         (0)     7861 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/design.fsf
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/design.grp
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/design.lcon
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/design.mat
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/inputreg/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/inputreg/masksum.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/inputreg/masksum_overlay.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/inputreg/maskunique.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/inputreg/maskunique_overlay.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       14 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/mask.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/mean_func.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/bg_image.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/
+-rwxrwxrwx   0 root         (0) root         (0)      327 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/.flame
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/cluster_mask_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      831 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/cluster_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)      145 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/design.con
+-rw-rw-rw-   0 root         (0) root         (0)     8071 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/design.fsf
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/design.grp
+-rw-rw-rw-   0 root         (0) root         (0)       14 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/design.lcon
+-rw-rw-rw-   0 root         (0) root         (0)        9 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/design.lev
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/design.mat
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       39 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      766 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/lmax_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)       25 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/mask.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/mean_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       43 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/rendered_thresh_zstat1.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/cope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        2 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/dof
+-rw-rw-rw-   0 root         (0) root         (0)      373 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/logfile
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/mean_random_effects_var1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/pe1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/pe2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/res4d.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/smoothness
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/tdof_t1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/tstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       35 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/varcope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       35 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/weights1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       45 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/zflame1lowertstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       45 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/zflame1uppertstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/stats/zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/thresh_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        6 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/thresh_zstat1.vol
+-rw-rw-rw-   0 root         (0) root         (0)       43 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/var_filtered_func_data.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/
+-rwxrwxrwx   0 root         (0) root         (0)      327 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/.flame
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/cluster_mask_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/cluster_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)      145 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/design.con
+-rw-rw-rw-   0 root         (0) root         (0)     8071 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/design.fsf
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/design.grp
+-rw-rw-rw-   0 root         (0) root         (0)       14 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/design.lcon
+-rw-rw-rw-   0 root         (0) root         (0)        7 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/design.lev
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/design.mat
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       39 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2340 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/lmax_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)       25 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/mask.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/mean_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       43 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/rendered_thresh_zstat1.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/cope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        2 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/dof
+-rw-rw-rw-   0 root         (0) root         (0)      373 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/logfile
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/mean_random_effects_var1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/pe1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/pe2.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/res4d.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/smoothness
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/tdof_t1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/tstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       35 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/varcope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       35 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/weights1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       45 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/zflame1lowertstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       45 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/zflame1uppertstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/stats/zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/thresh_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        6 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/thresh_zstat1.vol
+-rw-rw-rw-   0 root         (0) root         (0)       43 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/var_filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      145 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/design.con
+-rw-rw-rw-   0 root         (0) root         (0)     8071 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/design.fsf
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/design.grp
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/design.lcon
+-rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/design.mat
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/inputreg/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/inputreg/masksum.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/inputreg/masksum_overlay.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/inputreg/maskunique.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/inputreg/maskunique_overlay.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       14 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/mask.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/mean_func.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/bg_image.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/
+-rwxrwxrwx   0 root         (0) root         (0)      215 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/.flame
+-rw-rw-rw-   0 root         (0) root         (0)      253 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/cluster_mask_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      522 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/cluster_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)      129 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/design.con
+-rw-rw-rw-   0 root         (0) root         (0)     7891 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/design.fsf
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/design.grp
+-rw-rw-rw-   0 root         (0) root         (0)        9 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/design.lcon
+-rw-rw-rw-   0 root         (0) root         (0)        7 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/design.lev
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/design.mat
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)    11136 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      527 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/lmax_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/mask.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     3644 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/mean_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     3726 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/rendered_thresh_zstat1.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/
+-rw-rw-rw-   0 root         (0) root         (0)     3839 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/cope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        2 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/dof
+-rw-rw-rw-   0 root         (0) root         (0)      262 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/logfile
+-rw-rw-rw-   0 root         (0) root         (0)      138 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/mean_random_effects_var1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     3839 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/pe1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)    10615 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/res4d.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       41 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/smoothness
+-rw-rw-rw-   0 root         (0) root         (0)      142 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/tdof_t1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     3839 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/tstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     3748 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/varcope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      160 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/weights1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      138 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/zflame1lowertstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      138 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/zflame1uppertstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     3832 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      159 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/tdof_filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/thresh_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        6 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/thresh_zstat1.vol
+-rw-rw-rw-   0 root         (0) root         (0)    10862 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/var_filtered_func_data.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/
+-rwxrwxrwx   0 root         (0) root         (0)      215 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/.flame
+-rw-rw-rw-   0 root         (0) root         (0)      138 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/cluster_mask_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      457 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/cluster_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)      129 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/design.con
+-rw-rw-rw-   0 root         (0) root         (0)     7891 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/design.fsf
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/design.grp
+-rw-rw-rw-   0 root         (0) root         (0)        8 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/design.lcon
+-rw-rw-rw-   0 root         (0) root         (0)        9 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/design.lev
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/design.mat
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/example_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)    11247 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      335 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/lmax_zstat1_std.txt
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/mask.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     3644 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/mean_func.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     3760 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/rendered_thresh_zstat1.nii.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 22:44:23.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/
+-rw-rw-rw-   0 root         (0) root         (0)     3890 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/cope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        2 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/dof
+-rw-rw-rw-   0 root         (0) root         (0)      262 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/logfile
+-rw-rw-rw-   0 root         (0) root         (0)      138 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/mean_random_effects_var1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     3890 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/pe1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)    10802 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/res4d.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)       41 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/smoothness
+-rw-rw-rw-   0 root         (0) root         (0)      142 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/tdof_t1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     3889 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/tstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     3755 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/varcope1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      160 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/weights1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      138 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/zflame1lowertstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      138 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/zflame1uppertstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     3893 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      159 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/tdof_filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      301 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/thresh_zstat1.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)        6 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/thresh_zstat1.vol
+-rw-rw-rw-   0 root         (0) root         (0)    10871 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/var_filtered_func_data.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)      129 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/design.con
+-rw-rw-rw-   0 root         (0) root         (0)     7891 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/design.fsf
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/design.grp
+-rw-rw-rw-   0 root         (0) root         (0)       17 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/design.lcon
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/design.mat
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/mask.nii.gz
+-rw-rw-rw-   0 root         (0) root         (0)     3644 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/mean_func.nii.gz
+-rwxrwxrwx   0 root         (0) root         (0)    32615 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_mesh.vtk
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2022-06-02 20:10:03.000000 fslpy-3.9.5/tests/testdata/test_mesh_data.txt
```

### Comparing `fslpy-3.9.4/CHANGELOG.rst` & `fslpy-3.9.5/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,43 @@
 This document contains the ``fslpy`` release history in reverse chronological
 order.
 
 
+3.9.5 (Thursday 2nd June 2022)
+------------------------------
+
+
+Changed
+^^^^^^^
+
+
+* Updated the :func:`.ensureIsImage` function to support ``pathlib.Path``
+  objects (!343).
+
+
+Fixed
+^^^^^
+
+
+* Some fixes in the :mod:`.wrappers` module (specifically in the
+  :class:`.FileOrThing` class) to better support ``pathlib.Path`` objects
+  (!343).
+
+
 3.9.4 (Friday 27th May 2022)
 ----------------------------
 
 
 Changed
 ^^^^^^^
 
 
 * Changed the behaviour of :meth:`.Image.__getitem__` so that, if image
   data is accessed with a boolean mask array (e.g. ``image[mask > 0]``),
   the image data is loaded into memory (!341).
-* Fixed an issue in the :func:`.func_to_cmd` function (!339).
 
 
 3.9.3 (Friday 27th May 2022)
 ----------------------------
 
 
 Fixed
```

### Comparing `fslpy-3.9.4/LICENSE` & `fslpy-3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/PKG-INFO` & `fslpy-3.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fslpy
-Version: 3.9.4
+Version: 3.9.5
 Summary: FSL Python library
 Home-page: https://git.fmrib.ox.ac.uk/fsl/fslpy
 Author: Paul McCarthy
 Author-email: pauldmccarthy@gmail.com
 License: Apache License Version 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fslpy-3.9.4/README.rst` & `fslpy-3.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/doc/conf.py` & `fslpy-3.9.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/doc/contributing.rst` & `fslpy-3.9.5/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/doc/fsl.data.rst` & `fslpy-3.9.5/doc/fsl.data.rst`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/doc/fsl.scripts.rst` & `fslpy-3.9.5/doc/fsl.scripts.rst`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/doc/fsl.utils.rst` & `fslpy-3.9.5/doc/fsl.utils.rst`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/doc/images/fnirt_coefficient_field.png` & `fslpy-3.9.5/doc/images/fnirt_coefficient_field.png`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/doc/images/fnirt_coefficient_field.xcf` & `fslpy-3.9.5/doc/images/fnirt_coefficient_field.xcf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/doc/images/fnirt_warp_field.png` & `fslpy-3.9.5/doc/images/fnirt_warp_field.png`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/doc/images/fnirt_warp_field.xcf` & `fslpy-3.9.5/doc/images/fnirt_warp_field.xcf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/doc/images/nonlinear_registration_process.png` & `fslpy-3.9.5/doc/images/nonlinear_registration_process.png`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/doc/images/nonlinear_registration_process.xcf` & `fslpy-3.9.5/doc/images/nonlinear_registration_process.xcf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/doc/index.rst` & `fslpy-3.9.5/doc/index.rst`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/atlases.py` & `fslpy-3.9.5/fsl/data/atlases.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/bitmap.py` & `fslpy-3.9.5/fsl/data/bitmap.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/cifti.py` & `fslpy-3.9.5/fsl/data/cifti.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/constants.py` & `fslpy-3.9.5/fsl/data/constants.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/dicom.py` & `fslpy-3.9.5/fsl/data/dicom.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/dtifit.py` & `fslpy-3.9.5/fsl/data/dtifit.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/featanalysis.py` & `fslpy-3.9.5/fsl/data/featanalysis.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/featdesign.py` & `fslpy-3.9.5/fsl/data/featdesign.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/featimage.py` & `fslpy-3.9.5/fsl/data/featimage.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/fixlabels.py` & `fslpy-3.9.5/fsl/data/fixlabels.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/freesurfer.py` & `fslpy-3.9.5/fsl/data/freesurfer.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/gifti.py` & `fslpy-3.9.5/fsl/data/gifti.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/image.py` & `fslpy-3.9.5/fsl/data/image.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/imagewrapper.py` & `fslpy-3.9.5/fsl/data/imagewrapper.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/melodicanalysis.py` & `fslpy-3.9.5/fsl/data/melodicanalysis.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/melodicimage.py` & `fslpy-3.9.5/fsl/data/melodicimage.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/mesh.py` & `fslpy-3.9.5/fsl/data/mesh.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/mghimage.py` & `fslpy-3.9.5/fsl/data/mghimage.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/utils.py` & `fslpy-3.9.5/fsl/data/utils.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/vest.py` & `fslpy-3.9.5/fsl/data/vest.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/volumelabels.py` & `fslpy-3.9.5/fsl/data/volumelabels.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/data/vtk.py` & `fslpy-3.9.5/fsl/data/vtk.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/Text2Vest.py` & `fslpy-3.9.5/fsl/scripts/Text2Vest.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/Vest2Text.py` & `fslpy-3.9.5/fsl/scripts/Vest2Text.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/atlasq.py` & `fslpy-3.9.5/fsl/scripts/atlasq.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/fsl_abspath.py` & `fslpy-3.9.5/fsl/scripts/fsl_abspath.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/fsl_apply_x5.py` & `fslpy-3.9.5/fsl/scripts/fsl_apply_x5.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/fsl_convert_x5.py` & `fslpy-3.9.5/fsl/scripts/fsl_convert_x5.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/fsl_ents.py` & `fslpy-3.9.5/fsl/scripts/fsl_ents.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/imcp.py` & `fslpy-3.9.5/fsl/scripts/imcp.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/imglob.py` & `fslpy-3.9.5/fsl/scripts/imglob.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/imln.py` & `fslpy-3.9.5/fsl/scripts/imln.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/immv.py` & `fslpy-3.9.5/fsl/scripts/immv.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/imrm.py` & `fslpy-3.9.5/fsl/scripts/imrm.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/imtest.py` & `fslpy-3.9.5/fsl/scripts/imtest.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/remove_ext.py` & `fslpy-3.9.5/fsl/scripts/remove_ext.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/scripts/resample_image.py` & `fslpy-3.9.5/fsl/scripts/resample_image.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/transform/affine.py` & `fslpy-3.9.5/fsl/transform/affine.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/transform/flirt.py` & `fslpy-3.9.5/fsl/transform/flirt.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/transform/fnirt.py` & `fslpy-3.9.5/fsl/transform/fnirt.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/transform/nonlinear.py` & `fslpy-3.9.5/fsl/transform/nonlinear.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/transform/x5.py` & `fslpy-3.9.5/fsl/transform/x5.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/assertions.py` & `fslpy-3.9.5/fsl/utils/assertions.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/bids.py` & `fslpy-3.9.5/fsl/utils/bids.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/cache.py` & `fslpy-3.9.5/fsl/utils/cache.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/deprecated.py` & `fslpy-3.9.5/fsl/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/ensure.py` & `fslpy-3.9.5/fsl/utils/ensure.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 
 .. autosummary::
    :nosignatures:
 
    ensureIsImage
 """
 
+import pathlib
 
 import nibabel as nib
 
 import fsl.data.image as fslimage
 
 
 def ensureIsImage(img):
     """Ensures that the given ``img`` is an in-memory ``nibabel`` object.
     """
-    if isinstance(img, str):
+    if isinstance(img, (str, pathlib.Path)):
         img = fslimage.addExt(img)
         img = nib.load(img)
     return img
```

### Comparing `fslpy-3.9.4/fsl/utils/filetree/__init__.py` & `fslpy-3.9.5/fsl/utils/filetree/__init__.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/filetree/filetree.py` & `fslpy-3.9.5/fsl/utils/filetree/filetree.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/filetree/parse.py` & `fslpy-3.9.5/fsl/utils/filetree/parse.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/filetree/query.py` & `fslpy-3.9.5/fsl/utils/filetree/query.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/filetree/trees/BedpostX.tree` & `fslpy-3.9.5/fsl/utils/filetree/trees/BedpostX.tree`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/filetree/trees/HCP_Surface.tree` & `fslpy-3.9.5/fsl/utils/filetree/trees/HCP_Surface.tree`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/filetree/trees/HCP_directory.tree` & `fslpy-3.9.5/fsl/utils/filetree/trees/HCP_directory.tree`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/filetree/trees/ProbtrackX.tree` & `fslpy-3.9.5/fsl/utils/filetree/trees/ProbtrackX.tree`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/filetree/trees/bids_raw.tree` & `fslpy-3.9.5/fsl/utils/filetree/trees/bids_raw.tree`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/filetree/trees/eddy.tree` & `fslpy-3.9.5/fsl/utils/filetree/trees/eddy.tree`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/filetree/trees/freesurfer.tree` & `fslpy-3.9.5/fsl/utils/filetree/trees/freesurfer.tree`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/filetree/trees/fsl_anat.tree` & `fslpy-3.9.5/fsl/utils/filetree/trees/fsl_anat.tree`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/filetree/trees/tbss.tree` & `fslpy-3.9.5/fsl/utils/filetree/trees/tbss.tree`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/filetree/utils.py` & `fslpy-3.9.5/fsl/utils/filetree/utils.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/fslsub.py` & `fslpy-3.9.5/fsl/utils/fslsub.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/idle.py` & `fslpy-3.9.5/fsl/utils/idle.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/image/resample.py` & `fslpy-3.9.5/fsl/utils/image/resample.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/image/roi.py` & `fslpy-3.9.5/fsl/utils/image/roi.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/imcp.py` & `fslpy-3.9.5/fsl/utils/imcp.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/memoize.py` & `fslpy-3.9.5/fsl/utils/memoize.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/meta.py` & `fslpy-3.9.5/fsl/utils/meta.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/naninfrange.py` & `fslpy-3.9.5/fsl/utils/naninfrange.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/notifier.py` & `fslpy-3.9.5/fsl/utils/notifier.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/parse_data.py` & `fslpy-3.9.5/fsl/utils/parse_data.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/path.py` & `fslpy-3.9.5/fsl/utils/path.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/platform.py` & `fslpy-3.9.5/fsl/utils/platform.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/run.py` & `fslpy-3.9.5/fsl/utils/run.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/settings.py` & `fslpy-3.9.5/fsl/utils/settings.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/tempdir.py` & `fslpy-3.9.5/fsl/utils/tempdir.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/utils/weakfuncref.py` & `fslpy-3.9.5/fsl/utils/weakfuncref.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/version.py` & `fslpy-3.9.5/fsl/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 import os.path as op
 import            re
 import            string
 
 
-__version__ = '3.9.4'
+__version__ = '3.9.5'
 """Current version number, as a string. """
 
 
 def parseVersionString(versionString):
     """Parses the given version string, and returns a tuple containing
     the individual components of the version number (see the description
     of the :attr:`__version__` attribute).
```

### Comparing `fslpy-3.9.4/fsl/wrappers/__init__.py` & `fslpy-3.9.5/fsl/wrappers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -72,14 +72,29 @@
     from fsl.wrappers import fslmaths
 
     image  = nib.load('image.nii')
     mask   = nib.load('mask.nii')
     output = fslmaths(image).mas(mask).bin().run()
 
 
+It is possible to run a Python script in Windows, and call FSL commands which
+are installed in a WSL environment. When specifying inputs/outputs as
+file/directory paths, the safest option is to use ``pathlib.Path`` objects
+to ensure that they are correctly translated bewteen Windows and Linux-style
+paths, e.g.::
+
+    from pathlib import Path
+    from fsl.wrappers import bet
+
+    bet(Path('T1\\T1.nii.gz`), Path('T1_brain'))
+
+If you use strings to specify inputs/outputs, they must be absolute paths, as
+they may otherwise not be translated correctly.
+
+
 If you are *writing* wrapper functions, take a look at the
 :mod:`.wrapperutils` module - it contains several useful functions and
 decorators.
 """
 
 
 from fsl.wrappers.wrapperutils import (LOAD,)
```

### Comparing `fslpy-3.9.4/fsl/wrappers/bet.py` & `fslpy-3.9.5/fsl/wrappers/bet.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/wrappers/eddy.py` & `fslpy-3.9.5/fsl/wrappers/eddy.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/wrappers/epi_reg.py` & `fslpy-3.9.5/fsl/wrappers/epi_reg.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/wrappers/fast.py` & `fslpy-3.9.5/fsl/wrappers/fast.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/wrappers/flirt.py` & `fslpy-3.9.5/fsl/wrappers/flirt.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/wrappers/fnirt.py` & `fslpy-3.9.5/fsl/wrappers/fnirt.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/wrappers/fsl_anat.py` & `fslpy-3.9.5/fsl/wrappers/fsl_anat.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/wrappers/fsl_sub.py` & `fslpy-3.9.5/fsl/wrappers/fsl_sub.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/wrappers/fslmaths.py` & `fslpy-3.9.5/fsl/wrappers/fslmaths.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/wrappers/fslstats.py` & `fslpy-3.9.5/fsl/wrappers/fslstats.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/wrappers/fugue.py` & `fslpy-3.9.5/fsl/wrappers/fugue.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/wrappers/melodic.py` & `fslpy-3.9.5/fsl/wrappers/melodic.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/wrappers/misc.py` & `fslpy-3.9.5/fsl/wrappers/misc.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/wrappers/tbss.py` & `fslpy-3.9.5/fsl/wrappers/tbss.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fsl/wrappers/wrapperutils.py` & `fslpy-3.9.5/fsl/wrappers/wrapperutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -705,14 +705,15 @@
           - A directory in which all temporary input/output files should be
             stored
 
           - The name of the keyword argument to be processed
 
           - The argument value that was passed in
         """
+
         self.__func      = func
         self.__prepIn    = prepIn
         self.__prepOut   = prepOut
         self.__load      = load
         self.__removeExt = removeExt
         self.__things    = args
         self.__outprefix = kwargs.get('outprefix', None)
@@ -869,14 +870,16 @@
         #
         # Importantly, here we assume that the
         # underlying function (and hence the
         # underlying command-line tool) will
         # accept an output prefix which contains
         # a directory path.
         if prefix is not None:
+            if isinstance(prefix, pathlib.Path):
+                prefix = op.abspath(prefix)
 
             # If prefix is set to LOAD,
             # all generated output files
             # should be loaded - we use a
             # randomly generated prefix,
             # and add it to prefixedFiles,
             # so that every file which
@@ -961,14 +964,23 @@
 
                 if infile is not None:
                     allargs[name] = infile
 
         if realPrefix is not None and len(prefixedFiles) == 0:
             allargs[self.__outprefix] = realPrefix
 
+        # Turn any Path objects into absolute path
+        # strings. Don't use Path.resolve(), as it
+        # returns a relative path for non-existent
+        # files/dirs on Windows/certain Python
+        # versions.
+        for k, v in allargs.items():
+            if isinstance(v, pathlib.Path):
+                allargs[k] = op.abspath(v)
+
         args   = [allargs.pop(k) for k in argnames]
         kwargs = allargs
 
         return args, kwargs, realPrefix, outfiles, prefixedFiles
 
 
     def __generateResult(
```

### Comparing `fslpy-3.9.4/fslpy.egg-info/PKG-INFO` & `fslpy-3.9.5/fslpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fslpy
-Version: 3.9.4
+Version: 3.9.5
 Summary: FSL Python library
 Home-page: https://git.fmrib.ox.ac.uk/fsl/fslpy
 Author: Paul McCarthy
 Author-email: pauldmccarthy@gmail.com
 License: Apache License Version 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fslpy-3.9.4/fslpy.egg-info/SOURCES.txt` & `fslpy-3.9.5/fslpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/fslpy.egg-info/entry_points.txt` & `fslpy-3.9.5/fslpy.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/setup.cfg` & `fslpy-3.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/setup.py` & `fslpy-3.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/__init__.py` & `fslpy-3.9.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/conftest.py` & `fslpy-3.9.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_assertions.py` & `fslpy-3.9.5/tests/test_assertions.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_atlases.py` & `fslpy-3.9.5/tests/test_atlases.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_atlases_query.py` & `fslpy-3.9.5/tests/test_atlases_query.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_bids.py` & `fslpy-3.9.5/tests/test_bids.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_bitmap.py` & `fslpy-3.9.5/tests/test_bitmap.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_cache.py` & `fslpy-3.9.5/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_cifti.py` & `fslpy-3.9.5/tests/test_cifti.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_deprecated.py` & `fslpy-3.9.5/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_dicom.py` & `fslpy-3.9.5/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_dtifit.py` & `fslpy-3.9.5/tests/test_dtifit.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_ensure.py` & `fslpy-3.9.5/tests/test_ensure.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 #
 # test_ensure.py -
 #
 # Author: Paul McCarthy <pauldmccarthy@gmail.com>
 #
 
+import pathlib
 
 import numpy   as np
 import nibabel as nib
 
 import fsl.utils.tempdir as tempdir
 import fsl.utils.ensure  as ensure
 
@@ -18,16 +19,18 @@
 def test_ensureIsImage():
 
     with tempdir.tempdir():
         img = make_random_image('image.nii')
 
         assert ensure.ensureIsImage(img) is img
 
-        loaded = [ensure.ensureIsImage('image.nii'),
-                  ensure.ensureIsImage('image')]
+        loaded = [ensure.ensureIsImage(             'image.nii'),
+                  ensure.ensureIsImage(             'image'),
+                  ensure.ensureIsImage(pathlib.Path('image')),
+                  ensure.ensureIsImage(pathlib.Path('image.nii'))]
 
         for l in loaded:
             assert isinstance(l, nib.nifti1.Nifti1Image)
             assert np.all(np.asanyarray(img.dataobj) == np.asanyarray(l.dataobj))
 
         l = None
         loaded = None
```

### Comparing `fslpy-3.9.4/tests/test_featanalysis.py` & `fslpy-3.9.5/tests/test_featanalysis.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_featdesign.py` & `fslpy-3.9.5/tests/test_featdesign.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_featimage.py` & `fslpy-3.9.5/tests/test_featimage.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_filetree/test_query.py` & `fslpy-3.9.5/tests/test_filetree/test_query.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_filetree/test_read.py` & `fslpy-3.9.5/tests/test_filetree/test_read.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_filetree/test_registration.py` & `fslpy-3.9.5/tests/test_filetree/test_registration.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_filetree/test_template.py` & `fslpy-3.9.5/tests/test_filetree/test_template.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_fixlabels.py` & `fslpy-3.9.5/tests/test_fixlabels.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_freesurfer.py` & `fslpy-3.9.5/tests/test_freesurfer.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_fsl_data_utils.py` & `fslpy-3.9.5/tests/test_fsl_data_utils.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_fsl_utils_path.py` & `fslpy-3.9.5/tests/test_fsl_utils_path.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_fslsub.py` & `fslpy-3.9.5/tests/test_fslsub.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_gifti.py` & `fslpy-3.9.5/tests/test_gifti.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_idle.py` & `fslpy-3.9.5/tests/test_idle.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_image.py` & `fslpy-3.9.5/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_image_data_access.py` & `fslpy-3.9.5/tests/test_image_data_access.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_image_resample.py` & `fslpy-3.9.5/tests/test_image_resample.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_image_roi.py` & `fslpy-3.9.5/tests/test_image_roi.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_immv_imcp.py` & `fslpy-3.9.5/tests/test_immv_imcp.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_importall.py` & `fslpy-3.9.5/tests/test_importall.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_melodicanalysis.py` & `fslpy-3.9.5/tests/test_melodicanalysis.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_melodicimage.py` & `fslpy-3.9.5/tests/test_melodicimage.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_memoize.py` & `fslpy-3.9.5/tests/test_memoize.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_mesh.py` & `fslpy-3.9.5/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_meta.py` & `fslpy-3.9.5/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_mghimage.py` & `fslpy-3.9.5/tests/test_mghimage.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_naninfrange.py` & `fslpy-3.9.5/tests/test_naninfrange.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_notifier.py` & `fslpy-3.9.5/tests/test_notifier.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_parse_data.py` & `fslpy-3.9.5/tests/test_parse_data.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_platform.py` & `fslpy-3.9.5/tests/test_platform.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_run.py` & `fslpy-3.9.5/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_atlasq_list_summary.py` & `fslpy-3.9.5/tests/test_scripts/test_atlasq_list_summary.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_atlasq_ohi.py` & `fslpy-3.9.5/tests/test_scripts/test_atlasq_ohi.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_atlasq_query.py` & `fslpy-3.9.5/tests/test_scripts/test_atlasq_query.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_fsl_abspath.py` & `fslpy-3.9.5/tests/test_scripts/test_fsl_abspath.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_fsl_apply_x5.py` & `fslpy-3.9.5/tests/test_scripts/test_fsl_apply_x5.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_fsl_convert_x5.py` & `fslpy-3.9.5/tests/test_scripts/test_fsl_convert_x5.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_fsl_ents.py` & `fslpy-3.9.5/tests/test_scripts/test_fsl_ents.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_imglob.py` & `fslpy-3.9.5/tests/test_scripts/test_imglob.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_imln.py` & `fslpy-3.9.5/tests/test_scripts/test_imln.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_immv_imcp.py` & `fslpy-3.9.5/tests/test_scripts/test_immv_imcp.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_imrm.py` & `fslpy-3.9.5/tests/test_scripts/test_imrm.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_imtest.py` & `fslpy-3.9.5/tests/test_scripts/test_imtest.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_remove_ext.py` & `fslpy-3.9.5/tests/test_scripts/test_remove_ext.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_resample_image.py` & `fslpy-3.9.5/tests/test_scripts/test_resample_image.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_scripts/test_vest2text.py` & `fslpy-3.9.5/tests/test_scripts/test_vest2text.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_settings.py` & `fslpy-3.9.5/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_tempdir.py` & `fslpy-3.9.5/tests/test_tempdir.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/test_affine.py` & `fslpy-3.9.5/tests/test_transform/test_affine.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/test_flirt.py` & `fslpy-3.9.5/tests/test_transform/test_flirt.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/test_fnirt.py` & `fslpy-3.9.5/tests/test_transform/test_fnirt.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/test_nonlinear.py` & `fslpy-3.9.5/tests/test_transform/test_nonlinear.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/test_x5.py` & `fslpy-3.9.5/tests/test_transform/test_x5.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/nonlinear/coefficientfield.nii.gz` & `fslpy-3.9.5/tests/test_transform/testdata/nonlinear/coefficientfield.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/nonlinear/displacementfield.nii.gz` & `fslpy-3.9.5/tests/test_transform/testdata/nonlinear/displacementfield.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/nonlinear/displacementfield_no_premat.nii.gz` & `fslpy-3.9.5/tests/test_transform/testdata/nonlinear/displacementfield_no_premat.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/nonlinear/ref.nii.gz` & `fslpy-3.9.5/tests/test_transform/testdata/nonlinear/ref.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/nonlinear/src.nii.gz` & `fslpy-3.9.5/tests/test_transform/testdata/nonlinear/src.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_axisBounds.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_axisBounds.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_compose.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_compose.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_concat.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_concat.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_flirtMatrixToSform.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_flirtMatrixToSform.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_invert.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_invert.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_scaleoffsetxform.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_scaleoffsetxform.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_00.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_00.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_01.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_01.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_02.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_02.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_03.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_03.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_04.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_04.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_05.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_05.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_06.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_06.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_07.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_07.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_08.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_08.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_09.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_09.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_10.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_10.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_11.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_11.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_12.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_12.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_13.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_13.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_14.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_14.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_15.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_15.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_16.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_16.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_17.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_17.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_18.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_18.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_19.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_19.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_20.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_20.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_transform/testdata/test_transform_test_transform_coords.txt` & `fslpy-3.9.5/tests/test_transform/testdata/test_transform_test_transform_coords.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_version.py` & `fslpy-3.9.5/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_vest.py` & `fslpy-3.9.5/tests/test_vest.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_volumelabels.py` & `fslpy-3.9.5/tests/test_volumelabels.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_vtk.py` & `fslpy-3.9.5/tests/test_vtk.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_weakfuncref.py` & `fslpy-3.9.5/tests/test_weakfuncref.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_wrappers/test_fslstats.py` & `fslpy-3.9.5/tests/test_wrappers/test_fslstats.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_wrappers/test_wrappers.py` & `fslpy-3.9.5/tests/test_wrappers/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/test_wrappers/test_wrapperutils.py` & `fslpy-3.9.5/tests/test_wrappers/test_wrapperutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -471,14 +471,52 @@
 
         res = basefunc(img, 'myout', myout=wutils.LOAD)
         assert np.all(np.asanyarray(res['myout_times5'] .dataobj) == exp1)
         assert np.all(np.asanyarray(res['myout_times10'].dataobj) == exp2)
         cleardir(td, 'myout*')
 
 
+def test_fileOrThing_pathlib():
+    @wutils.fileOrImage('img', 'out')
+    def basefunc(img, out):
+        img    = np.asanyarray(nib.load(img).dataobj)
+        outimg = nib.nifti1.Nifti1Image(img * 5,  np.eye(4))
+        nib.save(outimg, out)
+
+    with tempdir.tempdir() as td:
+        img = nib.nifti1.Nifti1Image(np.array([[1, 2], [3, 4]]), np.eye(4))
+        exp = np.asanyarray(img.dataobj) * 5
+        nib.save(img, 'img.nii')
+
+        basefunc(pathlib.Path('img.nii'), pathlib.Path('output.nii'))
+        assert np.all(np.asanyarray(nib.load('output.nii') .dataobj) == exp)
+
+
+def test_fileOrThing_outprefix_pathlib():
+    @wutils.fileOrImage('img', outprefix='output_base')
+    def basefunc(img, output_base):
+        img = np.asanyarray(nib.load(img).dataobj)
+
+        out1 = nib.nifti1.Nifti1Image(img * 5,  np.eye(4))
+        out2 = nib.nifti1.Nifti1Image(img * 10, np.eye(4))
+
+        nib.save(out1, '{}_times5.nii.gz' .format(output_base))
+        nib.save(out2, '{}_times10.nii.gz'.format(output_base))
+
+    with tempdir.tempdir() as td:
+        img  = nib.nifti1.Nifti1Image(np.array([[1, 2], [3, 4]]), np.eye(4))
+        exp1 = np.asanyarray(img.dataobj) * 5
+        exp2 = np.asanyarray(img.dataobj) * 10
+        nib.save(img, 'img.nii')
+
+        basefunc(pathlib.Path('img.nii'), pathlib.Path('myout'))
+        assert np.all(np.asanyarray(nib.load('myout_times5.nii.gz') .dataobj) == exp1)
+        assert np.all(np.asanyarray(nib.load('myout_times10.nii.gz').dataobj) == exp2)
+
+
 def test_fileOrThing_outprefix_differentTypes():
 
     @wutils.fileOrImage('img', outprefix='outpref')
     def func(img, outpref):
 
         img  = nib.load(img)
         img  = nib.nifti1.Nifti1Image(np.asanyarray(img.dataobj) * 2, np.eye(4))
```

### Comparing `fslpy-3.9.4/tests/testdata/example.mgz` & `fslpy-3.9.5/tests/testdata/example.mgz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/example.shape.gii` & `fslpy-3.9.5/tests/testdata/example.shape.gii`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/example.surf.gii` & `fslpy-3.9.5/tests/testdata/example.surf.gii`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/example4D.shape.gii` & `fslpy-3.9.5/tests/testdata/example4D.shape.gii`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/example4D_multiple_darrays.shape.gii` & `fslpy-3.9.5/tests/testdata/example4D_multiple_darrays.shape.gii`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/example_bad1.surf.gii` & `fslpy-3.9.5/tests/testdata/example_bad1.surf.gii`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/example_bad2.surf.gii` & `fslpy-3.9.5/tests/testdata/example_bad2.surf.gii`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/example_bad3.surf.gii` & `fslpy-3.9.5/tests/testdata/example_bad3.surf.gii`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/example_bad4.surf.gii` & `fslpy-3.9.5/tests/testdata/example_bad4.surf.gii`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/example_bad5.surf.gii` & `fslpy-3.9.5/tests/testdata/example_bad5.surf.gii`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/example_bad6.surf.gii` & `fslpy-3.9.5/tests/testdata/example_bad6.surf.gii`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/example_dicom.tbz2` & `fslpy-3.9.5/tests/testdata/example_dicom.tbz2`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/cluster_zstat2_std.txt` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/cluster_zstat2_std.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/confoundevs.txt` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/confoundevs.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/design.fsf` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/design.fsf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/design.mat` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/design.mat`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.par` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf.par`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf_final.par` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_1.feat/mc/prefiltered_func_data_mcf_final.par`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/confoundevs.txt` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/confoundevs.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/design.fsf` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/design.fsf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/design.mat` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/design.mat`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.par` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf.par`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf_final.par` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_2.feat/mc/prefiltered_func_data_mcf_final.par`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/confoundevs.txt` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/confoundevs.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/design.con` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/design.con`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/design.fsf` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/design.fsf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/design.mat` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/design.mat`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.par` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf.par`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_diff.dat` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_diff.dat`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_final.par` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_3.feat/mc/prefiltered_func_data_mcf_final.par`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/design.fsf` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/design.fsf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/design.mat` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/design.mat`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.par` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_nostats.feat/mc/prefiltered_func_data_mcf.par`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/design.fsf` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/design.fsf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/design.mat` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/design.mat`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/filtered_func_data.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/filtered_func_data.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/res4d.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/res4d.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/1stlevel_realdata.feat/stats/threshac1.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/1stlevel_realdata.feat/stats/threshac1.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/cluster_zstat1_std.txt` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/cluster_zstat1_std.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/design.fsf` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/design.fsf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/lmax_zstat1_std.txt` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope1.feat/lmax_zstat1_std.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/design.fsf` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/cope2.feat/design.fsf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_1.gfeat/design.fsf` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_1.gfeat/design.fsf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/cluster_zstat1_std.txt` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/cluster_zstat1_std.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/design.fsf` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/design.fsf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/lmax_zstat1_std.txt` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope1.feat/lmax_zstat1_std.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/cluster_zstat1_std.txt` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/cluster_zstat1_std.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/design.fsf` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/design.fsf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/lmax_zstat1_std.txt` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/cope2.feat/lmax_zstat1_std.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_2.gfeat/design.fsf` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_2.gfeat/design.fsf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/bg_image.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/bg_image.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/cluster_zstat1_std.txt` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/cluster_zstat1_std.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/design.fsf` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/design.fsf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/example_func.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/example_func.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/filtered_func_data.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/filtered_func_data.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/lmax_zstat1_std.txt` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/lmax_zstat1_std.txt`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/mean_func.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/mean_func.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/rendered_thresh_zstat1.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/rendered_thresh_zstat1.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/cope1.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/cope1.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/pe1.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/pe1.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/res4d.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/res4d.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/tstat1.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/tstat1.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/varcope1.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/varcope1.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/zstat1.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/stats/zstat1.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/thresh_zstat1.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/thresh_zstat1.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/var_filtered_func_data.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope1.feat/var_filtered_func_data.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/design.fsf` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/design.fsf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/example_func.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/example_func.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/filtered_func_data.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/filtered_func_data.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/mean_func.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/mean_func.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/rendered_thresh_zstat1.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/rendered_thresh_zstat1.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/cope1.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/cope1.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/pe1.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/pe1.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/res4d.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/res4d.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/tstat1.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/tstat1.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/varcope1.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/varcope1.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/zstat1.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/stats/zstat1.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/var_filtered_func_data.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/cope2.feat/var_filtered_func_data.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/design.fsf` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/design.fsf`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_feat/2ndlevel_realdata.gfeat/mean_func.nii.gz` & `fslpy-3.9.5/tests/testdata/test_feat/2ndlevel_realdata.gfeat/mean_func.nii.gz`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_mesh.vtk` & `fslpy-3.9.5/tests/testdata/test_mesh.vtk`

 * *Files identical despite different names*

### Comparing `fslpy-3.9.4/tests/testdata/test_mesh_data.txt` & `fslpy-3.9.5/tests/testdata/test_mesh_data.txt`

 * *Files identical despite different names*

