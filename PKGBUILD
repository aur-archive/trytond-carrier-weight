# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-carrier-weight
_pkgname=trytond_carrier_weight
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The carrier_weight module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-carrier>=3.4' 'trytond-company>=3.4' 'trytond-currency>=3.4' 'trytond-product>=3.4' 'trytond-product-measurements>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("77028bf10467f1dccfd72c3b29fd0275")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}