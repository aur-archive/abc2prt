# Contributor: Eric Forgeot < http://ifiction.free.fr >
pkgname=abc2prt
pkgver=1.0.2
pkgrel=1
pkgdesc="A simple tool to extract parts from multivoice ABC music files."
arch=(i686 x86_64)
url="http://abcplus.sourceforge.net/"
license=('gpl')
#depends=('')
source=(http://abcplus.sourceforge.net/${pkgname}-${pkgver}.tar.gz)
#md5sums=(' ')


build() {

    cd $srcdir/${pkgname}-${pkgver}
    mkdir -p $pkgdir/usr/share/abc2prt
    mkdir -p $pkgdir/usr/bin
    
    make || return 1
    
    cp $srcdir/${pkgname}-${pkgver}/README $pkgdir/usr/share/abc2prt
    cp $srcdir/${pkgname}-${pkgver}/*.abc $pkgdir/usr/share/abc2prt
    cp $srcdir/${pkgname}-${pkgver}/abc2prt $pkgdir/usr/bin

}

