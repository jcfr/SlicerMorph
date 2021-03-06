# Slicer Morph
This is the development repository for our NSF ABI grant

SlicerMorph enable biologists to retrieve, visualize, measure and annotate high-resolution specimen data both from volumetric scans (CTs and MRs) as well as from 3D surface scanners effectively within 3D-Slicer. It also provides a Generalized Procrustes Analysis (GPA) module as well as tools to visualize PCA decomposition of the GPA results.

## Module Descriptions
- **ConvertMorphologikaLandmarks:** Imports a Morphologika formatted landmark file that may contain multiple subjects and exports a Slicer .FCSV landmark file for each individual to a directory specified by the user.
- **GPA:** Performs generalized Procrustes analysis (GPA) with or without scaling and principle component analysis (PCA) of shape from landmark data and provides visualizations of statistical output.
- **ImportSurfaceToSegment:** Imports a 3D surface model as a segmentation and prompts the user to edit it using the Segment Editor module.
- **MorphoSource:** MorphoSource is a publicly available repository for 3D media representing biological specimens. This module provides convenient access and data import from M/S directly into Slicer.
- **ReadLandmarkFile:** Imports IDAV landmark editor files with header length specified by the user.
- **SkyscanReconImport:** Imports an image stack from Bruker/Skyscan reconstruction software (Nrecon) with correct voxel spacing and orientation as a 3D volume.

## License
See License.md
