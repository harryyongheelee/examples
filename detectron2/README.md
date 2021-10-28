# Detectron2

Run Detectron2 example on Vessl:
* Dataset mount
  1. Create a new dataset with a public S3 bucket directory `s3://savvihub-public-apne2/detectron2`.
  2. Mount the dataset to `/input/balloon` at the experiment create form.
* Start Command
  ```bash
  pip install -r examples/detectron2/requirements.txt && python examples/detectron2/main.py
  ```
### Troubleshooting
* `nvcc fatal   : Unsupported gpu architecture 'compute_86'`
  * Refer to https://github.com/facebookresearch/detectron2/issues/149#issuecomment-737039021