pkgname=nhwd
pkgver=18.02
pkgrel=1
pkgdesc="Namib Hardware Detection"
arch=('i686' 'x86_64')
url="https://github.com/meerkatbrowser/nhwd"
license=("GPL")
depends=('nhwd-db')
makedepends=('git')

build() {
  cd ..
  mkdir -p build
  cd build
  cmake ../
  make
}

package() {
  cd ..
  cd build
  make DESTDIR=${pkgdir} install
}

