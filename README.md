# vrepper

Tethered V-REP (using V-REP as a remote controlled multi-body simulator) in Python.

The Python binding (`vrep.py` and friends) and the driver libraries (`remoteApi.dll` and `remoteApi.dylib`) is copied as-is from V-REP PRO EDU V3.4

## Usage

Add the path to your V-REP installation to your `PATH`:

- (Windows) might be something like `C:/Program Files/V-REP3/V-REP_PRO_EDU/`

  ```bash
  $ set PATH=%PATH%;C:/Program Files/V-REP3/V-REP_PRO_EDU/
  ```

- (Mac OS X) might be something like `/Users/chia/V-REP_PRO_EDU/vrep.app/Contents/MacOS/`

  ```bash
  $ export PATH=$PATH:"/Users/chia/V-REP_PRO_EDU/vrep.app/Contents/MacOS/"
  ```

Then run the following:

```bash
$ cd vrepper
$ pip install -e . #(install the vrepper package in edit mode)
$ ipython test_body_joint.py #(run the example)
```

The last command will start V-REP in headless mode (no GUI) and run a simple simulation step-by-step. Then it will shut itself down and exit.

## Why should you use V-REP

- build your model with its GUI tools
- simulate your model with whatever programming language you like

## Why should you use vrepper

If you are looking for:

- remote controlled simulation
- low overhead communication
- ability to start/stop simulation repeatedly to perform all kinds of experiment

Then vrepper has already paved the way for you. You should at least take a look at vrepper's source code.
