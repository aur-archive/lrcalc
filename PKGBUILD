# Maintainer: Antonio Rojas <nqn76sw@gmail.com>

pkgname=lrcalc
pkgver=1.2
pkgrel=1
pkgdesc="Littlewood-Richardson calculator"
arch=('i686' 'x86_64')
url="http://math.rutgers.edu/~asbuch/lrcalc/"
license=('GPL2')
depends=()
source=("http://math.rutgers.edu/~asbuch/lrcalc/$pkgname-$pkgver.tar.gz")
md5sums=('6bba16c0cca9debccd0af847bd3d4a23')

build() {
  cd $pkgname-$pkgver
  ./configure --prefix=/usr
  make
}

package() {
  cd $pkgname-$pkgver
  make install DESTDIR="$pkgdir"
}

