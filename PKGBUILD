# Contributor: DsTr <kostindima@gmail.com>

pkgname=qconf
pkgver=1.4
pkgrel=2
pkgdesc="QConf allows you to have a nice configure script for your qmake-based project."
arch=(i686 x86_64 ppc)
url="http://delta.affinix.com/qconf/"
license=('GPL')
depends=(qt)
makedepends=()
provides=(qconf-svn)
conflicts=(qconf-svn)
replaces=(qconf-svn)
source=(http://delta.affinix.com/download/qconf-$pkgver.tar.bz2)
md5sums=(e0080044f88c31e032008d5a5682a112)

build() {
  cd $srcdir/qconf-$pkgver
  ./configure --prefix=/usr
  make
  make INSTALL_ROOT="$pkgdir" install
}
