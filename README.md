# ghostscript
#Custom built Ghostscript package to mirror old environment
#Built with these options
wget http://www.imagemagick.org/download/delegates/ghostscript-9.22.tar.gz 
tar xvzf ghostscript-9.22.tar.gz cd ghostscript-9.22 
./configure --enable-dynamic --enable-freetype --enable-fontconfig --enable-openjpeg --disable-compile-inits --with-drivers=ALL --with-fontpath="/usr/share/fonts/urw-fonts /usr/share/fonts/Type1 /usr/share/fonts /usr/share/poppler/cMap/Adobe-CNS1 /usr/share/poppler/cMap/Adobe-GB1 /usr/share/poppler/cMap/Adobe-Japan1 /usr/share/poppler/cMap/Adobe-Japan2 /usr/share/poppler/cMap/Adobe-Korea1" --with-ijs --with-jbig2dec --with-libpaper --without-luratech --disable-cups --with-system-libtiff 
make 
checkinstall
