# Maintainer: BlackEagle < ike DOT devolder AT gmail DOT com >
# vim:syntax=sh
pkgname=closure-linter
pkgver=2.3.5
pkgrel=2
pkgdesc="A JavaScript style checker and style fixer"
arch=('any')
url="http://code.google.com/closure"
license=('APACHE')
depends=('python2' 'python2-gflags')
makedepends=('python2-distribute')
source=("http://$pkgname.googlecode.com/files/${pkgname/-/_}-$pkgver.tar.gz")

build() {
	cd ${pkgname/-/_}-$pkgver
	python2 setup.py build
}

package() {
	cd ${pkgname/-/_}-$pkgver
	python2 setup.py install --root="$pkgdir"
}
sha256sums=('3c5fc9d3eb7c62f6d203a136a8bc37e89b80c467603c37dbc5a2626145abd93d')
