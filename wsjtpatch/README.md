How to compile console decoder jt65:

```
svn co -r 7579 svn://svn.code.sf.net/p/wsjt/wsjt/branches/wsjtx
cd wsjtx
wget https://github.com/alexander-sholohov/spot_decoder/raw/master/wsjtpatch/spot-wsjtx-r7579.patch
svn patch spot-wsjtx-r7579.patch
mkdir build
cd build
cmake -DWSJT_SKIP_MANPAGES=ON -DWSJT_GENERATE_DOCS=OFF ..
make jt65
```

Done. Please find jt65 at current directory.  

Prerequirements:  
sudo apt-get install libfftw3-dev  
gcc 4.8.4 or later  
sudo apt-get install gfortran  

