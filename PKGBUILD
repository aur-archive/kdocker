# Maintainer: DonVla <donvla@users.sourceforge.net>

pkgname=kdocker
pkgver=4.8
pkgrel=3
pkgdesc="dock any application into the system tray"
arch=('i686' 'x86_64')
url="https://launchpad.net/kdocker"
license=(GPL)
depends=('qt4')
source=("http://launchpad.net/${pkgname}/trunk/${pkgver}/+download/${pkgname}-${pkgver}.tar.gz")
md5sums=('19bc0a6c9435f57e407c381d7bb2b220')
sha256sums=('16e5d6dab6957139343b29d2bab7d1f7154d74bb4a60dace897b23cf6f8921a9')

build() {
    cd "${srcdir}/${pkgname}-${pkgver}"
    qmake-qt4 && make
}                                                                                                                                                                                                                                                                                                                              

package(){
    cd "${srcdir}/${pkgname}-${pkgver}"
    make INSTALL_ROOT="${pkgdir}" install
}                 
