# h5py-aarch64
This repository provides an h5py wheel for AArch64 architecture. Currently there is only `h5py-3.1.0-cp36-cp36m-linux_aarch64.whl` which is built on Jetson TX2. If you need other versions, feel free to open an issue.

If you have an AArch64 device, you can build your own version by

```bash
sudo env H5PY_SETUP_REQUIRES=0 pip3 download -d /ssddata/h5py h5py==3.1.0
sudo env H5PY_SETUP_REQUIRES=0 pip3 wheel -w /ssddata/h5py h5py=3.1.0
```

The release also includes the source file tarball of the corresponding version `h5py` and wheels of `cached_property` and `numpy` built together with `h5py`.
