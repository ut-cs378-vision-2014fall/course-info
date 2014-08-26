## Installing the Python / Numpy / OpenCV Stack

### Mac OS X 10.9 (Mavericks)

#### Step 1: Install [Homebrew](http://brew.sh), the OS X package manager

```bash
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
brew doctor
```

#### Step 2: Install OpenCV packages

```bash
brew tap homebrew/science
brew install opencv
mkdir -p ~/Library/Python/2.7/lib/python/site-packages
echo '/usr/local/lib/python2.7/site-packages' > ~/Library/Python/2.7/lib/python/site-packages/homebrew.pth
```

#### Step 3: Check that it worked

Invoke the Python interpreter, and import the OpenCV package. If there are no errors, you're in business!

```bash
python
import cv2
```

### Ubuntu Linux 14.04

#### Step 1: Install OpenCV packages

```bash
sudo apt-get install python-opencv
```

#### Step 2: Check that it worked

Invoke the Python interpreter, and import the OpenCV package. If there are no errors, you're in business!

```bash
python
import cv2
```