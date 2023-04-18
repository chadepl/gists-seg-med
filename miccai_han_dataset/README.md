# MICCAI head and neck dataset

You can find the MICCAI head and neck dataset at [this](https://www.imagenglab.com/newsite/pddca/) link.
Download and uncompress `PDDCA part 1`, `PDDCA part 2`, `PDDCA part 3` and `PDDCA description`, and put them into a folder with the following structure:
- `miccai_data`
  - `pddca.odt` 
  - `PDDCA-1.4.1_part1` 
  - `PDDCA-1.4.1_part2`
  - `PDDCA-1.4.1_part3`
    
The folder `miccai_data` is the source dir for the function at `process_patients.py`.
The function `convert_to_numpy` transforms the dataset from the `nrrd` format to more familiar `numpy` arrays.
After converting the dataset to a suitable array format, you can check the patients' data using `patient_vis.py`.

These two files demonstrate basic usage of the following libraries, which are common in medical image segmentation:
- `numpy`: array manipulation.
- `SimpleITK`: image processing, geared towards 3D medical images.
- `napari`: interactive volume visualizer.