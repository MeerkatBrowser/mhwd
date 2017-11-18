pkgname=nhwd
pkgver=17.11
pkgrel=1
pkgdesc="Namib Hardware Detection"
arch=('i686' 'x86_64')
url="https://github.com/meerkatbrowser/nhwd"
license=("GPL")
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

